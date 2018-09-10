---
title: "Tester's Digest #71: Debugging"
excerpt: Ways to build up one's debugging technique, and some practical examples.
---

TESTER'S DIGEST
===============
ISSUE #71 - September 9, 2018

Debugging technique is something people tend to learn on the job, as you're not likely to find courses on "Debugging Theory" or practical seminars, which is too bad. Our current issue covers some approaches and a couple of specific debugging tales, with more available in the earlier Tester's Digest:

<http://testersdigest.mehras.net/2018/01/13/testers-digest-43-debugging-tales.html>

Topic: Debugging
=================

Testing vs debugging, and some debugging tips:

<http://www.abodeqa.com/differences-testing-debugging/>

Why having a screenshot of the user’s problem is highly valuable for the developer's debugging process:

<https://lotsog.blogspot.com/2018/03/a-screenshot-speaks-thousand-words.html>

A great discussion of differential diagnosis, a technique used in the medical field and directly applicable to debugging / troubleshooting, particularly when it’s not a solo endeavor but involves a team (when doesn’t it…)

<https://blog.danslimmon.com/2015/10/19/troubleshooting-chatops-ddx/>

From the same author, a strong recommendation to test with the aim of falsifying a hypothesis, not with the aim of confirming one:

<https://blog.danslimmon.com/2016/09/07/falsifiability-why-you-rule-things-out-not-in/>

Getting the bugs to reproduce can be the hardest thing. Fun story here of a Windows related bug, hunted down by the Israeli Army, and resulting thoughts on how to get the debugging data you need from real production bug occurrences.

<https://blog.sentry.io/2018/06/13/comedy-of-errors-rookout>

Neat overview (by the above Rookout guys) of different approaches to debugging production issues, from naive “Hail Mary” to intentional breaking things and reverting them, from monitoring to observability. The aside on “TDD cult” made me laugh.

<https://www.rookout.com/the-5-approaches-to-production-debugging/>

A complicated story of debugging a slow ssh connection to a machine:

<https://rachelbythebay.com/w/2018/03/16/slowroad/>

How to debug memory leaks in Node.js and in Java:

<https://www.toptal.com/nodejs/debugging-memory-leaks-node-js-applications>

<https://www.toptal.com/java/hunting-memory-leaks-in-java>


Off-Topic
=========

GitHub's announcement of "Project Paper Cuts" wherein the company shall start fixing annoying usability issues tickled me funny. Apparently, bug fixing qualifies as "exciting new ways".

<https://blog.github.com/2018-08-28-announcing-paper-cuts/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
