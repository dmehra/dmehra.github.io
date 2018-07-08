---
title: "Tester's Digest #65: Testing ML Models"
excerpt: How does one test Machine Learning models?
---

TESTER'S DIGEST
===============
ISSUE #65 - July 8, 2018

How does one test Machine Learning (ML) models? We look at approaches to testing chatbots and DNNs for self-driving cars, checklists for ranking maturity of your ML, antipatterns to look out for, data science metrics for evaluating models, and compliance testing. Earlier Tester's Digests on the subject covered adversarial attacks and more:

<http://testersdigest.mehras.net/2017/11/05/testers-digest-37-test-machine-learning.html>

<http://testersdigest.mehras.net/2017/04/30/testers-digest-13-testing-data-science.html>

Topic: Testing ML Models
========================

How do you test a Deep Neural Network (DNN) which is the approach underlying modern self-driving cars? DeepTest system automatically generates test cases by applying image transformations to the seed set of road conditions images, and measures “neuron coverage” (a metric similar to code coverage but for DNNs) to make sure the additional test cases are improving overall coverage. It found thousands of erroneous behaviors in top-performing DNNs.

<https://blog.acolyer.org/2018/06/18/deeptest-automated-testing-of-deep-neural-network-driven-autonomous-cars/>

Tester shares guidelines for testing deep learning based chatbots:

<http://kavliwashere.com/testing-deep-learning-chatbots/>

Joel test for data science, a checklist way to gauge the maturity of your DS processes:

<https://blog.dominodatalab.com/joel-test-data-science/>

Essentially the same thing but with a lot more detail, from Google. They provide a list of 28 “specific tests” (checks) to assess production readiness of machine learning models. By ranking each category, you arrive at the ML Test Score at one of six levels from “more of a research project” to “exceptional levels of automated testing and monitoring”.

<https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46555.pdf>

Antipatterns in machine learning which lead to accumulation of technical debt:

<https://ai.google/research/pubs/pub43146>

These metrics are used by data scientists for evaluating ML models, and should be understood and utilized by testers as well. Part 1 covers regression metrics + BLEU score for NLP (mostly applied to machine translation), part 2 has classification metrics such as recall, precision, ROC-AUC etc.

<https://medium.com/usf-msds/choosing-the-right-metric-for-machine-learning-models-part-1-a99d7d7414e4>

<https://medium.com/usf-msds/choosing-the-right-metric-for-evaluating-machine-learning-models-part-2-86d5649a5428>

A common question posed to a QA team by data scientists is “can you help us determine if the new model is better than the old model?”. Here is an example of such evaluation for sentiment algorithms.

<https://blog.algorithmia.com/benchmarking-sentiment-analysis-algorithms/>

Privacy and compliance aspects of managing data science models and their input data - this discussion is framed as risk management and calls out organizational processes and roles (which in my mind fall under QA umbrella).

<https://www.oreilly.com/ideas/managing-risk-in-machine-learning-models>


Off-Topic
=========

How do you test product ideas? Good tips here on defining a hypothesis and tracking experiments. The second post on Hypothesis Driven Development directly compares product development to QA, ultimately defining it as a test of an idea, which I found pleasing.

<https://builttoadapt.io/7-tools-and-tips-for-tracking-your-experiments-74d20c1b1f0e>

<https://barryoreilly.com/2013/10/21/how-to-implement-hypothesis-driven-development/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
