---
title: "Tester's Digest #7: Technical Debt"
excerpt: Our topic this week is technical debt, as a few good posts caught my eye.
---

TESTER'S DIGEST
===============
ISSUE #7 - Mar 19, 2017

---

This issue is cobbled together in haste due to a new baby arriving ahead of schedule. Please excuse possible newsletter delays over the next few weeks. Our topic this week is technical debt, as a few good posts caught my eye.

Topic: Technical Debt
=====================

Thoughts on technical debt from a developer's perspective. Interestingly, the acceptability of taking on tech debt is not left up to the developer, but instead framed as a conscious business decision:

<https://devblog.dymel.pl/2017/03/16/technical-debt/>

Managing technical debt based on "old debt is bad and new debt is good" principle, a debt ceiling, and scientific looking charts:

<http://blog.crisp.se/2013/10/11/henrikkniberg/good-and-bad-technical-debt>

The "iron triangle" model of looking at technical debt says that any project faces tradeoffs between schedule, cost and scope (that's the triangle), with the hidden 4th being quality; imagine it being the area of the triangle. If you bend the sides inwards by taking shortcuts, you're squeezing the quality out. Has specific recommendations for managing technical debt if JIRA is your tool - wish it went into more detail on that.

<https://www.clearvision-cm.com/blog/avoid-technical-debt-jira-iron-triangle/>

Identifying and quantifying architectural debt, from a 2016 ICSE paper. The technique looks at cooccurrence of code changes in file sets over time to identify changes that stem from architectural debt. Analysis of several Apache projects suggests that this type of debt accounts for 85% of the total project maintenance effort!

<https://blog.acolyer.org/2016/06/13/identifying-and-quantifying-architectural-debt/>

Managing "process debt" (bugs, testcases, documentation) as a variety of technical debt. I like the concept of auto-closing bugs that have been dormant with no updates for >6 months with a note "Will Not Fix - Over Six Months Old".

<https://dojo.ministryoftesting.com/lessons/when-testers-deal-with-process-debt-ideas-to-manage-it-and-get-back-to-testing-faster>

Lessons from scaling Twitter - broader than technical debt alone, of course, but does touch on the topic. "There is no such a thing as a temporary change or workaround: In most cases, workarounds are tech debt":

<https://blog.twitter.com/2017/the-infrastructure-behind-twitter-scale>

On the intersection of product quality (less is more, when it comes to features) and classic quality (absence of bugs, maintainability), and an angle on technical debt (if you take it on, you have to pay it back), from Spotify:

<https://labs.spotify.com/2014/04/11/qualities-of-quality/>


Off-Topic
=========

You know how you should always test for short and long input strings, right? Not everyone does; so a single-character first or last name, or 67 middle names, easily breaks many governmental record keeping systems.

<https://agiletestingdays.com/blog/exclusive-excerpt-from-gojko-adzics-new-book-computer-says-no-names-that-make-computers-go-crazy/>

These high-reliability practices could have prevented the 2017 Oscars ceremony epic fail:

<https://www.forbes.com/sites/davidmarquet/2017/03/10/avoid-an-oscar-epicfail-4-practices-for-high-reliability/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
