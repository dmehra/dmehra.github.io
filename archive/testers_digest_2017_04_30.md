TESTER'S DIGEST
===============
ISSUE #13 - Apr 30, 2017

---

Today we look at how (and why) we should test software relying on Data Science. If you know of more resources than what's in this newsletter, please send them my way. In a bit of topic reversal, I present *using* DS concepts for testing in Off-Topic section.

Topic: Testing Data Science
===========================

We are not going to dig into today's topic. We are not even scratching the surface. It's more like drawing with your finger on a fogged up mirror. That is because the question of how to test anything related to Data Science (ML, AI, DL, you name it) is barely beginning to get asked. Take it from Satya Nadella who, after Microsoft's Tay AI bot disaster, had only this to say:

"it was a great call to even get more grounded in the design principles we talked about, having stronger algorithmic accountability, what does QA mean? What does Quality Assurance mean?"

Good question. Here is the source but you won't find any answers there...

<https://qz.com/792554/microsoft-msft-ceo-satya-nadella-on-artificial-intelligence-algorithmic-accountability-and-what-he-learned-from-tay/>

I see the youth of data science as an engineering field as the reason. It is today as software development overall was in 1960s, per Donald Knuth:

"computer programming was so badly understood that hardly anyone even thought about proving programs correct; we just fiddled with a program until we 'knew' it worked."

<https://blog.acolyer.org/2016/09/08/computer-programming-as-an-art/>

First off, an introduction: what can data science do for you? This post lists out the kinds of questions (with business/user value) which are answerable with DS solutions, and the statistical approaches and tools DS uses to come up with answers. It's all math underneath, you know.

<https://medium.com/towards-data-science/how-to-ask-questions-data-science-can-solve-e073d6a06236>

A discourse on how to integrate DS with regular software development and productize the results. Sadly, any mention of how testing fits in is missing, other than A/B tests. Don't you wish A/B tests stuck with the label "experiments", leaving "tests" to mean what they should mean?

<https://www.oreilly.com/ideas/what-is-hardcore-data-science-in-practice>

More on productization of Machine Learning (ML) in this glorious, meaty and long document from Google. The testing aspect only covers best practices for testing your model (i.e. validating that the model gives reasonable predictions when fed real production data, which is distinct from the training data set). This type of testing is usually performed by the data scientists themselves, analogous to developer-owned unit testing. While light on testing, this paper is great on everything else.

<http://martin.zinkevich.org/rules_of_ml/rules_of_ml.pdf>

So, how do we test ML systems? Unfortunately, we have no idea. Only generalities here. A good start if you coming in at zero level.

<https://www.stickyminds.com/article/testing-moving-target-how-do-we-test-machine-learning-systems>

Finally, something to bite into: the first post I've seen with specifics of testing a data science model, written by a tester:

<http://angiejones.tech/test-automation-for-machine-learning/>

For an idea of how one might devise tests to break ML, this covers adversarial attacks on neural networks, or how to fool deep learning:

<https://blog.acolyer.org/2017/02/28/when-dnns-go-wrong-adversarial-examples-and-what-we-can-learn-from-them/>

If you take on testing of DS models or applications using them, you will necessarily begin with understanding of the data that goes into the model, and will be working with large data sets. This document, based off a Google guide "Good Data Analysis", has useful recommendations. Not specifically testing related but just... good.

<http://www.unofficialgoogledatascience.com/2016/10/practical-advice-for-analysis-of-large.html>

For some comic relief, this detailed post goes through apocalyptic scenarios of AI taking over the world, with movie examples, and ties it back to testing by claiming that good QA practices can prevent catastrophe. The authors are banking on test-first methodologies (such as TDD) and risk-based testing to keep AI from turning evil.

<http://irishtechnews.ie/can-qa-testing-prevent-the-inevitable-robot-apocalypse/>

Off-Topic
=========

Where AI-powered testing bots fit into the engineering process:

<https://www.stickyminds.com/interview/role-artificial-intelligence-testing-interview-jason-arbon>

Future of QA is in coexistence of humans with QA bots:

<https://www.techwell.com/techwell-insights/2017/04/think-differently-about-future-software-testing>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
