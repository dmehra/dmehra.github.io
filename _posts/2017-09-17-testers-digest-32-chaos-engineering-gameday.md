---
title: "Tester's Digest #32: Chaos Engineering and GameDay Exercises"
excerpt: Chaos Engineering tells us to experiment in production to validate fault tolerance of our systems. This is not for the faint hearted! With practical writeups from companies who have run Chaos-inspired GameDay exercises.
---

TESTER'S DIGEST
===============
ISSUE #32 - September 17, 2017

Chaos Engineering tells us to experiment in production to validate fault tolerance of our systems. This is not for the faint hearted! With practical writeups from companies who have run Chaos-inspired GameDay exercises.

Topic: Chaos Engineering and GameDay Exercises
==============================================

Principles of Chaos Engineering are outlined here as a living community-maintained document:

<http://principlesofchaos.org/>

The above originated at Netflix, the makers of Chaos Monkey tool for random fault injection. This post describes their Chaos Kong exercise and another experiment with Subscriber service in 2015:

<https://medium.com/netflix-techblog/chaos-engineering-upgraded-878d341f15fa>

What is Chaos Engineering, by Gremlin guys who promise to provide fault injection as a service:

<https://blog.gremlininc.com/the-discipline-of-chaos-engineering-e39d2383c459>

The argument for, and practice of, running GameDay exercises in production at Etsy (back in 2012!)

<http://queue.acm.org/detail.cfm?id=2353017>

Datadog ran a Game Day event on their ElasticSearch cluster, describes results of different faults here:

<https://www.datadoghq.com/blog/elasticsearch-game-day/>

PagerDuty included a Chaos-inspired Breakathon event in their recent summit:

<https://www.pagerduty.com/blog/breakathon-details/>

There are really good arguments in favor of testing your system for fault resistance directly in production:

<https://opensource.com/article/17/8/testing-production>

But what if you are a medium-size startup with high-value customers, and the idea of injecting failures into production environment doesn't sit well with you? Or perhaps you want to intentionally go beyond the tolerance limits of your system to train the team on incident response? That was us at Quid, so we ran a GameDay in staging, and described how we organized the event:

<http://technology.quid.com/2017/09/our-first-engineering-game-day/>

Off-Topic
=========

Great overview of learning resources for today's test engineer:

<https://techbeacon.com/3-ways-qa-engineers-can-keep-pace-developers>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
