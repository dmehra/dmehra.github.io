---
title: "Tester's Digest #40: Test Automation"
excerpt: This issue on test automation covers automated regression tests, including UI test automation, including codeless UI test automation.
---

TESTER'S DIGEST
===============
ISSUE #41 - December 11, 2017

Test automation gets discussed so much that here's a full issue's worth since we last covered the topic in July. We cover automated regression tests, including UI test automation, including codeless UI test automation. Dear reader, please tell me that what you do with flaky tests is not "automatically rerun them"... but we cover that approach as well.

Topic: Test Automation
======================

Advice from industry practitioners (including yours truly) on QA automation, here's tl;dr. Do: gain buy-in from developers; utilize customer usage data; communicate expectations. Don't: focus on maximizing the number of test cases; miss low hanging fruit while chasing "all-the-things" automation; create technical debt in the form of unreliable tests.

<https://www.rainforestqa.com/blog/2017-12-07-the-dos-and-donts-of-revamping-your-qa-strategy/>

The place of automation in one's regression testing strategy:

<https://dojo.ministryoftesting.com/lessons/how-to-do-good-regression-testing>

Succinct post on the value of automated regression testing, what it can and cannot do for you, and a tl;dr of "there is no way around test automation, unless you want your users to find your bugs for you."

<https://medium.com/@roesslerj/why-there-is-no-way-around-test-automation-except-one-9c51aefd7806>

Should automated regression tests be finding bugs? This team looked back at their apparent success in building a regression suite that regularly finds bugs, and concluded that it wasn't all good news and "the holes are too big in the early stages".

<https://offbeattesting.com/2017/06/08/should-automation-find-bugs/>

Benefits and drawbacks of UI test automation:

<https://inviqa.com/blog/overview-frontend-automated-testing>

A most useful tip on how to approach test automation: address the infrastructure first, make sure a simple test runs in CI, resolve your data management issues. Then proceed to code up the testcases.

<http://www.ontestautomation.com/tackle-the-hard-problems-first/>

Controversial approach - or at least one I do not advocate taking - but here it is: if you have flaky automated tests and cannot (will not?) invest in fixing them, Spock framework provides automatic reruns on failure. "Still better than false-positive tests", says the post author.

<https://testdetective.com/rerun-flaky-tests-spock-retry/>

Codeless automation (for end-to-end / UI based tests), is that a thing? Supposing it even worked reliably, consider the author's points: "What is hard is writing good, readable, maintainable code. Structuring your tests. Testing the right thing at the right level. Creating a solid test data and test environment strategy. Those things are hard. And codeless test automation does nothing for those problems."

<https://www.ontestautomation.com/why-theres-no-such-thing-as-codeless-automation/>

Off-Topic
=========

The Bug of the Week award goes to Ai.Type mobile keyboard app, which leaked 31M customer records through a misconfigured MongoDB database. Or rather, configured with defaults. Which are "open to the world". Know your Mongo...

<https://mackeepersecurity.com/post/virtual-keyboard-developer-leaked-31-million-of-client-records>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
