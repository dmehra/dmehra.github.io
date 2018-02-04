---
title: "Tester's Digest #46: Technical Debt"
excerpt: A new look at the problem of technical debt, its subtypes, measurement, and ways of paying it off.
---

TESTER'S DIGEST
===============
ISSUE #46 - February 4, 2018

It's been nearly a year since we last looked at technical debt, and the new content written about the issue has mounted along with the debt itself. This is our new look at the problem of technical debt, its subtypes, measurement, and ways of paying it off. The earlier take is available in Tester's Digest archive:

<http://testersdigest.mehras.net/2017/03/19/testers-digest-7-technical-debt.html>

Topic: Technical Debt
=====================

Kinds of technical debt, including defect debt, and some ideas for quantifying the costs of carrying such debt:

<https://blog.cloudymusings.com/a-lexicon-of-software-development-debt-6d88524f0a19>

Bug debt! "Unresolved bugs are like the undeliverable mail of our day—a one-way communication without a recipient."

<https://www.stickyminds.com/article/clean-your-bug-tracker-and-keep-numbers-manageable>

Feature flags are considered technical debt, for very good reasons:

<https://dzone.com/articles/feature-toggles-are-one-worst>

The big reason behind technical debt: we have systems with technical debt because those systems work -- that is, they appear to be working well enough, since the "working" part is visible, and the "debt" part is not.

<https://medium.com/@GeneHughson/dealing-with-technical-debt-like-we-mean-it-155a98a39f1c>

Why isn't anyone doing anything about the tech debt? Let's hope the situation at your workplace is not as dire as in this fictional bureaucracy:

<https://hackernoon.com/were-drowning-in-tech-debt-why-isn-t-anyone-listening-f4269cb5cc40>

PagerDuty on measuring technical debt with incident related data. While this is obviously tooting their own horn, the idea appears sound. "For example, if your MTTR for incidents related to a certain program is higher than your average MTTR, there’s a good chance the program in question is generating technical debt. Similarly, if servers running one type of operating system account for a disproportionate number of alerts, there’s probably a code or configuration flaw at play. That’s a technical debt you can address."

<https://www.pagerduty.com/blog/technical-debt/>

When taking on technical debt (on dev or test side), have a specific plan for how you will pay it off:

<https://testwithnishi.com/2017/09/07/paying-off-the-technical-debt-in-your-agile-projects/>

One approach to dipping into your technical debt... spin the wheel!

<https://goodenoughsoftware.net/2016/11/30/wheel-of-technical-debt/>

How LinkedIn paused new development for 2 months to pay off its tech debt in 2011 - light on detail, big on inspiration:

<https://www.linkedin.com/pulse/when-your-tech-debt-comes-due-kevin-scott/>

The system complexity angle on managing technical debt: have points of flexibility in the right places in your software (not everywhere), minimize dependencies, refactor for velocity, throw away prototype code and low-performing features, build culture of testing and code review.

<https://hackernoon.com/managing-technical-debt-1806424e7d40>

Off-Topic
=========

Worth learning: how to be a wizard. Well, that's the title anyway, but this slide deck from Stripe's engineer Julia Evans is amazing (take it from the person who hates slide decks). It covers the learning process of a future great engineer (or tester!)- what do you read? what do you try? how do you ask questions? how do you debug? how do you design? how do you develop understanding?

<https://www.slideshare.net/JuliaEvans8/so-you-want-to-be-a-wizard-73101468>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
