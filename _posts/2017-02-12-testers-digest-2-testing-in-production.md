---
title: "Tester's Digest #2: Testing In Production"
excerpt: Testing In Production. -- What legitimate organizations mean when they say they test in prod.
---

TESTER'S DIGEST
===============
ISSUE #2 - Feb 12th, 2017

---

I try to focus on one main topic in each weekly issue of Tester's Digest,
with news sprinkled in.

Topic: Testing In Production
============================

For the related memes, head to Fun section; here we take a serious look at what
legitimate organizations mean when they say they test in prod.

If you're new to the TIP concept, start with some high-level advice from SauceLabs:

<https://saucelabs.com/blog/test-faster-and-smarter-by-testing-in-production>

And a bit more detail in this handy introductory post:

<http://www.awesome-testing.com/2016/09/testops-2-testing-in-production.html>

Tests in production can be risky. How do you run a cost/benefit analysis to decide
whether it's worth the risk? How do you then lower the risk? Thoughts from
TurbineLabs based on Twitter's testing experience:

<https://medium.com/turbine-labs/every-release-is-a-production-test-b31d80f2bc74#.bmmlogxt1>

From Twitter itself, a description of their failure injection testing in prod:

<https://blog.twitter.com/2015/how-we-break-things-at-twitter-failure-testing>

Netflix largely tests in production, also with fault injection. The impact on end users is
"member pain" when they happen to be in the path of a failure test; Netflix aims
to minimize the pain, but considers it acceptable for a small percentage of users.
So next time when your show won't play, consider that it might be not due to your
modem or even a bug, but the result of an intentional test!

<http://techblog.netflix.com/2016/01/automated-failure-testing.html>

If you want to avoid "member pain" and serve the known correct output to your users,
while simultaneously sending production requests down the new path, so you can
compare outputs of old ("control") vs new ("experiment") and alert yourself on mismatch,
try GitHub's Scientist. The framework is a year old now and ported to multiple languages.

<https://githubengineering.com/scientist/>

Here is an example of GitHub using Scientist to find/fix issues in their merge code:

<https://githubengineering.com/move-fast/>

This recent post from The Guardian describes their production testing system which
triggers post-commit tests in prod and shows results as a badge on the GitHub pull request.
The prod tests cheat a bit by targeting the production deployment of the app, but
against a staging backend with test accounts.

<https://www.theguardian.com/info/developer-blog/2016/dec/20/testing-in-production-rethinking-the-conventional-deployment-pipeline>

Salesforce advocates regular re-runs of tests in production, via their Gearset automation:

<https://gearset.com/blog/salesforce-testing-best-practice-why-you-should-regularly-run-production-tests>

On usability testing in production, from LaunchDarkly (with a pitch to use their feature flag offering, of course):

<http://blog.launchdarkly.com/running-usability-tests-in-production/>


News
====

GitLab's well-considered postmortem analysis of their database incident of Jan 31:

<https://about.gitlab.com/2017/02/10/postmortem-of-database-outage-of-january-31/>

If you missed it while it was happening, here is the play-by-play of the incident itself, worth reading before the postmortem:

<https://about.gitlab.com/2017/02/01/gitlab-dot-com-database-incident/>

Fun
===

For "Testing In Production" memes, head straight to Google Images:

<https://www.google.com/search?q=testing+in+production+meme&tbm=isch>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
