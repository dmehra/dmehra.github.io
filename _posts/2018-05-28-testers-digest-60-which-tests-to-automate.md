---
title: "Tester's Digest #60: Which Tests To Automate"
excerpt: How should you approach the selection of test cases for automating? Some answers are informed by the testing pyramid, others by statistics.
---

TESTER'S DIGEST
===============
ISSUE #60 - May 28, 2018

How should you approach the selection of test cases for automating? Some answers are informed by the testing pyramid, others by statistics.

Topic: Which Tests To Automate
==============================

A nice take on the testing pyramid and its application to test automation. The author suggests using the pyramid as a mental model, not as a set of guidelines to the tune of "X% of your tests should be unit tests". Don't miss his practical example of testing a shopping website, it’s in the comments (search for “electronic cigarettes”).

<http://www.ontestautomation.com/why-and-how-i-still-use-the-test-automation-pyramid/>

Deeper analysis of what the pyramid may look like in different environments and why:

<https://blog.gurock.com/how-much-ui-automation-do-you-need/>

Yet another look at the testing pyramid, this time with microservices in mind (although there is nothing microservice specific about the post):

<https://medium.com/@nathankpeck/microservice-testing-introduction-347d2f74095e>

3 ways to fail at end-to-end test automation, and 1 possible path to success -- using automated tooling to supplement manual testing:

<https://www.stickyminds.com/article/tales-test-automation-failure-and-how-find-success>

How Google selects automated regression tests to run from the safety perspective: “Would skipping this test target miss a transition?”

<https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46740.pdf>

How can you decide which parts of the code need test coverage, particularly when inheriting an old codebase with poor test coverage? This approach uses measurements of cyclomatic complexity of the classes and coupling (i.e. usage of one class by others) to locate classes worth testing.

<https://www.toptal.com/software/coupling-and-cyclomatic-complexity>

Do's and don'ts of test automation, presented as visual tiles.

<http://kavliwashere.com/starting-up-test-automation/>

Off-Topic
=========

This checklist is so old yet still so relevant -- "Is it the first of the month?" bit us more than once in the last couple of years! Would be cool to come up with a list like this, updated for 2018 tech stack.

<http://everythingsysadmin.com/dumb-things-to-check.html>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
