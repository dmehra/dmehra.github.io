---
title: "Tester's Digest #66: Testing Microservices"
excerpt: What is different about testing in the world of microservice architecture?
---

TESTER'S DIGEST
===============
ISSUE #66 - July 22, 2018

What is different about testing in the world of microservice architecture?

Topic: Testing Microservices
============================

How do you test a system built on the microservice architecture? Unit tests are here to stay, but don't help cover the "pathological unpredictability" of distributed systems. You'll be doing a lot more integration tests, and testing in production. This post has a lot more depth, heed it.

<https://medium.com/@copyconstruct/testing-microservices-the-sane-way-9bb31d158c16>

Unit tests for microservices, or more broadly, for components of distributed systems:

<https://medium.com/@nathankpeck/microservice-testing-unit-tests-d795194fe14e>

After switching to a micro service architecture, team ran into unexpected performance degradations in prod. Their solution was to introduce chaos testing in the staging environment, to supplant classic unit and QA testing.

<https://searchmicroservices.techtarget.com/feature/How-a-SaaS-provider-made-microservices-deployment-safely-chaotic>

Fault injection testing of microservices with Gremlin, a companion to ChaosMonkey (not the same Gremlin as the Chaos-as-a-service provider, this one is an open source Python SDK):

<https://developer.ibm.com/open/2016/06/06/systematically-resilience-testing-of-microservices-with-gremlin/>

Problems one should expect when adopting microservice architecture, from Segment's engineering team who did the shift, then went back to monolith, and can speak to the tradeoffs:

<https://segment.com/blog/goodbye-microservices/>

Off-Topic
=========

Fun bug story -- a single-character typo cripples AI capabilities of “Aliens: Colonial Marines” game monsters for years:

<https://arstechnica.com/gaming/2018/07/a-years-old-one-letter-typo-led-to-aliens-colonial-marines-awful-ai/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
