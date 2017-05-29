---
description: This issue covers testing practices used at specific tech companies: Google, Facebook, Yelp, AirBnB, Atlassian.
---

TESTER'S DIGEST
===============
ISSUE #17 - May 28, 2017

---

This issue covers testing practices used at some high profile tech companies. Please send me links if you know of other good posts from industry leaders explaining their approach to testing.

Topic: Testing Practices At Tech Companies
==========================================

The rest of this list will be large companies, but the majority of tech companies are small or medium size startups. This "CTO's guide to Ops" offers up quality requirements of a startup with interesting maxims such as "Zealous testing isn’t a great use of time". Based on context, I posit that this hypothetical startup does not target enterprise customers. The pointers about metrics and logs are right on for any organization.

<https://medium.com/@cgroom/the-startup-ctos-guide-to-ops-1-of-3-guiding-principles-2607e21d9f89>

Yelp is proudly running 20 mln tests a day on 2 mln Docker containers, using a homegrown scalable, fault tolerant test runner called Seagull. Their test runtime is kept under 30 min due to parallelization.

<https://engineeringblog.yelp.com/2017/04/how-yelp-runs-millions-of-tests-every-day.html>

AirBnB now (as of Feb 2014) states that the important thing is to "test all the f***ing time" (TATFT). This post covers their journey from introduction of Pull Requests to building a culture of testing around those, from local testing to test automation running in CI and having a large reliable test suite.

<http://nerds.airbnb.com/testing-at-airbnb/>

Atlassian approaches QA as Quality Assistance, i.e. working with development teams to give them tools and processes to build quality into their features from the start.

<https://www.atlassian.com/inside-atlassian/qa>

Both Google and Facebook subscribe to a culture of developers testing their own code (well... unit testing). This post covers testing practices and code coverage at both companies, with references to their blogs and other internal sources. That includes a curious perspective from an ex-employee of FB as intentionally paying less attention to quality and focusing on other things instead, like making the company more "fun", because after all its social networking app is not critical to people.

<https://www.process.st/software-testing-methods/>

This has more details on testing and deployment process at Facebook circa 2012:

<https://www.quora.com/What-kind-of-automated-testing-does-Facebook-do>

<https://arstechnica.com/business/2012/04/exclusive-a-behind-the-scenes-look-at-facebook-release-engineering/2/>

To learn more about How Google Tests Software, you can read the eponymous book from 2012, or this series of Google Testing Blog posts in 7 parts from 2011, by the same author James Whittaker. They are not linked together, so I'm including each post here for easy reference.

How Google Tests Software - Part One (covers org structure):

<https://testing.googleblog.com/2011/01/how-google-tests-software.html>

How Google Tests Software - Part Two (roles of SWE, SET, and TE):

<https://testing.googleblog.com/2011/02/how-google-tests-software-part-two.html>

How Google Tests Software - Part Three (merging testing into development):

<https://testing.googleblog.com/2011/02/how-google-tests-software-part-three.html>

How Google Tests Software - Part Four (canary and beta deployments):

<https://testing.googleblog.com/2011/03/how-google-tests-software-part-four.html>

How Google Tests Software - Part Five (small/medium/large tests, automation vs manual):

<https://testing.googleblog.com/2011/03/how-google-tests-software-part-five.html>

How Google Tests Software - Part Six (The Life of an SET, Software Engineer in Test):

<https://testing.googleblog.com/2011/05/how-google-tests-software-part-six.html>

How Google Tests Software - Part Six (The Life of a TE, Test Engineer):

<https://testing.googleblog.com/2011/05/how-google-tests-software-part-seven.html>

Off-Topic
=========

In followup to the previous issue on Exploratory Testing:

<http://testersdigest.mehras.net/archive/testers_digest_2017_05_21.html>

I want to suggest a newer, better post by James Bach and Michael Bolton that traces the development of their ideas on exploratory testing and arrives at its 3.0 version where ALL testing is defined as exploratory.

<http://www.satisfice.com/blog/archives/1509>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
