---
title: "Tester's Digest #45: Security Testing"
excerpt: We covered security risks in the last issue, and will continue the topic into security testing.
---

TESTER'S DIGEST
===============
ISSUE #45 - January 28, 2018

We covered security risks in the last issue, and will continue the topic into security testing.

Topic: Security Testing
=======================

Quality vs security. Some questionable statements there such as "quality is binary – the software either works or it doesn’t", but good links to resources on weaknesses. Mentions fuzz testing as a useful technique to find security holes.

<https://www.synopsys.com/blogs/software-security/does-software-quality-equal-software-security/>

What it's like to be a bug hunter in the security space:

<https://blog.cobalt.io/learn-through-play-following-the-path-of-a-bug-hunter-8ed64092aa7b>

Yelp's public bug bounty program finds some hard-to-find critical security vulnerabilities, while the earlier private program weeded out the common ones:

<https://engineeringblog.yelp.com/2016/12/100-days-public-bug-bounty-program.html>

Automating security acceptance tests in a BDD framework, using OWASP ZAP:

<https://opencredo.com/automating-your-security-acceptance-tests/>

Security patterns in web apps, and a Rails specific tool called SPACE (Security PAttern CheckEr)
that promises to find bugs if the developer defines a lightweight mapping from code to patterns:

<https://blog.acolyer.org/2017/02/07/finding-security-bugs-in-web-applications-using-a-catalog-of-access-control-patterns/>

DIY pen testing:

<https://highon.coffee/blog/penetration-testing-tools-cheat-sheet/>

OWASP mobile security testing guide defines itself as a comprehensive manual and certainly is, with sections on general code quality and cryptography in mobile apps, common attacks, memory corruption bugs, auth architectures, network communication testing, and specifics of Android and iOS. It is, in a word, amazing, well maintained and current.

<https://github.com/OWASP/owasp-mstg>

If you need to test HTTPS clients implementing the common TLS encryption protocol, Yelp gives you tlspretense-service tool, and Netflix open sourced bettertls which specifically targets name constraints for HTTPS clients:

<https://engineeringblog.yelp.com/2015/05/https-client-testing-made-easy.html>

<http://techblog.netflix.com/2017/04/bettertls-name-constraints-test-suite.html>

Security Monkey is another tool from Netflix, this one monitors AWS changes and alerts on security problems, also released for Google Cloud Platform:

<http://techblog.netflix.com/2017/03/netflix-security-monkey-on-google-cloud.html>

Off-Topic
=========

An interesting take on the limitations of Chaos Engineering:

<https://medium.com/production-ready/the-limitations-of-chaos-engineering-2a74816c0df3>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
