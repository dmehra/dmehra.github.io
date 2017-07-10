---
description: Building Better Software -- Code Review. -- Testing doesn't put quality into software, it only shines the light on the good, bad and ugly that's already present therein. To build higher quality software, consider applying specific best practices at the stages of design and development. This issue looks at code review.
---

TESTER'S DIGEST
===============
ISSUE #23 - July 9, 2017

---

Testing doesn't put quality into software, it only shines the light on the good, bad and ugly that's already present therein. To build higher quality software, consider applying specific best practices at the stages of design and development. This issue looks at code review. We will get to static code analysis next week.

Topic: Code Review
==================

Praise for code review as a process from two different ex-Googlers, written in 2011 and 2016:

<http://goodmath.scientopia.org/2011/07/06/things-everyone-should-do-code-review/>

<https://blog.fullstory.com/what-we-learned-from-google-code-reviews-arent-just-for-catching-bugs-b125a13aa292>

A lighthearted take on the wrong ways to do code review, both as the reviewer, and the author of the code up for review:

<https://rjzaworski.com/2016/06/how-to-ruin-code-review>

Advice on improving code review practices from Asana (team collaboration SaaS). I liked the step where reviewer runs the app from the branch under review to help them understand what the change does, and possibly find bugs.

<https://blog.asana.com/2016/12/7-ways-to-uplevel-your-code-review-skills/>

Code review practices at Atlassian (circa 2010): it's not a bug hunt, and it's not a blame game. They regard code review as an embodiment of the 1st principle of the Agile Manifesto: "Individuals and interactions over processes and tools", and see improved code quality as a nice side effect.

<https://www.atlassian.com/blog/archives/code_review_in_agile_teams_part_i>

<https://www.atlassian.com/blog/archives/code_review_in_agile_teams_part_ii>

<https://www.atlassian.com/agile/code-reviews>

This post opens with a code review template used at Server Density (monitoring SaaS provider) and touches on the testing aspect, both unit tests and manual testing of a pull request.

<https://blog.serverdensity.com/how-to-do-code-reviews/>

Description of Spotify's 2-pass code review:

<https://medium.com/@mrjoelkemp/giving-better-code-reviews-16109e0fdd36>

If you're hungry for more articles on the subject, this is a 161-page PDF with a Cisco case study and lots more "Best Kept Secrets of Peer Code Review":

<https://smartbear.com/SmartBear/media/pdfs/best-kept-secrets-of-peer-code-review.pdf>


Off-Topic
=========

Things worth learning: How innovations are born, with the background on statistical underpinning of, well, everything:

<https://blog.acolyer.org/2017/02/03/dynamics-on-emerging-spaces-modeling-the-emergence-of-novelties/>

The above touches on Benford's law, which is worth a more detailed read. The law states that in many data sets, values start with 1 about 30% of the time, while <5% of the values start with 9, instead of the about 11% you'd expect from uniform distribution. This is not a joke but very real albeit surprising math.

<http://people.math.gatech.edu/~hill/ARTICLES/The%20Power%20of%20One.pdf>

Back to innovations, for a taste of the software I work on, check out Quid's network representation of news and companies data, where articles with similar language are combined into clusters, and nodes bridging two clusters reveal innovative ideas and businesses.

<https://quid.com/feed/why-do-bridging-nodes-matter-they-connect-ideas>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
