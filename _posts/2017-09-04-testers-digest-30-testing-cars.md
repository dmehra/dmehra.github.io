---
title: "Tester's Digest #30: Testing Cars"
excerpt: Modern cars are like Oreo cookies with hardware on the outside and lots of gooey software in the middle. How do you test that?
---

TESTER'S DIGEST
===============
ISSUE #30 - September 4, 2017

Modern cars are like Oreo cookies with hardware on the outside and lots of gooey software in the middle. How do you test that?

Topic: Testing Cars
===================

How much software is there inside modern cars? You could use LOC (number of lines of code) to estimate, check out the beautiful visualization of LOC in different things:

<http://www.informationisbeautiful.net/visualizations/million-lines-of-code/>

However, there are caveats in this type of accounting. This post explains how a Mercedes reports 20x LOC of an F-35 bomber while probably not being "more complex":

<http://joebarkai.com/fallacy-behind-counting-lines-of-code/>

Also, LOC may not be a good beacon for complexity in the world of machine learning where you can train a model to steer a car in 99 lines of code. Ok, this is in simulation and relies on libraries like TensorFlow which in itself is near 1 million LOC at this time, but still. I was not able to find LOC estimates for self driving cars.

<https://blog.coast.ai/training-a-deep-learning-model-to-steer-a-car-in-99-lines-of-code-ba94e0456e6a>

How do you test self driving cars? Waymo uses their Carcraft simulation software and physical structured testing at the Castle base in Central Valley, CA, where they built out a kind of city for robotic cars to navigate. They translated 20,000 scenarios from structured testing into simulation, and additionally apply fuzzing technique to play out more variations.

<https://www.theatlantic.com/technology/archive/2017/08/inside-waymos-secret-testing-and-simulation-facilities/537648/>

Tesla's approach seems to rely on "shadow mode" data collection from its Autopilot-enabled vehicle fleet, and early access users (car owners) who pay for the privilege of beta testing the self-driving features. These articles have a decidedly negative sentiment toward Tesla, but their reasoning seems sound to me.

<https://www.wired.com/story/tesla-drivers-are-paying-big-bucks-to-test-flawed-self-driving-software/>

<http://www.betabreakers.com/tesla-motors-skips-beta-test-phase-new-vehicle/>

In Porshe's manufacturing process for the Panamera 2017 model, described here in 12 steps, the steps 1-5, 8, and 12 are largely testing. That's >50%.

<https://www.wired.com/2016/10/painstaking-process-building-porsche-panamera/>

Off-Topic
=========

An example of a misconfiguration bug/error with an outsized impact: Google takes down Internet in most of Japan by misconfiguring BGP peer prefixes for Verizon. The second post has all the technical detail for BGP geeks.

<https://thenextweb.com/google/2017/08/28/google-japan-internet-blackout/>

<https://bgpmon.net/bgp-leak-causing-internet-outages-in-japan-and-beyond/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
