---
title: "Tester's Digest #58: Video Game Test Automation"
excerpt: The challenges of test automation for video games, and some solutions.
---

TESTER'S DIGEST
===============
ISSUE #58 - May 13, 2018

What skills befit a modern software tester? We examine domain expertise, data-driven testing, technical skills, DevOps skillset, UX aspect, and pair testing.

Topic: Video Game Test Automation
=================================

In the last issue we looked at QA at Nitro Nation; here is the sister post from their developers who are trying to do test automation, and the challenges they face. The post is over a year old, and I believe Unity made some progress with testing frameworks available for the engine.

<http://blog.filippkeks.com/2016/11/21/why-game-developers-are-afraid-of-test-automation.html>

Automated testing at Riot Games for League of Legends includes running 5500 tests on each build in CI, for a total of 100k tests a day. The tests are written in Python, based on RPC endpoints (similar to REST API testing for web apps). The post goes into detail on their Jenkins setup and examples of test code, good stuff.

<https://engineering.riotgames.com/news/automated-testing-league-legends>

A deep conversation on testing at EA (circa 2014, when they were working on Sports' FIFA 10 / 11). Covers the difficulty of testing online team play, EA's early failures at test automation, and steps they took to make tests more reliable. They moved toward MVVM architecture (Model - View - ViewModel) which allows to separate UI testing from gameplay testing, and considered introducing a DSL layer to simplify test development.

<https://queue.acm.org/detail.cfm?id=2627372>

This developer laments that he's not able to unit test his games, since the gameplay logic bugs are hard to catch in unit tests, and visual issues would be expensive to test for. A valuable comment thread discussing the difference between unit and integration tests, and a notion that unit tests only apply to the game engine.

<https://grumpygamer.com/unit_testing_games>

Another perspective from a developer who works on mobile games in C++ and writes unit tests, with specific examples of areas he covered in unit testing.

<http://www.gamasutra.com/blogs/FrancoisGuibert/20170612/299785/Unit_testing_in_video_games.php>

Interesting take on why game developers don't use TDD (Test Driven Development) approach, that calls out how game devs derive similar benefits by following other best practices: writing production usage code first, using assertions, and static compilation checks.

<http://chrismdp.com/2015/03/why-games-coders-dont-use-tdd-and-why-it-matters/>

Mobile game test automation is a separate beast, with the need to test and benchmark performance on a multitude of devices. This short post presents a possible automation framework based on Appium that utilizes Sikuli, Robot and Vysor:

<http://www.tothenew.com/blog/test-automation-approach-for-mobile-games/>

The setup can be made easier by using test automation platform as a service, such as the one by BitBar.

<https://bitbar.com/mobile-game-testing-and-test-automation-using-real-devices/>

Off-Topic
=========

Researchers use AI to play-test video games, the article is only skin deep, but the referenced paper is the real deal:

<https://motherboard.vice.com/en_us/article/538we3/researchers-are-building-ai-to-replace-video-game-testers>

<https://arxiv.org/pdf/1703.06275.pdf>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
