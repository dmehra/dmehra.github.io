---
title: "Tester's Digest #14: On Maintenance"
excerpt: Today we talk about code maintenance and maintainability, a key factor in quality, in my experience. This necessarily connects to the topic of technical debt.
---

TESTER'S DIGEST
===============
ISSUE #14 - May 7, 2017

---

Today we talk about software maintenance and maintainability, a key factor in quality, in my experience. This necessarily connects to the topic of technical debt, see also an older issue:

[Issue #7 - March 19, 2017]({{ site.baseurl }}{% post_url 2017-03-19-testers-digest-7-technical-debt %}) // Topic: Technical Debt

Topic: On Maintenance
=====================

On software maintenance and it's substantial costs -- 80% of total project time anyone? The posts suggests ways to lower the burden of maintenance, but that part is specific to Erlang:

<http://ferd.ca/code-janitor-nobody-s-dream-everyone-s-job-and-how-erlang-can-help.html>

"Dead code is not dead until it's buried" and other thoughts on removing stale code, with a nod to Knight Capital disaster caused in part by activation of an old code path.

<https://www.infoq.com/news/2017/02/dead-code>

Maintenance is nearly synonymous with managing technical debt. According to this post, tech debt is not always quantifiable -- it is a metaphor, but with a real cost. Some examples are: lack of test coverage (!), hardcoded values, misused APIs, redundant code, brittle error handling, missing or inaccurate documentation, reliance on old versions of third-party code, and more.

<http://www.ontechnicaldebt.com/blog/can-technical-debt-be-quantified-the-limits-and-promise-of-the-metaphor/>

Tests need maintenance too! This post talks about pruning old / bad / irrelevant / duplicate tests. The one point I disagree with is the notion of retiring tests once a feature has matured because they won't be finding bugs any more - my take is that you keep them to catch possible regressions in old functionality introduced by new work, that is the whole point of regression testing. Otherwise, prune well and often!

<https://testzius.wordpress.com/2017/04/20/prune-your-automation/>

So, how does one go about building a maintainable system? Here are lessons from scaling Twitter, including "there is no such a thing as a temporary change or workaround: In most cases, workarounds are tech debt".

<https://blog.twitter.com/2017/the-infrastructure-behind-twitter-scale>

How to design (and build, and test) services for the real world:
* expect failures
* keep it simple
* automate all the things

<https://blog.acolyer.org/2016/09/12/on-designing-and-deploying-internet-scale-services/>

The post links out to a services checklist which is great for both dev and test:

<https://gist.github.com/acolyer/95ef23802803cb8b4eb5>

"Every line of code written comes at a price: maintenance." This post advocates writing disposable code over reusable code to minimize maintenance, counterintuitive as that sounds at first: "write code that is easy to delete, not easy to extend".

<http://programmingisterrible.com/post/139222674273/write-code-that-is-easy-to-delete-not-easy-to>

How (and why) to design your code for testability:

<https://blog.nelhage.com/2016/03/design-for-testability/>


Off-Topic
=========

Since one of the posts above references Knight Capital, here are 2 more to shed light on the 2012 event when the fund lost a lot of money due to an automated trading system snafu.

This very long read provides meta analysis of a sort-of-but-not-quite postmortem of the Knight Capital accident, worthwhile if you wish to understand what does and doesn't constitute a proper postmortem.

<http://www.kitchensoap.com/2013/10/29/counterfactuals-knight-capital/>

What actually happened at Knight, from devops perspective. Was it poor release engineering? Not enough automation? Error-prone process? This post offers analysis and insightful comments, too.

<https://dougseven.com/2014/04/17/knightmare-a-devops-cautionary-tale/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
