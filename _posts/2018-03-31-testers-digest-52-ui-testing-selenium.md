---
title: "Tester's Digest #52: UI Testing with Selenium"
excerpt: Selenium is a popular approach to UI-based testing, let's look at some ways of making it sane, starting with PageObject Model.
---

TESTER'S DIGEST
===============
ISSUE #52 - March 31, 2018

Digging further into web UI testing, we focus on Selenium as a popular approach. Let's look at some ways of making Selenium tests sane, starting with PageObject Model.

Topic: UI Testing with Selenium
===============================

The rest of resources here assume that you know what Selenium is, but in case you don't, here is a refreshing look at a tester's first experience with it:

<http://testingfuntime.blogspot.com/2014/12/selenium-adventures-how-to-automate.html>

Good old introduction to Page Object Model to create a layer of abstraction between your UI and the tests thereof:

<https://martinfowler.com/bliki/PageObject.html>

Using PageObject and PageFactory patterns with Selenium:

<https://www.toptal.com/selenium/test-automation-in-selenium-using-page-object-model-and-page-factory>

Using the Robot pattern which to me seemed like a glorified PageObject model. It is well presented with examples targeting Android based testing.

<https://news.realm.io/news/kau-jake-wharton-testing-robots/>

Argument for using data- attributes to locate UI elements in your tests, so they can be independent of CSS and class name changes in the front end code.

<https://blog.kentcdodds.com/making-your-ui-tests-resilient-to-change-d37a6ee37269>

How GitLab switched their UI tests from PhantomJS to headless Chrome with Selenium and ChromeDriver, covers differences between PhantomJS and Selenium in a lot of detail:

<https://about.gitlab.com/2017/12/19/moving-to-headless-chrome/>

How to set up your Visual Studio Code IDE for debugging of Selenium WebDriverIO (Node.js based) tests, with niceties such as breakpoints:

<http://blog.likewise.org/2017/02/debugging-a-javascript-webdriverio-project-in-vscode/>

People commonly advocate use of a BDD layer like Cucumber on top of your Selenium tests (and I had a good experience with that approach), but here is some well considered criticism, few years old yet still valid.

<https://www.jimmycuadra.com/posts/please-don-t-use-cucumber/>

Off-Topic
=========

Suitable for April 1st, or for any other day if you're bored of the regular "Lorem ipsum" text in UI mocks:

<http://meettheipsums.com/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
