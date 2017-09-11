---
title: "Tester's Digest #31: Testing Airplanes"
excerpt: Tester's Digest is about software, yet most interesting things combine hardware and software. Like cars (covered in the last issue) and airplanes. Today we look at testing Boeing 737 MAX, Southwest test flights, wind tunnels, and debugging a plane crash. In off-topic section, more hardware including a slot machine.
---

TESTER'S DIGEST
===============
ISSUE #31 - September 10, 2017

Tester's Digest is about software, yet most interesting things combine hardware and software. Like cars (covered in the last issue) and airplanes. Today we look at testing Boeing 737 MAX, Southwest test flights, wind tunnels, and debugging a plane crash.

Topic: Testing Airplanes
========================

Stress testing the new Boeing 737 MAX - 3 min video with not much detail but lots of eye candy. More videos (but not much more details) from Boeing itself.

<https://www.wired.com/2016/10/inside-737-test-plane-boeing-beats-bejesus/>

<http://www.boeing.com/commercial/737max/creating-the-737-max>

The article about Southwest's 5-day testing of the 737 MAX for "Service Ready Operational Validation" gives a better sense of what happy-path testing for an aircraft looks like: planned missed approach test, deicing, boarding/deplanning, charging and use of other ground equipment, covering 225 operational conditions.

<https://airwaysmag.com/industry/southwest-boeing-737-max-8-srov/>

If you're hungry for more detail, this blog post covers the experience of being on one of those test flights by Southwest:

<http://www.airliners.net/forum/viewtopic.php?f=9&t=961887>

The flipside of testing is debugging the issues that happen despite our best efforts at prevention. Here is a look at debugging the worst possible outcome in aviation: a plane crash. Highlights the importance of a clear human-computer interface, and not allowing the UI to silence cautions from the system about its own malfunction.

<https://fearoflanding.com/accidents/accident-reports/when-both-your-mind-and-your-instruments-are-lying/>

Minimum acceptable code coverage for aviation software is set by DO-178B standard. This post sheds some light on the requirements but I can't tell you any more due to the scary warning not to copy any part of the document without permission. Fair use, people...

<http://www.bullseye.com/minimum.html>

Badass testing tool: world's largest wind tunnel.

<https://www.wired.com/2017/02/climb-inside-worlds-largest-wind-tunnel/>

Off-Topic
=========

Shock test for a storage box - a really big storage box, Amazon's Snowball Edge.

<http://venturebeat.com/2017/03/12/watch-aws-shock-test-its-snowball-edge-data-storage-box-with-underwater-explosives/>

How would you test a slot machine?

<https://www.stickyminds.com/article/qa-slot-machines-testing-randomization-winning-combinations-and-big-payouts>


---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
