---
title: "Tester's Digest #15: Failure Injection"
excerpt: Today's theme is failure injection testing, prominently featuring Netflix who gave the world ChaosMonkey. In the off-topic section you will find a few fun email bugs.
---

TESTER'S DIGEST
===============
ISSUE #15 - May 14, 2017

---

Today's theme is failure injection testing, prominently featuring Netflix who gave the world ChaosMonkey. In the off-topic section you will find a few fun email bugs.

Topic: Failure Injection
========================

Why is fault injection testing important? Because "sooner or later, all complex systems will fail. It’s not a matter of if, it’s a matter of when." Breaking things on purpose, at a time and in a way that is convenient, is much preferable to having them break as a surprise to you.

<https://blog.gremlininc.com/breaking-things-on-purpose-a519c0f5698b>

From Twitter, description of their failure injection testing in production
(supported failure conditions being power down, service down, network down):

<https://blog.twitter.com/2015/how-we-break-things-at-twitter-failure-testing>

From Netflix, the well known "Chaos Monkey" and the rest of the Simian Army,
n use since 2011 to randomly break your production system and see if it is in fact
fault tolerant. This is not for the faint of heart:

<http://techblog.netflix.com/2011/07/netflix-simian-army.html>

Using Chaos Monkey to kill your EC2 instances in a controlled way from command line (with background on how Chaos Monkey is normally used):

<https://medium.com/production-ready/using-chaos-monkey-whenever-you-feel-like-it-e5fe31257a07#.fxf0q61qc>

Netflix later developed a FIT (Failure Injection Testing) tool for more control:

<http://techblog.netflix.com/2014/10/fit-failure-injection-testing.html>

Here is an example of Netflix using Latency Monkey (from the Simian Army suite)
and FIT to test their Merchandise Application Platform:

<http://techblog.netflix.com/2015/08/from-chaos-to-control-testing.html>

The academic underpinning for Netflix's failure testing was this paper on "Lineage-driven fault injection". It is a technique for reasoning backwards from correct system outcomes to determine whether failures could have prevented that outcome (if so, those are bugs). The paper describes a prototype called MOLLY.

<https://people.eecs.berkeley.edu/~palvaro/molly.pdf>

Netflix expanded on MOLLY thus:

<http://techblog.netflix.com/2016/01/automated-failure-testing.html>

Using errfs, a file system layer that simulates block corruption, read/write errors and out of space conditions, researchers find that distributed storage systems (incl. Redis, ZooKeeper, Cassandra, Kafka, RethinkDB, MongoDB, LogCabin, and CockroachDB) will silently corrupt data, lose data, or return unexpected errors, despite the fault being injected in a single node while the system is configured for redundancy. While this is bad news, having a new testing tool in addition to Jepsen.io is great!

<https://blog.acolyer.org/2017/03/08/redundancy-does-not-imply-fault-tolerance-analysis-of-distributed-storage-reactions-to-single-errors-and-corruptions/>

Off-Topic
=========

I was reminded of an Internet-famous email bug, and came across a couple more, for your reading pleasure:

"We can't send email more than 500 miles". Yes this story is real, as recently confirmed by the author on HackerNews. If any technical details in it bother you, see FAQ.

<https://www.ibiblio.org/harris/500milemail.html>

Microsoft Exchange email explosion on "Bedlam DL3", also known as "Me Too!"

<https://blogs.technet.microsoft.com/exchange/2004/04/08/me-too/>

A multi time zone variation on the same unintentional reply-all DDOS attack, prompted by "Free bananas in the kitchen!!!"

<http://www.metafilter.com/78177/PLEASE-UNSUBSCRIBE-ME-FROM-THIS-LIST#2408665>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
