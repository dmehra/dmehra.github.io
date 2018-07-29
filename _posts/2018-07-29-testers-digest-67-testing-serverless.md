---
title: "Tester's Digest #67: Testing Serverless"
excerpt: Challenges of testing in the serverless world of Lambda functions running on a FaaS platform
---

TESTER'S DIGEST
===============
ISSUE #67- July 29, 2018

We looked at testing microservices last week, let's expand to the new frontier of serverless architecture, a world of Lambda functions running on a FaaS (Function-As-A-Service) platform. I do not yet have first-hand experience of testing in this setup myself, learning along with you from authors who describe it.

Topic: Testing Serverless
=========================

What is serverless, anyway? Here is Martin Fowler’s intro, including a chapter on testing a serverless app, which basically says “unit testing is easy, integration testing is hard”:

<https://martinfowler.com/articles/serverless.html>

How is serverless different from, or similar to, microservices?

<https://www.stratoscale.com/blog/compute/keeping-small-serverless-functions-vs-microservices/>

Comprehensive post on changing your approach to testing as you go serverless, including the shift in your test pyramid (more integration tests, cheaper UI tests), how to write testable serverless functions, and more.

<https://medium.freecodecamp.org/the-best-ways-to-test-your-serverless-applications-40b88d6ee31e>

A good philosophical discussion of test boundaries in the serverless architecture:

<https://read.acloud.guru/testing-and-the-serverless-approach-495cef7495ea>

A practical writeup on testing serverless at Yubl. For context, Yubl was a British social network startup which went out of business, but I doubt that outcome had anything to do with their testing strategy. They went with the premise “don’t mock services that you can’t change” and placed emphasis on integration/end-to-end testing.

<https://hackernoon.com/yubls-road-to-serverless-part-2-testing-and-ci-cd-72b2e583fe64>

Tips on making serverless functions testable (the examples are for the Node.js serverless framework, points apply more broadly): separate your business logic from the FaaS provider, set up event mocks, test in both local and remote invocation modes.

<https://serverless.com/framework/docs/providers/aws/guide/testing/>

What does chaos testing look like in a serverless world where you don’t control the failure of FaaS components and can’t unleash a chaos monkey tool on them? The first post is going on 2 years old, the other two are newer and offer up some ideas.

<https://serverless.zone/monkeyless-chaos-integration-testing-for-serverless-architectures-9d1a4208c3ca>

<https://hackernoon.com/chaos-engineering-and-aws-lambda-latency-injection-ddeb4ff8d983>

<https://github.com/serverless/guide/blob/master/source/dev/testing.md>

If you run into a failure in serverless world, how will you debug it? The author of this post sets up 3 testcases: causing timeout of a lambda function under load; improper format of the lambda function (i.e. coding bug); and error due to insertion of a duplicate key. Each scenario is debugged with these observability tools: AWS X-Ray, Dashbird, Thundra, IOPipe, all of which are judged immature to some degree.

<https://hackernoon.com/benchmarked-serverless-observability-tools-got-very-disappointed-e54f5e3381bf>


Off-Topic
=========

Akin’s laws of spacecraft design (broadly applicable to software engineering):

<https://spacecraft.ssl.umd.edu/akins_laws.html>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
