TESTER'S DIGEST
===============
ISSUE #11 - Apr 16, 2017

---

We look at end-to-end testing, also known under the names of functional, integration, or application testing. The focus will be on automated regression tests, exploratory testing is its own subject. This time I'm referencing a couple of my own posts, a rarity.

Topic: End-to-end Testing
=========================

For clarity on what other kinds of testing there are, and where end-to-end testing fits in (named UI automation here):

<https://wolvesbaneacademy.xyz/2017/03/11/a-software-testing-process-for-the-team/>

What makes a good end-to-end test? From Google's Testing On The Toilet blog:

<https://testing.googleblog.com/2016/09/testing-on-toilet-what-makes-good-end.html>

A solid overview of User Acceptance Testing (UAT) which can be seen as a type of manual end-to-end testing, usually performed by the entire project team or by the business / product owner, representing the end user.

<https://www.simple-talk.com/dotnet/net-development/user-acceptance-testing-application-lifecycle/>

Product integration testing at Netflix. They test "High Impact Titles" (Netflix popular movies/shows) manually before launch, and via automated tests that validate assumptions after launch, with parallelization for multiple regions. QA work also covers A/B testing which made little sense until I saw an explanation in the comments section: the tests (formerly manual, now automated) verify that neither A nor B option is functionally broken.

<http://techblog.netflix.com/2016/07/product-integration-testing-at-speed-of-Netflix.html>

Shameless plug for my own slide deck comparing end-to-end testing via Selenium WebDriver UI automation vs a crowdsourced approach using RainforestQA platform:

<http://www.slideshare.net/KatieChin3/comparing-agile-aq-approaches-to-endtoend-testing-68145860>

And an overview of testing process at Quid (my employer) where I tried to name the right people / groups who should define tests at different levels. Our end-to-end test suite was built with active participation of Client Services and Product Management teams who best understand the product and user workflows.

<http://technology.quid.com/2016/08/its-not-the-stork-where-tests-come-from/>

Short, to-the-point post on picking the right level for test automation (UI vs API):

<https://www.techwell.com/techwell-insights/2017/02/where-begin-test-automation>

How data could be served to end-to-end tests: by creating it for the test run, querying prior to test execution, resetting for each run, or virtualizing.

<http://www.ontestautomation.com/managing-test-data-in-end-to-end-test-automation/>

Off-Topic
=========

Followup on GitLab's data loss incident we covered earlier, that talks about organizational change for even further transparency, including live streaming the incident response on YouTube as learning material for others in the industry,

<https://increment.com/on-call/the-benefits-of-transparency/>


---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
