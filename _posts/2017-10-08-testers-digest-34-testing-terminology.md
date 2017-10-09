---
title: "Tester's Digest #34: Testing Terminology"
excerpt: Today we dive into semantics of testing terminology -- what words we use, what we mean by them, and why that matters. A rose is a rose is a rose... isn't it? In the off-topic section, don't miss the STELLA Report.
---

TESTER'S DIGEST
===============
ISSUE #34 - October 8, 2017

Apologies for missing a week, Tester's Digest went to conference. Next issue will cover the highlights of StarWest 2017. Today we dive into semantics of testing terminology -- what words we use, what we mean by them, and why that matters. A rose is a rose is a rose... isn't it? In the off-topic section, don't miss the STELLA Report.

Topic: Testing Terminology
==========================

Oldie but goodie from Michael Bolton: we are in the business of "quality assistance" not "quality assurance", because how can you assure quality as a tester if you're not going to change the product source code to make it any better...

<http://www.developsense.com/blog/2010/05/testers-get-out-of-the-quality-assurance-business/>

Thoughts on replacing "QA" with a more suitable title. From the comments, I like "Software Detective" and "Quality Activist".

<https://medium.com/@Squidish_QA/exploring-testing-titles-in-agile-d720fef1da16#.ke9qbedkt>

Testing vs checking, by James Bach and Michael Bolton. "Checks" are another (better?) name for regression tests (and I suppose monitoring alerts as well), while "tests" refer to exploratory, experimental activities.

<http://www.satisfice.com/blog/archives/856>

Words matter, and what I mean by "test case" may not be what you mean:

<https://www.techwell.com/techwell-insights/2017/04/speaking-same-language-software-testing>

Why flexibility around word labels such as "bug" can help in getting things done:

<https://www.stickyminds.com/article/semantics-and-risk-labels-software-testing>

Should you call a bug a bug? Or a defect? Or a problem? Or an issue? Does it matter? As the Bard said, a rose by any other name would smell as sweet...

<http://www.developsense.com/blog/2014/04/ive-had-it-with-defects/>

Off-Topic
=========

Read of the week: the "STELLA report" by SNAFUcatchers, a group that includes Richard Cook of Ohio State University and focuses on "understanding and coping with the immense levels of complexity involved in the operation of critical digital services". At their workshop, extended by a day due to the Stella snowstorm, they analyzed software industry SNAFUs (near-outages), 3 of which are covered in the report: Apache, Travis CI, Logstash. It's not the technical specifics that matter, though; the report extracts commonalities and discusses possible improvements. I found the view of the system as "above line" (human cognition and mental model) and "below line" (software system, including monitoring tools) very valuable, and intend to dig into the concept of "dark debt" which was new to me.  

<https://drive.google.com/file/d/0B7kFkt5WxLeDTml5cTFsWXFCb1U/view>

Worth learning: memory management in Javascript, all the way from transistors and flip-flops to garbage collection to 4 common memory leaks to watch out for.

<https://blog.sessionstack.com/how-javascript-works-memory-management-how-to-handle-4-common-memory-leaks-3f28b94cfbec>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
