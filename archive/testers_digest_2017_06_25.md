---
description: Continuous Integration / Continuous Delivery. Today we look at the testing aspects of CI/CD.
---

TESTER'S DIGEST
===============
ISSUE #21 - June 25, 2017

---

Today we look at the testing aspects of CI/CD (Continuous Integration and Continuous Delivery).

In the off-topic section, I will start posting links to things somewhat outside your usual tester's curriculum (if such a thing existed) yet worth learning.

Topic: Continuous Integration / Continuous Delivery
===================================================

What is Continuous Delivery:

<https://labs.klipfolio.com/blog/what-is-continuous-delivery-agile>

And how to do it right (including a call to "create and implement a quality control strategy"):

<https://labs.klipfolio.com/blog/continuous-delivery-practices>

How human testing fits into CI/CD: the idea of this post is to create "continuous human testing" process whereby testers use automation tools to quickly spin up testing environments from CI, then perform exploratory testing activities on the software "as a customer might see and use it". With proper tooling, humans can also reproduce bugs as part of support calls.

<https://blog.gurock.com/the-future-of-near-instant-deployments-and-continuous-human-testing/>

"Dark launching" at Facebook: before releasing a new feature, route a subset of user queries to the backend as silent queries, without returning results to the users, with the goal of exposing pain points from the new load across the entire system:

<https://www.facebook.com/note.php?note_id=96390263919>

"Dark Canary" at LinkedIn: similar to Facebook's "dark launching", stand up a production instance of the new service and tee off traffic from a production source node to the canary, without returning results upstream, but compare to the current version of the service to identify health problems and capacity requirements.

<https://www.usenix.org/conference/srecon17americas/program/presentation/barot>

Automate all the things, right? Perhaps not all... this post does a good job of describing risks of automation in deploy process, and reasons for keeping certain actions manual.

<https://blog.skyliner.io/risky-business-requires-active-operators-9debbb082995#.a31cxs9ul>

Deployment raciness and backwards compatibility, lessons from RainforestQA startup:

<https://www.rainforestqa.com/blog/2017-05-11-common-pitfalls-of-continuous-delivery-deployment-raciness/>

Why rollback of a failed/buggy deploy is not really a thing (the implication being, you better be testing before pushing code to production... do not count on rollback as the easy bug mitigation strategy):

<https://blog.skyliner.io/you-cant-have-a-rollback-button-83e914f420d9>

Off-Topic
=========

Things worth learning: a visual introduction to probability and statistics.

<http://students.brown.edu/seeing-theory/>

With an add-on illustrating spurious correlations with no causation:

<http://tylervigen.com/spurious-correlations>


---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
