# Why We Deprecate

As humans, we know hoarding is bad for the psyche. As engineers, we see the value of refactoring, [deleting old code](https://www.infoq.com/news/2017/02/dead-code), [writing code so it's easy to delete](https://programmingisterrible.com/post/139222674273/write-code-that-is-easy-to-delete-not-easy-to), [pruning irrelevant tests](https://testzius.wordpress.com/2017/04/20/prune-your-automation/). As product managers and UX designers, we need to retire old features when we add new, shiny features.

Here is what happens when we fail at deprecation - not quite from the realm of software, but true story.

My local greenbelt had a doggy poo bag dispenser. A very simple one. One might call it the MVP of doggy poo bag dispensers: it was just a box with a lid, filled with small plastic bags (shown here without the bags).

![image 1]({{ site.url }}/assets/why-we-deprecate/doggy_poo_1.png){:width="50%"}

As a good MVP should, this dispenser fulfilled the basic user need of getting a doggy poo bag out when one is needed... and no more. It had no access controls, a malicious or naive user could take all the bags out in one go. It was only sort of weatherproof, having a lid against rain, but easy to be left open with the lid up. The UX of having to open the lid to take a bag out was inconvenient in requiring two hands, when the user likely had one hand occupied with the leash. It was unlabeled, with no usage instructions. It had a poor supporting framework, literally a stick in the ground. It was flimsy. It was not pretty.

The designers always envisioned a followup to this MVP, and perhaps it took longer to roll out than expected. Meanwhile the original dispenser had a number of bugs reported against it, the biggest one being: the lid broke off. The doggy poo bags got wet in the rain, but the bug was deprioritized given that v2 was coming very soon, and anyway California was in a drought. Then finally, the new and improved dispenser was deployed!

![image 2]({{ site.url }}/assets/why-we-deprecate/doggy_poo_2.png){:width="50%"}

Oh, it was brilliant. Improved UX that supports "make the right thing easy and the wrong thing hard" principle: one-handed operation resulting in removal of exactly one doggy poo bag! Access controls meet quotas meet load shedding: it's impossible to accidentally pull out all the bags! Fault tolerance: the dispenser is entirely weatherproof, cemented into the ground, and hard to break! In-product documentation included!

Okay, maybe v2 had some glitches, such as replacement of see-through design that made it easy to know when bags started to run low, with an opaque design. All that can be addressed in v3 with utilization metrics reporting to a centralized city-wide doggy poo bag dispenser dashboard, automated refills by drone, and/or growing new organic bags in place. Meanwhile, v2 is a clear improvement over v1, so we rejoice.

One problem though. The old, now lidless dispenser is still there.

Why's that? Wouldn't you just remove it when putting the new one in? Ah... well... say, v2 was done by a different team. How do they know that v1 is safe to remove? Maybe it serves a need. Maybe there's a user cohort who are unable to use v2 for some legacy reason and must stick with the original dispenser. What if there's a reason why the lid bug was never fixed in the first place? It is conceivable that some users could only take doggy poo bags out of an open-top dispenser, so we should leave it for them. If we are not the people who made the old dispenser, we may feel that we lack the authority to remove it. And if the MVP makers are now out of the picture, we don't even know how to ask them. So we keep things as they are "just in case".

What happens next, given that users see a gorgeous dispenser of doggy poo bags and an empty box next to it?

They start putting bags full of doggy poo into the old dispenser.

![pile-of-poo emoji]({{ site.url }}/assets/why-we-deprecate/pile_of_poo_emoji.png)

If we love and respect our users, we shall conclude that they mistake the dispenser for a trash can. If we have other feelings toward our users, we might conclude that they are too lazy to walk the ten steps over to the real trash can. Either way, we have a problem. A P1 escalation ticket gets filed for the old dispenser filling up with doggy poo. A lively discussion ensues, in which we still fail to locate the original makers of the dispenser, and therefore cannot make the call to just remove the damn thing. The decision? Clean out the current load of poo and introduce a warning message:

"Poop bags go in the garbage can, NOT IN HERE"

![image 3]({{ site.url }}/assets/why-we-deprecate/doggy_poo_3.png){:width="50%"}

Victory! Our literate users no longer place poo into the box. It remains gloriously empty and well labeled.

Until one day the original maintainers of the MVP dispenser get to their bug backlog and decide to address the missing-lid ticket. While working on the issue, they discover the odd warning label that was placed onto their product for no good reason. There's no poo problem here! Why would one possibly have a useless warning like this, that could insult the user's intelligence?! The lid is reinstated. The warning is gone.

We now have 2 perfectly functional dispensers right next to each other.

![image 4]({{ site.url }}/assets/why-we-deprecate/doggy_poo_4.jpg){:width="50%"}

The newer dispenser gets refilled by the support team. The older one does not, but there it is, taking up space and setting stage for a reoccurrence of "this is not a trash can" incident. I will continue to check on it and publish updates if and when a new chapter in this saga takes place.

Meanwhile... deprecate your old features if you don't want a product full of crap.
