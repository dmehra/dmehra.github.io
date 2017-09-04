---
description: Observability. -- How to know if your service/application is doing well, through metrics and alerts based on them, and how to debug it when it's not doing well, through logs.
---

TESTER'S DIGEST
===============
ISSUE #27 - August 7, 2017

---

Tester's Digest has had half a year's worth of weekly newsletters! Thanks for sticking with me this long, and please keep sending pointers to good materials. Today's issue looks at observability: How to know if your service/application is doing well, through metrics and alerts based on them, and how to debug it when it's not doing well, through logs.

Topic: Observability
====================

Twitter's 2013 observability stack (metric collection, storage, querying, dashboards, monitoring / alerts):

<https://blog.twitter.com/2013/observability-at-twitter>

On designing better alarms, so you get timely alerts on actionable events: "The trouble with alarm design is that it seems obvious. It’s not."

<https://humanisticsystems.com/2015/10/16/fit-for-purpose-questions-about-alarm-system-design-from-theory-and-practice/>

When you are debugging an issue using timeline charts of several metrics and find them to align visually, are they indeed correlated?

<https://www.vividcortex.com/blog/correlating-metrics>

Or maybe your debugging is based on logs. If so, these things about logs are good to know.

<https://honeycomb.io/blog/2017/04/lies-my-parents-told-me-about-logs/>

Solving the Goldilocks problem in logging not too much, not too little, but the most interesting events.

<https://honeycomb.io/blog/2017/06/build-observable-systems/>

What to monitor about your app, take 1: Google's 4 golden signals which I combined into a mnemonic LETS = Latency, Errors, Traffic, Saturation

<https://blog.netsil.com/the-4-golden-signals-of-api-health-and-performance-in-cloud-native-applications-a6e87526e74>

What to monitor about your app, take 2 and 3, for good measure: RED = Request rate, Error rate, Duration of requests; USE = Utilisation, Saturation, Error metrics

<https://twitter.com/i/web/status/852341680946544640>

"Logs and metrics are complementary" and what each is good for, a great overview if you ignore the "observability > unit tests" intro.

<https://medium.com/@cindysridharan/logs-and-metrics-6d34d3026e38?__s=b2sexxzpefs371hbo9ts>

Off-Topic
=========

Things worth learning: Hill's guidelines for evaluating whether a causal relationship exists, presented via xkcd comics:

<http://livefreeordichotomize.com/2016/12/15/hill-for-the-data-scientist-an-xkcd-story/>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
