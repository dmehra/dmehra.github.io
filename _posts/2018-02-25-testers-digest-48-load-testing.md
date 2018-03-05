---
title: "Tester's Digest #48: Load Testing"
excerpt: We look at the classical QA task of load testing, with some modern twists.
---

TESTER'S DIGEST
===============
ISSUE #48 - February 25, 2018

Tester's Digest is back after a flu break. We look at the classical QA task of load testing, with some modern twists - should developers do it? should you load test in production? how can it all go wrong?

Topic: Load Testing
===================

Should developers write their own load tests, rather than have QA or another team do it for them? This post votes yes:

<https://engineering.klarna.com/four-reasons-developers-should-write-their-own-load-tests-fac74c1be9f1#.sizpzib0g>

How you can write load tests wrong: 1) make them too short; 2) ignore anomalies; 3) reuse test data (or rather, fail to disable caching); 4) only load test under happy path conditions with no failures.

<https://engineering.klarna.com/four-load-testing-mistakes-developers-love-to-make-68b443f7e8a2#.3ea8he5fu>

Additional uses of load tests: to help reproduce a sporadic performance issue, or to uncover app slowness based on user's location.

<https://www.stickyminds.com/article/using-load-testing-tools-more-just-load-testing>

Load testing of websites with Vegeta tool and test data in a Python Pandas dataframe:

<https://serialized.net/2017/06/load-testing-with-vegeta-and-python/>

Website Speed Test tool, built on top of the well known WebPagetest, analyzes load time of images on your website and makes improvement suggestions, complete with optimized images you can download and use:

<https://www.smashingmagazine.com/2017/07/website-speed-test-image-analysis-tool/>

Open source tools for load and stress testing (Fiddler, JMeter, Locust, Taurus, Gatling, Siege and more):

<https://www.joecolantonio.com/2017/07/18/open-source-performance-testing-tools/>

On different ways of setting up a load testing environment, from testing in production to rolling your own:

<https://www.stickyminds.com/article/six-tips-building-better-load-testing-environment>

Off-Topic
=========

Worth learning: Introduction to distributed systems. Per Lamport, 1987, "A distributed system is one in which the failure of a computer you didn't even know existed can render your own computer unusable". These days, there is no other kind of systems...

<https://caitiem.com/2017/09/07/getting-started-with-distributed-systems/>

<https://github.com/aphyr/distsys-class>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
