---
title: "Tester's Digest #5: Catastrophic Failures"
excerpt: Catastrophic Failures. -- This issue will focus on the nature of catastrophe and its prevention.
---

TESTER'S DIGEST
===============
ISSUE #5 - Mar 5, 2017

---

This issue will focus on the nature of catastrophe and its prevention.

Topic: Catastrophic Failures
============================

Great "short treatise on the Nature of Failure" that you'd swear was written by an engineer for engineers... actually it's by a medical doctor, published nearly 20 years ago in the context of patient diagnosis. If this link ever goes dead, just google "How Complex Systems Fail" by Richard I. Cook, MD.

<http://web.mit.edu/2.75/resources/random/How%20Complex%20Systems%20Fail.pdf>

If you'd like a discourse more targeted at software, here is an overview of "Why Systems Fail" with industry examples (also older, circa 2000):

<http://www.benmeadowcroft.com/reports/systemfailure/>

Related line of thought in a recent post on "Black Swans": the really bad things that seem improbable but have an outsized impact and get rationalized after the fact...

<https://asym.dk/2017/01/23/where-might-the-black-swans-be-lurking/>

Can we find the critical bugs that trigger real-life catastrophe? Yes, says this review of a few distributed systems (such as Cassandra and HDFS). 92% of catastrophic failures resulted from incorrect handling of simple error conditions. A third of those could have been found by a static code checker, and another third by code inspection with a little knowledge of the system. Also, 77% of production failures can be reproduced by a unit test, and 98% on a system with at most 3 nodes. Critical bugs are not that hard to uncover...

<https://blog.acolyer.org/2016/10/06/simple-testing-can-prevent-most-critical-failures/>

How bad can it get due to software bugs? Catastrophe porn:

The Role of Software in Recent Catastrophic Accidents, from 2009 IEEE Reliability Society report, covers airport shutdowns, plane crashes, NASA disasters, US/Canadian blackout of 2003 (hey, I was there!), and more:

<http://paris.utdallas.edu/IEEE-RS-ATR/document/2009/2009-17.pdf>

20 famous software disasters, covers time period 1962 to 2005, starting with Mariner 1 rocket, with cost / summary / cause for each:

<http://www.devtopics.com/20-famous-software-disasters/>

11 "epic failures", overlapping with the above but described in more detail: Mariner 1 again (punctuation matters), Mars Orbiter 1998 (watch your units), Pentium floating point flaw of 1994 (why it matters to fix a rare bug reported by a single user), and more:

<http://www.computerworld.com/article/2515483/enterprise-applications/epic-failures--11-infamous-software-bugs.html>

Another angle at the famous older incidents / accidents including Therac 25:

<http://www.cse.psu.edu/~gxt29/bug/softwarebug.html>

Award-worthy software failures of 2016. These guys also have older blog entries for prior years, and a detailed report available for download, which they apparently compile by searching English language news for verbiage on "software bugs". They cover magnitude of the incidents, but don't go into root causes.

<https://www.tricentis.com/blog/2017/03/01/software-fail-awards/>

News
====

What caused the AWS S3 outage on Feb 28th, Amazon's own summary:

<https://aws.amazon.com/message/41926/>

If you prefer a less dry retelling, The Verge will tell you it was due to a typo.
Keep in mind, however, that catastrophe never has a single cause...

<http://www.theverge.com/2017/3/2/14792442/amazon-s3-outage-cause-typo-internet-server>

It's not all doom and gloom. For those who still remember the Mad Gadget vulnerability in Apache Commons Collections back in late 2015, good news! Google employees organized a volunteer initiative, called Operation Rosehub, to find open source projects that were still affected, and submitted PRs to fix all 2600 of them. The world is more secure thanks to those folks.

<https://opensource.googleblog.com/2017/03/operation-rosehub.html>

Fun
===

When you are frustrated over this bug or that outage, head for the anger rooms!

<https://www.techwell.com/techwell-insights/2017/02/how-release-anger-work-without-getting-fired>

If you didn't get your fill of software disasters, Reddit will happily provide a daily dose:

<https://www.reddit.com/r/softwaregore/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
