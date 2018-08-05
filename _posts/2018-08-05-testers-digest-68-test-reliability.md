---
title: "Tester's Digest #68: Test Reliability"
excerpt: Since automated tests are code, and code is inherently buggy, how do you increase test reliability?
---

TESTER'S DIGEST
===============
ISSUE #68 - August 5, 2018

Unreliable regression tests can be worse than no tests whatsoever. At the same time, automated tests are code, and code is inherently buggy. How do you reconcile these statements, assuming you agree with both? Let's look at what folks do to increase test reliability.

Topic: Test Reliability
=======================

Focus on keeping your test suite lean, meaning: valuable, reliable and fast.

<https://www.techwell.com/techwell-insights/2018/06/3-ways-keep-your-test-suite-lean>

Flaky UI tests may point out performance issues with the app, result from accidental load testing or concurrency - that's the technical side. On the human side, flaky tests can serve as a barometer of the team's attention to issues.

<https://www.stickyminds.com/article/what-flaky-tests-can-tell-you>

False positive and false negatives in automated tests, and how to avoid them. There's no silver bullet: "This will undoubtedly take time, effort, and craftsmanship up front". Design your tests with proper exception handling and synchronization, "test your tests", and audit them periodically.

<https://www.stickyminds.com/article/start-trusting-your-test-automation-again>

How do you know if your automated tests are doing the right thing? Perhaps, you periodically sample them for execution by hand, just like they QA cookies in a cookie factory:

<https://medium.com/the-test-sheep/the-biscuit-factory-model-for-test-sampling-25270185100b>

Run tests multiple times against the same "stability build" to uncover flaky behavior of the system under test, or tests themselves:

<http://katrinatester.blogspot.nl/2018/01/a-stability-strategy-for-test-automation.html>

Quarantining failing tests (unless it’s for a very short time) is a bad practice:

<https://testbitsblog.wordpress.com/2018/04/04/quarantining-failing-tests-is-a-death-sentence/>

Off-Topic
=========

Worth learning: how to read an RFC (Request For Comments, originally for Internet protocol specifications):

<https://www.mnot.net/blog/2018/07/31/read_rfc>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
