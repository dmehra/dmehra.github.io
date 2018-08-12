---
title: "Tester's Digest #69: Avoiding Bugs"
excerpt: Techniques to avoid entire categories of bugs when coding, including "the last line effect" and language-specific errors.
---

TESTER'S DIGEST
===============
ISSUE #69 - August 12, 2018

Testing is a valuable activity that reveals bugs, so that they can be fixed. Wouldn't it be better, though, if the bugs weren't there in the first place? There are some techniques to avoid coding the bugs in. Tell your dev friends!

Topic: Avoiding Bugs
====================

Learn about "The Last Line Effect": when copy/pasting blocks of code and making a change in each, it is the last block that will frequently contain a bug. Worth keeping in mind when acting as a peer code reviewer.

<https://www.viva64.com/en/b/0260/>

Google researchers look at the bugs in selecting arguments to a method call (in Java), conclude that probability of bugs increases markedly when methods have >5 arguments. They hence advise to keep the argument list at 5 or shorter, and to not reorder parameters in methods that are similar in meaning, or related through inheritance.

<https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46317.pdf>

Rollbar analyzed most common errors in web projects tracked by their service, and published a series of data-driven blog posts detailing those common bugs per language, with tips on preventing them! This is a pretty awesome resource.

Javascript:

<https://codeburst.io/top-10-javascript-errors-from-1000-projects-and-how-to-avoid-them-2956ce008437>

Ruby on Rails:

<https://rollbar.com/blog/top-10-ruby-on-rails-errors/>

PHP:

<https://rollbar.com/blog/top-php-errors/>

Website errors:

<https://rollbar.com/blog/top-100-websites-errors/>

For other languages (Python, C#, Java), see the Toptal posts referenced in our older TD issue:

<http://testersdigest.mehras.net/2018/04/15/testers-digest-54-dealing-with-bugs.html>

Not so immediately applicable (no open source tool available) but conceptually interesting: bugs tend to cluster around "architectural hotspots" which are specific files in the source code and/or inheritance hierarchies, dependency cycles, or unstable interfaces. If you can locate these hotspots in your codebase, any changes in those risky areas would deserve a more careful review.

<https://blog.acolyer.org/2016/06/09/design-rule-spaces-a-new-form-of-architectural-insight/>

<https://blog.acolyer.org/2016/06/10/hotspot-patterns-the-formal-definition-and-automatic-detection-of-architecture-smells/>

Even deeper into the weeds, consider the “naturalness” of buggy code: Just like true natural language, programming languages can be modeled using machine learning techniques (such as n-gram modeling) that will predict which sequences are "normal" vs "unusual". The unusual ones are likely to be buggy. With this tooling one could detect statistically improbable and yet syntactically correct lines of code and warn the developer of possible bugs. I only wish this was an open source project, not just a research paper...

<https://blog.acolyer.org/2016/06/08/on-the-naturalness-of-buggy-code/>


Off-Topic
=========

Story of a bug: video calls mysteriously drop after 1100 seconds… learn what ‘nonce’ means:

<https://medium.com/confrere/gone-in-1100-seconds-hunting-bugs-on-the-edge-of-webrtc-132a186c45dd>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
