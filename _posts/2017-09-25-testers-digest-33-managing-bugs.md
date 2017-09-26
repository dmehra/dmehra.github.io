---
title: "Tester's Digest #33: Managing Bugs"
excerpt: Testing can reveal bugs, but having that information doesn't make the software any less buggy... someone still has to fix the bugs. All of them? Some of them? Which ones? Let's look at approaches to managing bugs.
---

TESTER'S DIGEST
===============
ISSUE #33 - September 25, 2017

Testing can reveal bugs, but having that information doesn't make the software any less buggy... someone still has to fix the bugs. All of them? Some of them? Which ones? Let's look at approaches to managing bugs.

Topic: Managing Bugs
====================

Startup switches to a "zero bug" policy, each new bug either gets fixed immediately or closed. Never needing a bug scrub sure sounds attractive - these guys were in "early days" at the time of posting, I'd be curious to hear how successful this turned out.

<https://devblog.songkick.com/experimenting-with-a-zero-bug-policy-3281490dbc8b>

Support-driven or complaint-driven development is an idea to “focus engineering effort on fixing the things users actually complain about", as practiced at Scalyr. The blog post focuses on issues that weren't bugs per se, but were generating support tickets, and their resolution both made customers happier and decreased support costs. Win/win! It strikes me as a rather reactive approach to fixing things if this is all you do... but can be a useful prioritization technique.

<https://blog.scalyr.com/2017/07/support-driven-development/>

From an SRE practitioner, lessons in building a successful escalation process that are fully applicable to bug triage in QA. Also extols the virtues of (useful) documentation:

<https://zwischenzugs.wordpress.com/2017/04/04/things-i-learned-managing-site-reliability-for-some-of-the-worlds-busiest-gambling-sites/>

How an agile team deals with bugs, among other things: "Bugs that deter the acceptance of a user story are fixed."

<https://testkeis.wordpress.com/2017/04/11/how-our-team-does-agile/>

On the common pitfalls of not prioritizing quality in agile development. Interesting recommendation to classify problems into "bugs" (it works predictably wrong) and "defects" (it works unpredictably) and committing to fix defects immediately, while bugs get weighed against new feature dev.

<http://www.startuplessonslearned.com/2008/10/engineering-managers-lament.html>

Tips on bug prioritization and setting up a workflow for bug management from friends over at Bugsnag. They are advocating the approach of proactive bug detection and management with their tool which is quite good!

<https://blog.bugsnag.com/bug-prioritization/>

<https://blog.bugsnag.com/debugging-workflow/>

Off-Topic
=========

A highly valuable study for teams who code in Javascript or other dynamic-typing languages: adding static type annotations to your code can prevent about 15% of bugs. For Javascript, use Flow or TypeScript, both are pretty good.

<https://blog.acolyer.org/2017/09/19/to-type-or-not-to-type-quantifying-detectable-bugs-in-javascript/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
