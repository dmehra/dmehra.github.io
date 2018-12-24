---
title: "Tester's Digest #78: Testing At Scale"
excerpt: On test automation in large, microservice based systems.
---

TESTER'S DIGEST
===============
ISSUE #78 - December 23, 2018

Today's topic is test automation in large systems, which these days tends to mean a distributed, microservice based architecture. Since Google has just about the largest system under test, a couple of posts are from their blogs.

Topic: Testing At Scale
=======================

Google selects which tests to run at pre-submit stage (ie: on a developer's branch) and which to skip, to save resources. The selection is made by an ML model, trained on their gigantic test execution history. All relevant tests will still run in CI, but there is a cost to skipping a test which would have failed in pre-submit, since the CI build will break and revert will be required. The model can be tuned to trade off specificity vs sensitivity.

<https://testing.googleblog.com/2018/09/efficacy-presubmit.html>

How Google identifies which code change broke the build - the paper is heavy on statistics:

<https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45794.pdf>

Facebook employs a static code analysis tool (Infer) paired up with ML-based system (Getafix) that automatically suggests fixes for common bugs, mostly null pointer exceptions, but that alone covers a lot of ground:

<https://code.fb.com/developer-tools/getafix-how-facebook-tools-learn-to-fix-bugs-automatically/>

All of the above is amazing stuff that made engineers on my team salivate. Of course, most of us won't have a use for tooling of such complexity. Before moving on to a post that's more applicable to human-scale engineering, a word of warning: you may not need microservices at all.

<http://blog.jenkster.com/2018/07/microservices-check-size.html>

If you are on a microservice based architecture already or considering a move to one, this post nicely lays out the testing challenges you will face, and a promising approach: consumer-driven contract testing at the API layer between services, using a framework like Pact.

<https://hackernoon.com/how-to-test-microservices-with-consumer-driven-contracts-9bf5c2c05349>


Off-Topic
=========

This 4 year old can have a bright future in QA:

<https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/commit/?id=690b0543a813b0ecfc51b0374c0ce6c8275435f0>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
