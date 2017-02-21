TESTER'S DIGEST
===============
ISSUE #3 - Feb 20th, 2017

---

I try to focus on one main topic in each weekly issue of Tester's Digest,
with news sprinkled in.

Topic: Testing Distributed Systems
==================================

In today's world, you'd have to be in a rather niche space to *not* be testing distributed systems, so most aspects apply whether you're testing a system built on microservices, a web app that relies on AWS for its backend, an online game, or a large-scale NoSQL database. Global village, you know.

This remains required reading for newcomers to distributed systems (testers and coders alike):

<https://www.somethingsimilar.com/2013/01/14/notes-on-distributed-systems-for-young-bloods/>

Great list of testing resources:

<https://github.com/asatarin/testing-distributed-systems>

The challenges of scaling a system, as experienced by Uber, with "what I wish I knew" style lessons, and a prominent mention of load and failure testing:

<http://highscalability.com/blog/2016/10/12/lessons-learned-from-scaling-uber-to-2000-engineers-1000-ser.html>

How Facebook does load testing in production (live! but safely)

<https://blog.acolyer.org/2016/11/28/kraken-leveraging-live-traffic-tests-to-identify-and-resolve-resource-utilization-bottlenecks-in-large-scale-web-services/>

How do you uncover bugs in distributed storage systems during testing, rather than in production? These Microsoft folks exercised a test harness against systems written in the .NET framework, and found 8 bugs in MS Azure products that were hard to find with traditional testing techniques.

<https://blog.acolyer.org/2016/05/05/uncovering-bugs-in-distributed-storage-systems-during-testing-not-in-production/>

The two posts above come from The Morning Paper, a blog I hugely respect.

On the probability of data loss in large clusters, with the math (subtly incorrect, so be sure to read the comments about replication time being a factor in mean time to data loss):

<http://martin.kleppmann.com/2017/01/26/data-loss-in-large-clusters.html>

News
====

A recent post on migrating data at scale, safely (Stripe's account, pretty standard dual-writing approach). Does not cover the testing angle... left as an exercise to the reader?

<https://stripe.com/blog/online-migrations>


Fun
===

One approach to spreading good testing practices while, uh, not spreading germs. I swear this is not an April Fool's post:

<https://testing.googleblog.com/2007/01/introducing-testing-on-toilet.html>

As proof that the above was not a joke, here is the most recent installment of Testing on the Toilet, direct from Google's restrooms to yours:

<https://testing.googleblog.com/2017/01/testing-on-toilet-keep-cause-and-effect.html>

There were maybe a dozen posts total over the years, search for "testing on the toilet" to see them all.

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
