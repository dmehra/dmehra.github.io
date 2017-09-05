---
title: "Tester's Digest #20: Tester's Role"
excerpt: Tester's Role. -- Let's take a look at the role a tester plays in an engineering organization. Yes, again; Tester's Digest issue #1 opened this subject with coverage of Google's SDET vs TE roles, and today we explore further.
---

TESTER'S DIGEST
===============
ISSUE #20 - June 18, 2017

---

Let's take a look at the role a tester plays in an engineering organization. Yes, again; Tester's Digest issue #1 opened this subject with coverage of Google's SDET vs TE roles, and today we explore further. For reference:

[Issue #1 - February 5, 2017]({{ site.baseurl }}{% post_url 2017-02-05-testers-digest-1-testers-role %}) // Topic: Tester's Role

Topic: Tester's Role
====================

An incendiary post with original title "Stop Hiring Testers" gathered a lot of comments, was updated by the author as the result of lively discussion with the community and renamed to "Stop hiring software checkers!". Its main point is that an agile team doesn't need special people to find bugs in the code, developers can do that, while quality engineers can take a broader look that includes "documentation, release management, processes, testing, etc."

<https://www.linkedin.com/pulse/stop-hiring-software-testers-janna-loeffler-mba-csm>

A slightly less divisive take by the author of "How We Test Software At Microsoft" book, who talks about two schools of testing: the old school of bug finding in a test phase of the development project, and the agile "quality assistance" school of feeding tester input into early project stages to inform developer testing, thinking a lot about customer experience, and having the entire team embrace a quality culture.

<http://angryweasel.com/blog/two-new-schools/>

How a tester can enhance an agile delivery team by acting as a "technical tester" (exploration and UI automation), "the tool smith" (building Page Objects, DSLs, other automation), and "the generalist":

<https://blog.gurock.com/advice-on-balancing-testers-for-embedded-scrum-teams/>

Thoughts on the role of developer vs test engineer, from an experienced practitioner who has worked in both capacities, having started out as a "code monkey" and evolved into an excellent quality engineer (as I can personally attest, since I know the author). Interesting take on the progression of software engineering from "Stone Age" through Medieval and Renaissance stages to the Modern Age.

<https://rlgomes.github.io/work/writings/rant/engineering/personal/2012/10/13/13.38-The-Origin-of-The-Modern-Software-Engineer.html>

A tester should act as information provider, not as quality police:

<https://www.stickyminds.com/article/dont-become-quality-police>

Beware of "roleism" such as viewing testers as second-class citizens compared to developers:

<https://theitriskmanager.wordpress.com/2014/12/27/introducing-roleism/>

Testers should not be afraid to step outside the classic boundaries of their role to fix small bugs and work with product code:

<http://www.kenst.com/2017/04/testers-dont-be-afraid-to-make-production-changes/>


Off-Topic
=========

Thoughts on creating test data, benefits and risks of using fake data vs real production / customer data (anonymized, of course):

<http://rightsaidjames.com/2017/05/improving-test-data/>

On the problem of tests getting slow, and what to do about it, namely: static sleeps of N seconds are evil; figure out the SLAs of your product and wait for conditions to become true or until the SLA has been exceeded; and elevate visibility of bottlenecks.

<https://testzius.wordpress.com/2017/05/04/tests-getting-slower/>


---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
