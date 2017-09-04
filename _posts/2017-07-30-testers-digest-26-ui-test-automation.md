---
title: "Tester's Digest #26: UI Test Automation"
excerpt: UI Test Automation. -- Testing the UI of a web application, or testing the behavior of the application via the UI (different but often overlapping activities), increasingly calls for automation to catch regression bugs, and to keep with agile delivery schedules. We look at a few aspects of UI test automation in this issue.
---

TESTER'S DIGEST
===============
ISSUE #26 - July 30, 2017

---

Testing the UI of a web application, or testing the behavior of the application via the UI (different but often overlapping activities), increasingly calls for automation to catch regression bugs, and to keep with agile delivery schedules. We look at a few aspects of UI test automation in this issue.

Topic: UI Test Automation
===========================

What is reasonable in UI automation testing? This post covers the situation of regression testing a mature app, including valuable explanation of daily test maintenance activities.

<https://blog.gurock.com/reasonable-user-interface-ui-automation/>

Amusing Valentine's Day-themed post on UI-based test automation that makes serious points:

<https://www.joecolantonio.com/2017/02/14/2-ways-test-automation-can-break-heart/>

Why wouldn't you just use a record-and-replay framework (Selenium IDE or similar) to generate your UI tests, it's so much easier than designing page-object models and writing code, right? The answer is, they will break a lot, "because the information used to locate page elements keeps breaking". Read the 2016 study here:

<https://blog.acolyer.org/2016/05/30/why-do-recordreplay-tests-of-web-applications-break/>

Overview of end-to-end web testing frameworks for Javascript: CasperJS, Protractor, Nightwatch.js, TestCafe, CodeceptJS.

<https://medium.com/@adrian_lewis/top-5-most-rated-node-js-frameworks-for-end-to-end-web-testing-f8ebca4e5d44>

When is it worth testing via API (example uses Postman) rather than the UI?

<http://www.mwtestconsultancy.co.uk/data-driven-testing-gherkin-api/>

How to reason through selecting UI vs API testing approach:

<https://dev.to/eviltester/should-i-test-at-the-gui-level-or-the-api-level>

If end-to-end tests result in a slow and unreliable feedback loop for you, consider replacing them with contract based integration tests, with an example using Pact JS:

<https://devblog.xero.com/trust-but-verify-using-pact-for-contract-testing-495a1e303a6>

Mozilla post on cross browser compatibility, and a learning module on testing with SauceLabs and BrowserStack:

<https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Cross_browser_testing>

This is not specific to test automation, but a really good resource for any Web testing. It's actually a Web developer's checklist, but can double as a QA list of testing directions to consider:

<http://webdevchecklist.com/>


Off-Topic
=========

Things worth learning: How to read and understand a scientific paper: a guide for non-scientists, with a usage example.

<http://blogs.lse.ac.uk/impactofsocialsciences/2016/05/09/how-to-read-and-understand-a-scientific-paper-a-guide-for-non-scientists/>

<https://violentmetaphors.com/2013/09/08/an-example-of-how-to-read-a-vaccine-safety-study/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
