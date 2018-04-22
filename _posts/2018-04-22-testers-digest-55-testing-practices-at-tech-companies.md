---
title: "Tester's Digest #55: Testing Practices at Tech Companies"
excerpt: Who's doing what in the industry to keep quality up.
---

TESTER'S DIGEST
===============
ISSUE #55 - April 22, 2018

Let's see who is doing what in the industry to keep quality up. For our last look at the space of testing at tech companies a year ago, see this issue:

<http://testersdigest.mehras.net/2017/05/28/testers-digest-17-testing-practices-at-tech-companies.html>

Topic: Testing Practices at Tech Companies
==========================================

Approach to testing at these companies: Google, Facebook, Amazon, Spotify, Microsoft. They position differently on the "testing responsibility spectrum" and "testing importance spectrum".

<https://techbeacon.com/how-tech-giants-test-software-theres-no-one-way-qa>

Continous integration at Google: this slide deck is dense with information on their testing strategy (automation *only*), test coverage, flaky tests, regression test selection including new “Greenish” approach. The underlying research paper has more details.

<https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46593.pdf>

<https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45861.pdf>

A novel direction at Uber, brought about by their new CEO, is to follow the "Zero Defects" strategy. The article is heavier on Uber's travails and culture than on details, but I'm excited to see a technology leader advocate so strongly and publicly for quality.

<https://www.wired.com/story/uber-move-slow-test-things/>

Pair testing, session based testing, and bug scrubs / bug triages at Lucid:

<https://www.lucidchart.com/techblog/2017/08/15/how-to-defuse-a-bomb-wait-i-mean-a-bug-helpful-testing-methods-to-get-a-quality-product-out-faster/>

Risk reduction strategies at LaunchDarkly include pull requests with mandatory reviews, making small changes, using state machines to foresee risks, and canary launches. Interesting take on how Y2K didn't turn into a disaster (no, LD wasn't around back then... they are just making a point).

<http://blog.launchdarkly.com/what-makes-a-failure-a-disaster/>

What a typical day looks like for a tester at an online interior design company, including their tooling (JIRA, GitHub, Docker) and processes:

<https://www.kenst.com/2018/03/a-typical-day-of-testing-2018/>

Off-Topic
=========

Top takeaways from TISQA 2018 conference: TestAI shares what quality means for different products, and where AI fits in with test automation. Twitter decides what tests to automate based on risk, value, cost efficiency, and history of failures. Talks on API level testing over the more brittle UI tests, and consumer-driven contract testing.

<https://techbeacon.com/top-tisqa-takeaways-why-test-engineers-need-ai-more-qa-pros>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
