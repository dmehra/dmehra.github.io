---
title: "Tester's Digest #51: Visual Testing"
excerpt: Visual testing - what it is (just pixel comparison of screenshots, really, but with a lot of gotchas), how to do it, choice of tools and service providers.
---

TESTER'S DIGEST
===============
ISSUE #51 - March 18, 2018

Continuing coverage of web UI testing, we focus on visual testing / validation: what it is (just pixel comparison of screenshots, really, but with a lot of gotchas), how to do it, choice of tools and service providers. This became a long issue as I kept digging into the topic. There appear to be two levels of visual testing, with one set of tools geared more toward end-to-end tests that run in staging environment (Applitools Eyes, Percy, Backtrac), and another targeting developers at unit test level (React Storybook, Jest image snapshots, etc).

Topic: Visual Testing
=====================

Distinction between functional testing of the UI and visual testing:

<https://saucelabs.com/blog/review-of-visual-vs-functional-testing-with-pdiff-and-applitools>

Why do visual testing, by Applitools but not specific to their product. It's the basic idea of recording screenshots from functional tests, doing automated image comparison with last round's screenshots, and serving up the changed ones to a human for validation.

<http://testautomation.applitools.com/post/152615349182/why-visual-testing-and-agile-are-a-perfect-fit>

<http://testautomation.applitools.com/post/153726980802/the-roi-of-visual-testing>

What's hard about diffing screenshots for visual regression testing? Post from another service provider who promises to do it better (Backtrac).

<https://backtrac.io/blog/creating-screenshot-what-can-go-wrong>

The third popular provider, Percy, writes about using their own product to validate a large scale restyling of their site.

<https://blog.percy.io/redesigning-with-confidence-d11799845ecb>

More detail on what it looks like to test with Applitools Eyes. This is written by their evangelist, using a Calculator app as an example:

<https://hackernoon.com/testing-your-frontend-code-part-v-visual-testing-935864cfb5c7>

This satisfied user of Applitools built a dynamic baseline by comparing staging and production versions of the app pages via Selenium tests. Their approach aims to solve the problem of needing to thumbs up/down on lots of changes to manually re-record the baseline.

<https://engineering.datorama.com/dynamic-visual-testing-at-scale-how-we-automate-testing-of-our-analytics-dashboards-db72e261ad75>

How developers can incorporate visual testing into Test Driven Development, with React Storybook. Tests run automated, output gets checked manually. The post doesn't cover how this would integrate into CI, perhaps with a manual build stage?..

<https://blog.hichroma.com/visual-test-driven-development-aec1c98bed87

Nice description of why you shouldn't compare complete screenshots of your website/app pages from someone who did it that way at first, then moved to component-level isolated screenshots, advocates BackstopJS.

<https://medium.com/@philgourley/making-visual-regression-useful-acfae27e5031>

Good analysis of what snapshot tests are good for, at unit test level (using Jest image snapshots):

<https://benmccormick.org/2016/09/19/testing-with-jest-snapshots-first-impressions/>

Reflection on how visual testing fits into the work process of a development team, including code review.

<https://engineering.klarna.com/improving-communication-and-confidence-with-visual-snapshot-testing-b04154c3aaf0>

Lists of (mostly free open source) visual validation tools:

<https://www.joecolantonio.com/2017/02/02/top-21-free-visual-validation-tools-testers/>

<https://github.com/mojoaxel/awesome-regression-testing/blob/master/README.md>

Off-Topic
=========

Worth learning: debug Javascript code with console tricks beyond console.log()

<https://medium.com/appsflyer/10-tips-for-javascript-debugging-like-a-pro-with-console-7140027eb5f6>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
