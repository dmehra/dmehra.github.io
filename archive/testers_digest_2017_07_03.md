---
description: Building Better Software. -- Testing doesn't put quality into software, it only shines the light on the good, bad and ugly that's already present in it. To build higher quality software, consider applying specific best practices at the stages of design and development.
---

TESTER'S DIGEST
===============
ISSUE #22 - July 3, 2017

---

Testing doesn't put quality into software, it only shines the light on the good, bad and ugly that's already present in it. To build higher quality software, consider applying specific best practices at the stages of design and development.

Topic: Building Better Software
===============================

These lessons in software systems development are a great followup to "Notes on distributed systems for young bloods" that we referenced in 02/20/17 digest. The author covers end-to-end argument in systems design, concentrating complexity inside components to hide it from consumers, recognizing asynchronous nature of systems and expecting failures, performance improvements (bandwidth leads, latency trails), and even designing organizations that build better software - it's all about feedback loops!

<https://hackernoon.com/education-of-a-programmer-aaecf2d35312>

How to build for high availability (and whether the nines are worth it):

<http://blog.statuspage.io/high-availability>

Google maintains a "Code Health" group (composed of the 20%-choice-time contributors) who work out recommendations for things like code review, best coding practices, and sometimes get involved in refactoring, tooling and libraries that can benefit many developer groups at the company.

<https://testing.googleblog.com/2017/04/code-health-googles-internal-code.html>

Here's a practical tip from Google: reduce nesting to reduce complexity and bugginess of your code.

<https://testing.googleblog.com/2017/06/code-health-reduce-nesting-reduce.html>

More programming habits to avoid, so you end up with better code:

<https://techbeacon.com/35-bad-programming-habits-make-your-code-smell>

What can developers do to learn failure modes of their software, what bugs are important to fix, what is worth monitoring and logging, and how to design for reliability? Go on call! The experience of first-line support informs better software development.

<https://jvns.ca/blog/2017/06/18/operate-your-software/>

Working in support will similarly broaden a tester's perspective: "Ask your boss to put you in support for few weeks. You will see what going on there".

<http://thebrokentest.com/what-tester-can-learn-in-supprot/>

Another aspect of better software development is code review and static analysis tools. Static analysis can help identify bad/ugly code and find bugs. It's a large enough topic that we will pick it up in the next issue.


Off-Topic
=========

Things worth learning: Paradoxes of probability

<http://quillette.com/2017/05/26/paradoxes-probability-statistical-strangeness/>

When can you trust statistics? On p-values and spurious correlations:

<https://blog.acolyer.org/2017/01/25/toward-sustainable-insights-or-why-polygamy-is-bad-for-you/>


---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
