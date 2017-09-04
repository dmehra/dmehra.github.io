---
title: "Tester's Digest #12: Unit Tests"
excerpt: Today's theme is unit tests, a huge space, so don't expect exhaustive coverage!
---

TESTER'S DIGEST
===============
ISSUE #12 - Apr 23, 2017

---

Today's theme is unit tests, a huge space, so don't expect exhaustive coverage!

Topic: Unit Tests
=================

Why unit tests are worth the trouble:

<https://hackernoon.com/treat-yourself-e55a7c522f71#.cdbivs605>

A developer's approach to writing (mostly unit) tests:

<https://blog.nelhage.com/2016/12/how-i-test/>

Unit test tips from everydayunittesting.com which is a blog and a book "being written in an agile manner":

<http://www.everydayunittesting.com/2017/02/unit-testing-anti-pattern-asserting-on-not-null.html>

If your unit tests are difficult to write, that is a signal of poor design:

<http://www.drdobbs.com/testing/the-relationship-between-testability-and/240167101>

Test smells, i.e. markers of poor quality in your test code (not just for unit tests):

<http://xunitpatterns.com/Test%20Smells.html>

Always test these conditions or inputs: null, zero, one, many, too many. Obvious? I should hope so. But you still gotta do it. Every time.

<https://medium.com/sqa-mate/always-test-these-5-conditions-in-software-ed79d7a5cdd5#.joopscsv8>

A classic on using mock objects in your tests:

<https://martinfowler.com/articles/mocksArentStubs.html>

Best practices specific to RSpec, Ruby's BDD test framework:

<https://github.com/thoughtbot/guides/tree/master/best-practices#testing>

Sazerac is an interesting data-driven framework for Javascript unit tests:

<https://hackernoon.com/sazerac-data-driven-testing-for-javascript-e3408ac29d8c#.1b1fm0ipr>

Off-Topic
=========

Google's analysis of the degree of flakiness in their corpus of 4.2 million tests, broken down by test size/type. They find that "large" tests, i.e. end-to-end/integration tests, are the flakiest at 14% bogus failure rate over a week, compared to "small" (unit) tests at only 0.5%, and conclude that one needs to weigh whether to write a "large" test at all, and be careful if doing so.

<https://testing.googleblog.com/2017/04/where-do-our-flaky-tests-come-from.html>

While it's still April, this April's Fools post on reducing your MTTR for production incidents was the best. Achieve zero MTTR through skipping the investigation and resolution stages and simply auto-closing the tickets as soon as they are opened. Can be applied to bugs, too!

<https://victorops.com/blog/mttr-zero-one-weird-trick-solves-problems/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
