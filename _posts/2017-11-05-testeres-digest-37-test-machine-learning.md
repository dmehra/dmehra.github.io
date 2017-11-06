---
title: "Tester's Digest #37: How To Test Machine Learning"
excerpt: A new look at possible approaches to testing machine learning and other data science techniques.
---

TESTER'S DIGEST
===============
ISSUE #37 - November 5, 2017

A new look at possible approaches to testing machine learning and other data science techniques! We took a peek at testing data science a few months ago:

<http://testersdigest.mehras.net/2017/04/30/testers-digest-13-testing-data-science.html>

Since then, a few specific posts on testing for data scientists and test methodology for ML have appeared, which is very encouraging.

Topic: How To Test Machine Learning
===================================

Background for testers finding themselves in the brave new world of data science.

<http://www.datasciencecentral.com/profiles/blogs/40-techniques-used-by-data-scientists>

Examples of ML bugs here:

<https://blog.openai.com/openai-baselines-dqn/>

Fascinating angle at the quality of ML models (if you define quality as "can I break this?"). The adversarial approach is akin to "bad inputs" testing of regular software, only the test data is trickier to craft, and the results are much more far-reaching: a continuously learning model will produce wrong outputs for many other inputs once the "bad" data has been fed in.

<https://blog.acolyer.org/2017/09/13/adversarial-examples-for-evaluating-reading-comprehension-systems/>

DeepXplore testing method relies on having at least 3 neural networks for the same problem space so their solutions can be cross-checked against each other. The approach aims to maximize "neuron coverage" (similar to code coverage, a measure of network pathways that get activated during the test). It appears to be quite effective in finding bugs.

<https://spectrum.ieee.org/tech-talk/robotics/artificial-intelligence/better-bug-hunts-in-selfdriving-car-ai-could-save-lives>

DS meets hardware meets testing methodology: this team teaches a drone how to fly by letting it crash all over the place, rather than by training it on the "right" examples of flying.

<http://spectrum.ieee.org/automaton/robotics/drones/drone-uses-ai-and-11500-crashes-to-learn-how-to-fly>

If your company has a data science team, chances are, they can use an introduction to testing. Do not expect that DS folks understand the value of unit testing, have heard of TDD, and are armed with debugging skills. Quality engineers can make a tremendous difference by providing training and support to DS in this area. These posts will come in handy.

Quick slide deck on testing for data scientists, mentions three interesting projects: engarde, Hypothesis, and Feature Forge:

<http://slides.com/treycausey/pydata2015#/>

Deep, detailed slide deck on testing and debugging, targeted at data scientists who code in R:

<https://www.slideshare.net/ajayohri/software-testing-for-data-scientists>

TDD for data scientists, the post uses an example of testing a PySpark application:

<http://engineering.pivotal.io/post/test-driven-development-for-data-science/>

How to write unit tests when developing ML models:

<https://medium.com/@keeper6928/how-to-unit-test-machine-learning-code-57cf6fd81765>

Off-Topic
=========

Hilarious bug that happens if you ask Google Home "What is the temperature inside?"

<https://np.reddit.com/r/googlehome/comments/79vyg2/does_homemini_have_built_in_thermometers/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
