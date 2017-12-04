---
title: "Tester's Digest #40: Testing Metrics"
excerpt: Measuring things matters, so let's talk about metrics for testing and quality.
---

TESTER'S DIGEST
===============
ISSUE #40 - December 3, 2017

"If you can't measure it, you can't improve it", as the management consultant Peter Drucker said. Or didn't. Murky story there. He might have said "What gets measured gets improved" which is... not the same. In any case, measuring things matters, so let's talk about metrics for testing and quality.

Topic: Testing Metrics
======================

Basic intro to test metrics:

<http://www.softwaretestinghelp.com/software-test-metrics-and-measurements/>

There is no single quality metric... if watching multiple ones, don't average them out, take the worst value.

<https://www.cqse.eu/en/blog/one-metric-to-rule-them-all/>

What is worth measuring on agile projects? Some specific answers here: Slack Time (that's built-in buffer in your plans, not time spent in Slack chat), Speed of Processes, Condition of Most-Edited Files, Escaped Defects, and Net Promoters Score (or more generally, a metric of who is happier as the result of your work).

<https://www.industriallogic.com/blog/what-should-we-measure/>

How to track test coverage in agile process: the practical recommendations include a low-tech dashboard that tracks 1-5 rating of how well tested each feature is, and sticky notes on the wall for risks.

<https://www.stickyminds.com/article/test-coverage-age-continuous-delivery>

How to know the value of your regression tests. This post doesn't go as far as suggesting metrics, but outlines an approach with SMART acronym: Specific, Measurable, Achievable, Relevant, Time; and advocates measuring coverage that your regression tests provide.

<https://www.stickyminds.com/article/get-smart-about-your-regression-tests-value>

A better way of tracking end-to-end test results than a simple pass/fail metric: automatically detect failures due to infrastructure or test setup issues and mark them as "blocked". The result is time savings on failure triage, and cleaner information for the team.

<https://blog.testproject.io/2017/06/14/generate-valuable-test-automation-reports/>

Off-Topic
=========

The Bug of the Week award goes to Apple for their security hole in macOS High Sierra that allowed passwordless root access. It's fixed now if you did "Security Update 2017-001".

<https://www.theinquirer.net/inquirer/news/3022100/apple-pushes-out-fix-for-devastating-macos-high-sierra-flaw>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
