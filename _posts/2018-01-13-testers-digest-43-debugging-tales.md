---
title: "Tester's Digest #43: Debugging Tales"
excerpt: Debugging skills are hard won, and hard to teach. Here are some debugging stories to learn from.
---

TESTER'S DIGEST
===============
ISSUE #43 - January 13, 2018

Tester's Digest is back after a break for the holiday season, flu season, and performance review season! This issue is full of debugging stories. Debugging skills tend to be hard won through apprenticeship and trial-and-error, so I'm always excited when I come across writeups of specific situations to learn from.

Topic: Debugging Tales
======================

From debugging the Joyent outage of 5/27/2014, to thinking about the art and culture of debuggability, this is a great deck:

<https://www.slideshare.net/bcantrill/debugging-under-fire-keeping-your-head-when-systems-have-lost-their-mind>

Also from Joyent (as acquired by Samsung), a deck on finding unusual pathologies ("zebras not horses") in the data path:

<https://www.slideshare.net/bcantrill/zebras-all-the-way-down-the-engineering-challenges-of-the-data-path>

A story of a debugging deep dive, starting with investigation into a sudden traffic drop at the load balancer, then going into the nitty gritty of CPU and memory usage on the haproxy machines.

<https://blog.booking.com/troubleshooting-a-journey-into-the-unknown.html>

An instructive story of debugging a "flaky" test:

<http://blog.jgc.org/2013/07/your-test-suite-is-trying-to-tell-you.html>

Debugging a race condition in the Python Queue class, "a tragedy of deadlocks and despair":

<https://codewithoutrules.com/2017/08/16/concurrency-python/>

Debugging memory leaks in Ruby code:

<https://samsaffron.com/archive/2015/03/31/debugging-memory-leaks-in-ruby>

Debugging a data corruption issue in RavenDB: I appreciate not only the deep dive into the debugging process, but thoughts around prioritization (“All development ceases until [memory damage bug] is found”) and postmortem notes.

<https://ayende.com/blog/180481/production-postmortem-data-corruption-a-view-from-inside-the-sausage>

This debugging story is on its own level of awesome: guy decides to monitor his laptop’s resource utilization so he can be warned when, say, too many Chrome tabs are eating up too much memory (I need that!), but after setting up Prometheus, runs into a segfault crash. The investigation involves, among other things. a heat gun and building 32 kernels. Not to be missed.

<https://marcan.st/2017/12/debugging-an-evil-go-runtime-bug/>

Debugging one’s app slowdown via metrics as recorded by NewRelic and Honeycomb (with a bit of a plug for Honeycomb’s native support for high dimensional tag values):

<https://hackernoon.com/a-short-example-of-why-dimensions-are-suuuuuper-valuable-67e880055eb0>

Off-Topic
=========

Spectre and Meltdown have made the news so publicly that there's hardly a need to highlight them here. I will mention this article for its good coverage of the industry-standard process for vulnerability disclosure, and how it worked out differently with these bugs:

<https://www.theverge.com/2018/1/11/16878670/meltdown-spectre-disclosure-embargo-google-microsoft-linux>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
