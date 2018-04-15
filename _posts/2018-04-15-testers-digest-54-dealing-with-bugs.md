---
title: "Tester's Digest #54: Dealing With Bugs"
excerpt: Bugs happen. How do you respond? Also, overview of common bugs in different languages.
---

TESTER'S DIGEST
===============
ISSUE #54 - April 15, 2018

Bugs happen. How do you respond? Some thoughts on blameless approach applied to finding / not finding and fixing / not fixing bugs.

Topic: Dealing With Bugs
=========================

How to organize "Bug Hunts", more commonly known as bug bashes:

<http://qablog.practitest.com/what-do-you-pack-when-you-go-for-a-bug-hunts/>

What is a test team to do when they missed a bug? Good application of the blameless approach here:

<https://dragonqa.blog/2018/03/29/tester-horror-story-omission/>

To fix or not to fix, that is the question. Interesting blameless analysis of how to respond to outages, do you improve the system or leave it as is?

<https://www.xaprb.com/blog/schrodingers-outage/>

A particular situation when a bug should not be fixed: sometimes the user needs a way to put the system into an invalid state while recovering from a much worse invalid state.

<https://ayende.com/blog/180993/when-letting-the-user-put-the-system-into-an-invalid-state-is-a-desirable-property>

Fun split brain scenario bug:

<https://ayende.com/blog/181441-C/production-test-run-the-self-flagellating-server>

Common bugs, by language: Java, Python, C#, Javascript, Rails, PHP, and general web development. Pick your poison. (Testing folks, if you choose to go talk to your developer peers about these buggy patterns, keep in mind the blameless approach... not "You're screwing up here in such a basic way, there's a Top 10 post on the internet about people like you")

<https://www.toptal.com/java/top-10-most-common-java-development-mistakes>

<https://www.toptal.com/python/top-10-mistakes-that-python-programmers-make>

<https://www.toptal.com/c-sharp/top-10-mistakes-that-c-sharp-programmers-make>

<https://www.toptal.com/javascript/10-most-common-javascript-mistakes>

<https://www.toptal.com/ruby-on-rails/top-10-mistakes-that-rails-programmers-make>

<https://www.toptal.com/php/10-most-common-mistakes-php-programmers-make>

<https://www.toptal.com/web/top-10-mistakes-that-web-developers-make>

Off-Topic
=========

Floating point precision bugs, they will be a thing in any language you work with! This post targets Javascript where "0.1 + 0.2 === 0.3" is false (try it...), but the explanation applies to any other common programming language.

<https://modernweb.com/what-every-javascript-developer-should-know-about-floating-points/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
