---
title: "Tester's Digest #24: Static Code Analysis"
excerpt: Building Better Software -- Static Code Analysis. -- Testing doesn't put quality into software, it only shines the light on the good, bad and ugly that's already present therein. To build higher quality software, consider applying specific best practices at the stages of design and development. This issue looks at static code analysis.
---

TESTER'S DIGEST
===============
ISSUE #24 - July 16, 2017

---

Testing doesn't put quality into software, it only shines the light on the good, bad and ugly that's already present therein. To build higher quality software, consider applying specific best practices at the stages of design and development. This issue looks at static code analysis.

Topic: Static Code Analysis
===========================

Would static analysis tools help developers with code reviews? -- 2015 IEEE paper examines this question and suggests that developers remove 50-100% of certain types of issues that static analysis tools warn them about (in Java projects: warnings in the imports, regular expressions, and type resolution categories), but ignore others. The full paper needs IEEE subscription to access, but there is a slide deck covering it.

<http://ieeexplore.ieee.org/document/7081826/>

<https://www.slideshare.net/sebastianopanichella/saner2015-v2>

This post contrasts what static code analysis tools are good at with what human code review is good at. Static analysis shines at catching certain kinds of bugs such as memory corruption and leaks, buffer overflows, null pointers, infinite loops; and identifying maintainability problems such as too complex code. You still need humans to check the code's logic, and whether this code should have been written at all. "Tools can find cases of bad coding or bad typing – but not bad thinking."

<http://swreflections.blogspot.com/2014/09/can-static-analysis-replace-code-reviews.html>

Code review process followed by a development team at a financial services company (using Visual Studio tools) that includes looking at unit test coverage, code metrics such as maintainability index and cyclomatic complexity, and static code analysis to check for compliance with Microsoft rule set.

<https://stephenhaunts.com/2013/02/18/unit-test-coverage-code-metrics-and-static-code-analysis/>

A good list of mostly open-source static analysis tools, organized by programming language:

<https://github.com/mre/awesome-static-analysis>

Code clones... interesting concept that evaluates how much your code violates the DRY principle. Part 2 covers the tools for detection of code clones.

<https://www.cqse.eu/en/blog/practical-guide-to-code-clones-part1/>

Running static analysis on your code is not enough to enhance quality, you need a substantial manual action by quality engineers who will interpret the metrics and turn them into "actionable refactoring tasks" for developers. Based on a case study from Munich RE.

<https://www.cqse.eu/publications/2014-continuous-software-quality-control-in-practice.pdf>


Off-Topic
=========

Things worth learning: Develop an intuition for orders of magnitude in computer science / engineering

<https://blog.acolyer.org/2017/07/10/end-of-term-and-orders-of-magnitude/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
