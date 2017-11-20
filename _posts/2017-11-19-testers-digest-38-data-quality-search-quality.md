---
title: "Tester's Digest #38: Data Quality and Search Quality"
excerpt: Data quality is an area that presents interesting testing challenges. Search quality often overlaps with data quality (garbage in, garbage out) so we look at both.
---

TESTER'S DIGEST
===============
ISSUE #38 - November 19, 2017

Data quality is an area that presents interesting testing challenges. Search quality often overlaps with data quality (in that "garbage in, garbage out" manner) so we look at both.

Topic: Data Quality and Search Quality
======================================

"Data is never done", that is, data management needs to be treated as an ongoing task:

<https://www.coelevate.com/essays/growth-data-mistakes>

This short post on testing validity of data links to a free O'Reilly e-book report that presents a case study from Spiceworks with details on testing and improving data integrity:

<https://www.oreilly.com/ideas/a-guide-to-improving-data-integrity>

How Yelp tested their data quality to compare with competition: they pulled a sampling of businesses from "Best Of" lists, manually went through 1000 of them on Yelp and competitor sites, and assigned points for correctness.

<https://engineeringblog.yelp.com/2013/11/data-quality-how-yelp-stacks-up-to-the-competition.html>

Crossing over from data quality to search quality, start with this long read on how search works. Comes with a beautiful illustration of a production data indexing pipeline as a Rube Goldberg machine. Has a section on search quality that starts with a call to define what quality means to you, then lists classical metrics like precision, recall, F1 score, and types of human evaluation.

<https://medium.com/startup-grind/what-every-software-engineer-should-know-about-search-27d1df99f80d>

Netflix open sourced its query testing framework which helps tune precision and recall of queries against short text fields (such as movie titles) in multiple languages. The framework uses Google spreadsheets where testers specify queries and track results.

<http://techblog.netflix.com/2016/07/global-languages-support-at-netflix.html>

Also by Netflix, an attempt to tackle data quality: Netflix sources subtitles in >20 languages for its original English language content. As a first step in taking control of translation quality, they launched a test for the subtitle professionals called HERMES, and tag their work with an individual H-number. The stated goal is to be able to recommend translators for specific work by genre. Amusingly, there is a long thread of comments about invalid H-number errors... more testing needed?

<http://techblog.netflix.com/2017/03/the-netflix-hermes-test-quality.html>

Google's steps to remove inappropriate search results:

<https://blog.google/products/search/our-latest-quality-improvements-search/>

Facebook's steps to address fake news problem:

<https://newsroom.fb.com/news/2017/04/working-to-stop-misinformation-and-false-news/>

Off-Topic
=========

Bug of the week: flaw in Amazon Key can let rogue delivery agents disable the door camera in an untraceable way (fix coming).

<https://www.wired.com/story/amazon-key-flaw-let-deliverymen-disable-your-camera/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
