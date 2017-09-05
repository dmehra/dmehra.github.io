---
title: "Tester's Digest #29: Levels of Testing"
excerpt: Levels of Testing. -- We look at testing levels, from unit tests to functional and end-to-end system tests, and how to determine where to focus one's testing efforts.
---

TESTER'S DIGEST
===============
ISSUE #29 - August 27, 2017

---

Tester's Digest is back after a short vacation! We look at testing levels, from unit tests to functional and end-to-end system tests, and how to determine where to focus one's testing efforts.

Topic: Levels of Testing
========================

A really good overview of automated testing, unit vs integration tests, using testing DSLs such as Cucumber, prioritizing tests, managing them as code, costs of automated testing and how to lower them.

<http://www.lihaoyi.com/post/PrinciplesofAutomatedTesting.html>

The testing pyramid, with a wide base of unit tests and a narrow peak of end-to-end tests, is a familiar pictogram of the "right way to test". Here it is, reimagined as a bug filter:

<https://twitter.com/noahsussman/status/836612175707930625?lang=en>

The "wrong way to test" would be the dreaded ice-cream cone, with few unit tests and most coverage focused in expensive, slow, flaky end-to-end tests. This post presents it as the testing cupcake... yummy and bad for you:

<https://www.thoughtworks.com/insights/blog/introducing-software-testing-cupcake-anti-pattern>

Traditional testing phases revamped and combined into a "threaded" approach:

<http://testerkiwi.blogspot.co.nz/2017/05/phased-vs-threaded-testing.html>

We looked at this post from Google in a past issue, but worth mentioning in the context of testing levels: at Google, tests are broken into 3 categories: small, medium and large. That loosely maps to unit, functional and end-to-end system tests, but the distinction is based more on runtime than anything else. The post digs into metrics on test flakiness and shows, unsurprisingly, that large tests are least reliable, and should only be used where lower-level tests won't provide the needed coverage.

<https://testing.googleblog.com/2017/04/where-do-our-flaky-tests-come-from.html>

For more on unit tests, see our older issue:

[Issue #12 - April 23, 2017]({{ site.baseurl }}{% post_url 2017-04-23-testers-digest-12-unit-tests %}) // Topic: Unit Tests

For more on end-to-end tests, see our older issue:

[Issue #11 - April 16, 2017]({{ site.baseurl }}{% post_url 2017-04-16-testers-digest-11-end-to-end-testing %}) // Topic: End-to-end Testing

Off-Topic
=========

To continue the subject of games started last time, here is a list of science based games:

<https://github.com/stared/science-based-games-list>

And games that teach assembly language while promising to be fun:

<http://spectrum.ieee.org/geek-life/reviews/three-computer-games-that-make-assembly-language-fun>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
