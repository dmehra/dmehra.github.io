---
title: "Tester's Digest #42: Mutation Testing"
excerpt: You use tests to make your code better. You use mutation testing to make your tests better.
---

TESTER'S DIGEST
===============
ISSUE #42 - December 17, 2017

You use tests to make your code better. You use mutation testing to make your tests better.

Topic: Mutation Testing
=======================

What is mutation testing: the basic idea is to inject bugs into your source code to establish whether your unit tests would find them, with the purpose of then adding the missing tests.

<https://blog.codecentric.de/en/2016/01/mutation-testing-watching-watchmen/>

How to pick the right mutants to destroy in your code by adding only the useful missing tests:

<https://blog.codecentric.de/en/2016/02/sensible-mutation-testing-dont-go-killing-spree-2/>

Neither 100% coverage, nor 100% mutation coverage are a silver bullet against bugs. However, mutation testing clearly shows out pieces of code which need refactoring, and causes you to write more asserts and construct more detailed tests.

<http://atodorov.org/blog/2016/12/27/mutation-testing-vs-coverage/>

How mutation testing fits with agile process: use pairing, apply MT pragmatically to avoid shift from the useful mentality of "Did you think of this corner case?" to the much less useful "These 3% of expressions/mutants are not covered", and use MT as a tool to promote refactoring in the Red-Green-Refactor cycle of TDD.

<https://www.sep.com/sep-blog/2015/07/14/mutation-testing-totally-a-thing/>

A neat story of debugging a Rails issue, found via mutation testing:

<https://blog.arkency.com/constructor-for-a-included-module-in-ruby/>

This is the list of current MT tools I'm aware of.

Mutation testing in Java with PIT:

<http://pitest.org/>

Mutation testing in Python with Cosmic Ray or Mutmut:

<http://cosmic-ray.readthedocs.io/en/latest/>

<https://hackernoon.com/mutmut-a-python-mutation-testing-system-9b9639356c78>

Mutation testing in Javascript with Stryker:

<https://stryker-mutator.github.io/>

Mutation testing in Ruby with Mutant or Mutest:

<http://blog.arkency.com/2015/06/how-good-are-your-ruby-tests-testing-your-tests-with-mutant/>

<https://blog.cognitohq.com/how-to-write-better-code-using-mutation-testing/>

How Mutant gem works in Ruby, in much detail, for those interested in the technical underpinnings:

<https://troessner.svbtle.com/kill-all-the-mutants-a-deep-dive-into-mutation-testing-and-how-the-mutant-gem-works>


Off-Topic
=========

Worth learning: what happens when you press "play" on Netflix, from "what's a CDN" to how machine learning fits in.

<http://highscalability.com/blog/2017/12/11/netflix-what-happens-when-you-press-play.html>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
