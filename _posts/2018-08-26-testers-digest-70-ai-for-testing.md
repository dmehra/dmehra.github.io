---
title: "Tester's Digest #70: AI For Testing"
excerpt: Look past the hype to practical uses of ML/AI in testing, its promise and limits.
---

TESTER'S DIGEST
===============
ISSUE #70 - August 26, 2018

Application of machine learning / artificial intelligence techniques to the field of software testing is a hot area these days. Let's try to look past the hype to specific practical uses of ML/AI in testing, and consider the promise and the limits of this approach.

Topic: AI For Testing
====================

Deep theoretical analysis of how ML could be used to develop testing tools that learn. The first post covers supervised/unsupervised vs reinforcement learning and its reward model. The second one goes deeper into Markov decision process as applied to a “gridworld” of features and bugs. The author illustrates (with Pac-Man example and working Python code) limitations and reasonable expectations of AI-based testing. Worth a read!

<http://testerstories.com/2018/06/framing-automation-based-ai/>

<http://testerstories.com/2018/08/can-an-ai-become-a-tester/>

Examples of practical applications of AI in visual testing by Applitools, using ML for test failure analysis at Dell, “spidering” tools like Mabl that auto-generate testcases after learning your app, and then run the tests by diffing their results from expected output which was learned (like Testim).

<https://www.joecolantonio.com/how-ai-is-changing-test-automation/>

<https://www.joecolantonio.com/7-innovative-ai-test-automation-tools-future-third-wave/>

Diffblue is an AI-based testcase generator that uses reinforcement learning and solver search techniques to make the ML system go beyond the training set of test examples, generalizing so it can produce new unit tests, given a codebase (only Java for now). Another AI-based tool, Security Risk Detection from Microsoft, uses constraint solving ML to increase test coverage through “whitebox fuzzing” of inputs.

<https://thenewstack.io/ai-machine-learning-can-help-test-code-faster/>

Newcomers like Test.AI promise AI-powered testing through the GUI that automatically identifies testcases for web page elements and user workflows, and can tolerate frontend changes. That’s a beautiful vision, let’s see if the well-funded startup can get there. Their older post (under Appdiff name) explains how they train ML to recognize app state labels from 300k labeled screenshots.

<https://techcrunch.com/2018/07/31/test-ai-nabs-11m-series-a-led-by-google-to-put-bots-to-work-testing-apps/>

<https://medium.com/ai-for-software-testing/ai-for-testing-identifying-app-state-92a8c89a0216>

Gaming company uses AI to proactively detect bugs as developers write code:

<http://www.wired.co.uk/article/ubisoft-commit-assist-ai>

Netflix uses data science technique of predictive modeling to locate content that’s more likely to be buggy (poor recording, audio/video mismatch, subtitle snafus) so it can be tested by humans:

<https://medium.com/netflix-techblog/optimizing-content-quality-control-at-netflix-with-predictive-modeling-712281658ab9>

Off-Topic
=========

My beloved crowdsourced testing service, RainforestQA, hasn't written a recent public post about the details of ML that is powering their framework; they have, however, written about the deficiencies in QA process on the Death Star.

<https://www.rainforestqa.com/blog/2018-06-19-bad-qa-killed-2-million-imperials-death-star-post-mortem/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
