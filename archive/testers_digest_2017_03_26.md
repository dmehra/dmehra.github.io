TESTER'S DIGEST
===============
ISSUE #8 - Mar 26, 2017

---

This issue focuses on the how and why of postmortems. We touched on catastrophic failures in an earlier newsletter:

<http://testersdigest.mehras.net/archive/testers_digest_2017_03_05.html>

What is one to do if the catastrophe already occurred? Learn from it, by running a postmortem analysis.

Topic: Postmortems And Root Cause Analysis
==========================================

Do not look for a single root cause, as catastrophe is never caused by one person or one software bug, but a combination of factors including your organizational processes that jointly contribute to the disastrous outcome:

<http://www.kitchensoap.com/2012/02/10/each-necessary-but-only-jointly-sufficient/>

If you're not familiar with the Swiss Cheese model of accident causation, it's worth a look:

<https://en.m.wikipedia.org/wiki/Swiss_cheese_model>

This great slide deck covers accident causality, RCA (Root Cause Analysis) principles such as "what you look for is what you find" (beware!), types of accident models that go beyond Swiss Cheese, including non-linear ones. It also poses a question that was new to me: do we learn better from rare accidents, or from the daily safe operation, and should we shoot for making the system "more safe" or "less unsafe"?

<http://www.uis.no/getfile.php/Konferanser/Presentasjoner/Ulykkesgransking%202010/EH_AcciLearn_short.pdf>

To quote from the deck above, "The purpose of learning (from accidents, etc.) is to change behaviour so that certain outcomes become more likely and other outcomes less likely". This should be the ultimate goal of your postmortem analysis.

Many advocate "The 5 Whys" approach to running a postmortem, with the aim of getting from proximate causes to root causes of the incident. The 5 Whys comes from a Toyota tradition:

<http://www.toyota-global.com/company/toyota_traditions/quality/mar_apr_2006.html>

Eric Ries of "The Lean Startup" picked it up and ran with it as a tool for finding human causes of technical problems:

<https://www.fastcodesign.com/1669738/to-get-to-the-root-of-a-hard-problem-just-ask-why-five-times>

If you prefer Eric on video, HBR has one:

<https://hbr.org/2012/02/the-5-whys.html>

Example of using The 5 Whys in a startup postmortem, by Buffer:

<https://open.buffer.com/5-whys-process/>

More recently, GitLab used The 5 Whys in the postmortem of their data loss outage:

<https://about.gitlab.com/2017/02/10/postmortem-of-database-outage-of-january-31/>

The danger of naive application of The 5 Whys method is in digging deeply to a single root cause, rather than going for broad understanding of multiple contributing factors. An alternative is a debriefing that asks "how?" rather than "why?" (the post links to tutorials at the end).

<http://www.kitchensoap.com/2014/11/14/the-infinite-hows-or-the-dangers-of-the-five-whys/>

Note that the above critique is different from "5 whys and 5 hows" where the hows are just an inversion of the whys: "Why did the system fail? - Because the database was overloaded. How do we address that? - Let's add more DB capacity". That type of "hows" is simply a way to express action items from the postmortem. You will find it in some posts that I'm not quoting here as they tend to be surface level.

SRECon presentation that cautions against homing in on "bad software" (or hardware) in your root cause analysis:

<https://www.usenix.org/conference/srecon17americas/program/presentation/gibson>

Good tips on structuring your postmortems:

<https://medium.com/production-ready/writing-your-first-postmortem-8053c678b90f#.akqz3vlms>

<https://medium.com/production-ready/on-finding-root-causes-c0ce524bf98b#.tysbsk5a0>

<https://tech.shutterstock.com/2016/11/11/5-ways-to-hone-your-production-incident-postmortems/>

And if you'd like a ready-made tool to manage postmortems, Etsy's got Morgue:

<https://github.com/etsy/morgue/>

Off-Topic
=========

What happened to the GitLab engineer who served as the proximate cause of their data loss incident? He received lots of support from the company and the wider community, and is doing well. A great reminder to fix your process and not blame your people after an outage/catastrophe:

<https://about.gitlab.com/2017/03/17/how-is-team-member-1-doing/>

A most amusing time waster, "The Daily WTF is your how-not-to guide for developing software" and the premier place to post funny bugs you encounter when using software. Now I wish I kept a screenshot of my kids' public school enrollment form with the question "Are you Hispanic or Latino?" and non-binary answer choices "Yes / No / Other"...

<http://thedailywtf.com/>

Emoji URL shortener! Here it is, linking back to Tester's Digest. Those emoji are :bridge_at_night: :no_bicycles: :chipmunk:

<http://mosho.ws/🌉🚳🐿>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
