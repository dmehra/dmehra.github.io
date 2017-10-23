---
title: "Tester's Digest #35: StarWest 2017 Highlights"
excerpt: Tester's Digest went to StarWest 2017 testing conference! Unusually wordy issue highlighting ideas we liked.
---

TESTER'S DIGEST
===============
ISSUE #35 - October 22, 2017

Tester's Digest went to StarWest 2017 testing conference! Unusually wordy issue highlighting ideas we liked. The slide decks are not publicly posted (other than mine!), I link to the related posts where possible. To view the keynote talk videos, you can do a free signup here:

<https://vts.inxpo.com/Launch/QReg.htm?ShowKey=42256&AffiliateData=SWV17HomeTopRegButton>

Topic: StarWest 2017 Highlights
===============================

## AI is coming to take our jobs... not

A subset of talks, including not one but two keynotes, covered the future of QA in the world of AI / ML that we have entered. It was clearly an area of interest but without much specifics so far. The speakers highlighted two sides of the issue:

* what new tools are coming testers' way from the machine learning direction
* and will they supplant human testers?! perish the thought!
* and how do we intend to test the AIs (manually through our human acumen?...)

Jason Arvin and Tariq King are notable names in the space. Their new association AIST "Artificial Intelligence for Software Testing" could be worth joining,

<https://www.aitesting.org/>

More on AIST from Tariq:

<https://medium.com/ai-for-software-testing/getting-started-with-ai-for-testing-571f88dff3c9>

## Continuous testing metrics

One keynote talk touched on lots of devops-flavored things that we have in spades at my workplace (Quid Inc.) such as CI, automated tests, metrics, production monitoring:

<https://www.sealights.io/blog/testing-and-devops-star-west-2017-keynote/>

The one thing from the talk that we don't have is a velocity dashboard that shows time from first commit (or better yet, from JIRA ticket or even product idea / feature request) to when it's deployed in production. Averages computed over N weeks indicate whether our velocity is getting better. We are so building that at Quid.

Another worthwhile view, offered by a for-pay provider in the expo hall (CD Director), gives a swimlane-style visualization of builds progressing through deployment and testing stages, reminiscent of a Trello board. If someone knows of a DIY open source equivalent, please point me at it, otherwise we might be building this one too.

<https://blog.cddirector.io/https-medium-com-cddirector-nomorespreadsheets-welcome-to-cddirector-io-release-management-tool-2bda4caa4ddf>

Another commercial provider (Sealights) promises code coverage at any level, including for end-to-end tests, with "quality risks" called out if new build includes lines of code with no coverage by any level of tests. Intriguing. They have this neat writeup on quality metrics:

<https://www.sealights.io/test-metrics/>

## Service Virtualization is worthwhile

It's particularly handy for people who are relying on lots of legacy services but would like to test without actually using those legacy services. For homegrown microservices, service virtualization has merits too:

* Lets you test things before they exist
* Allows you to reduce infrastructure costs
* Lets you test how your service behaves when a different service is broken

## API level tests are necessary

You should test the Restful APIs before you test the GUI, not only does it exist first, it has to work before the gui will work anyway, so you should test it first. Sounds obvious, doesn't it? But do you actually do it?

Sitting at the API level is hugely powerful for testing workflows, you just do one thing after another, without complication of linking up with ever-changing UIs. You could tie together api based testing and web driven testing to go capture screenshots.

Also, Swagger is a self-proclaimed "WORLD'S MOST POPULAR API TOOLING" for development and testing.

<https://swagger.io/>

## How to get your Selenium tests to stability

 This was a really great talk by Craig Schwarzwald, here's a slide deck (from SauceCON but same topic), and the main points are listed below because they are just so good.

 <https://www.slideshare.net/saucelabs/saucecon-2017-selenium-say-goodbye-to-the-f-word-flaky-no-more>

* Avoid timing issues: Don't Hard Wait, just don't. Don't implicit wait, just don't. Poll for things (and put those polls in your page objects).
* Write Good Selectors: unique, unlikely to change, descriptive.
* Make sure your page object model has a base page object: Wrap selenium core commands (logging, error handling in one place). Use common functions (find text in table).
* Tests only call page objects and assert: Page objects never assert. Tests never refer to locators. Neither ever calls selenium commands directly
* Page Objects: Composition over Inheritance. Use class instances, not library page object.

All this assumes, of course, that your Selenium tests are written with a Page Object Model. If not, start there.

## Is crowdsourcing an alternative to Selenium for end-to-end tests

This was my talk, and the empirical answer is yes, since I've been crowdsourcing my end-to-end regression tests via RainforestQA platform for a year and a half now. Here is a writeup and slide deck:

<https://www.techwell.com/techwell-insights/2017/09/use-crowdsourcing-shortcut-ui-test-automation-journey>

<https://www.slideshare.net/secret/LUGWo4W1ZXy0nL>

## Model-based testing is a thing

You can define a model of your app (user workflows) using a tool like GraphWalker and yED graph editor. Then you hook up a page object model to that, and it auto generates Selenium testcases for you. If you pick a subset rather than telling to cover 100% of the graph edges, you end up with a randomized navigation through the app. This is definitely for teams with advanced testing level, but good to know it exists, and Python tools are available.

<https://github.com/FTSRG/swsv-labs/wiki/5-Model-based-test-generators>

<http://mit.bme.hu/~micskeiz/pages/mbt.html>

## Shift-left means testing requirements

"Shift-left" is a buzzword in QA these days. It usually means having the testers plug into development process early, rather than testing completed product waterfall-style, something like this:

* QA participates with Product/UX at the requirements and design stage
* QA helps the agile team include testing in the definition of "done"
* QA reviews the acceptance criteria for ambiguity and misses
* QA brainstorms with Dev to arrive at a test plan together, rather than producing one for the team

One QA team's definition of its role gave me a kick, it was "SHAT" (as in the past tense...): Show, Help, Advocate, Test.

## How to run a workshop, or WREST was best

One session we thoroughly enjoyed and learned a lot from was the "Workshop on Regulated Software Testing", i.e. testing of products/services regulated by the FDA or other controlling body. Participants presented their "experience story" and others chimed in with their comments, questions, or new threads of conversation. We got to learn how hospital-grade infusion pumps are tested (you'll sleep better if you don't know), and the operating procedures for an electrical grid (don't ask). It wasn't all horror stories, though; hearing about the setup of the development and testing processes at other companies was supremely useful, and the exchange of ideas with other practitioners felt cathartic.

## More conference

At StarWest we learned of this other conference called CAST, which has a more technical bent. CAST 2017 already happened, will be on the lookout for August 2018.

<https://www.associationforsoftwaretesting.org/conference/cast-2017/>

Off-Topic
=========

Nothing today due to an already huge issue. But if you have time to kill, make paperclips.

<http://www.decisionproblem.com/paperclips/index2.html>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
