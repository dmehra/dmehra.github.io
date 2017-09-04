---
description: Building Better Software -- Unit Tests and TDD, Worth It? -- To continue the topic of building better software, this issue considers the question of whether it's worthwhile for developers to write unit tests, and use Test Driven Development approach.
---

TESTER'S DIGEST
===============
ISSUE #25 - July 24, 2017

---

To continue the topic of building better software, this issue considers the question of whether it's worthwhile for developers to write unit tests, and use Test Driven Development approach.

Topic: Unit Tests and TDD, Worth It?
====================================

Why should we write tests? This post, not limited to unit tests, lays out 5 factors: verify correctness; prevent regressions; document behavior; guide design; and support refactoring. I'm with the author.

<https://www.devmynd.com/blog/five-factor-testing/>

One software architect stops unit testing in his organization, lives happily ever after:

<https://techbeacon.com/1-unit-testing-best-practice-stop-doing-it>

Where did he get that crazy idea? The underlying incendiary papers are:

<http://rbcs-us.com/documents/Why-Most-Unit-Testing-is-Waste.pdf>

<http://rbcs-us.com/documents/Segue.pdf>

On the uselessness of Test-Driven Development if you don't employ the 3rd step of TDD, the refactoring step (remember, TDD is red-green-refactor). The author posits that a whole lot of people "do TDD" but skip refactoring, in which case they are carrying all the costs of TDD without reaping many of the benefits. If your TDD is like that, you're better off with #NoTDD. Don't miss the long comment thread that mostly suggests that you, eh, do TDD with refactoring...

<https://blogs.msdn.microsoft.com/ericgu/2017/06/22/notdd/>

Let's say you don't side with the no-unit-tests, no-TDD camp; here's a handy example of using TDD approach to Node.js unit tests using Mocha test runner, Chai assertions library, Sinon for stubs/mocks, with a promise to make you "a 5-dan test-master in theory":

<https://blog.risingstack.com/getting-node-js-testing-and-tdd-right-node-js-at-scale/>

How to write readable unit tests:

<http://www.uxebu.com/blog/2013/01/08/make-tests-read-like-a-book/>

Should you always shoot for 100% code coverage? Not if the unit tests will validate straightforward units of code at the expense of much test complexity, says this technical architect.

<http://labs.ig.com/code-coverage-100-percent-tragedy>


Off-Topic
=========

Things worth learning: This post lists out technologies/tools a developer should know. As a tester, you should, at a minimum, know *about* them.

<https://hackernoon.com/what-should-be-in-a-coders-toolbox-96674fc8fb74>

For a not-so-deep dive into one area, here is an overview of database technology landscape (SQL, NoSQL, time series DB, streaming DB):

<https://www.xaprb.com/blog/defining-moments-in-database-history/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
