---
title: "Tester's Digest #4: Security Testing"
excerpt: This issue's topic of Security Testing was prompted by this week's news of the Cloudbleed security leak, and proof of successful attack on SHA1 encryption. Disclaimer! I'm not a security expert by any means, so caveat emptor.
---

TESTER'S DIGEST
===============
ISSUE #4 - Feb 26th, 2017

---

This issue's topic was prompted by this week's news of the Cloudbleed security leak, and proof of successful attack on SHA1 encryption. Disclaimer: I'm not a security expert by any means, so caveat emptor.

Topic: Security Testing
=======================

A very good list of resources for security testing and more:

<https://github.com/sbilly/awesome-security>

Security breaches and how to deal with them (an incident responder's view, useful for testers too):

<https://medium.com/starting-up-security/learning-from-a-year-of-security-breaches-ed036ea05d9b#.cstj51u9t>

Extreme security testing, the Red Team approach at Facebook:

<https://medium.com/starting-up-security/red-teams-6faa8d95f602#.q9vbu163v>

At the other end of the spectrum, beginner steps in checking for security vulnerabilities, using Fiddler as the tool:

<https://dojo.ministryoftesting.com/lessons/but-i-m-not-a-security-tester-security-testing-on-the-web-for-the-rest-of-us>

How to reengineer a piece of software (in this case, TLS security protocol spec and implementation) for quality and testability:

<https://blog.acolyer.org/2016/02/23/not-quite-so-broken-tls/>

Security questions (you know, "what was the name of your first pet?") are deeply insecure, and what to do about it:

<https://www.wired.com/2016/09/time-kill-security-questions-answer-lies/>


News
====

Don't panic. The big security holes named this week - collision in SHA-1, and Cloudbleed leak - are not known to be exploited in the wild. Safeguard yourself calmly.

SHA-1 hash function, known to be insecure for years, is now proven as such: cryptographers from Google and SWI Institute intentionally generated a SHA-1 collision on two distinct PDF files (underlying code to be released after 90 days). If you were still using SHA-1 for PGP encryption or anything else, please stop.

<https://security.googleblog.com/2017/02/announcing-first-sha1-collision.html>

SHAttered website has more practical details, including advice not to put those two PDFs into a Subversion repository, as that would break the svn server! They also offer a tester to validate if your files were part of a collision attack, with the promise that your uploaded files don't get stored. To trust or not to trust...

<http://shattered.io/>

Onto Cloudbleed: a Heartbleed-style buffer overflow bug in Cloudflare's code resulted in HTTP responses including random snippets of information from unrelated sites backed by Cloudflare service (such as: Fitbit, Uber, OKCupid). Your passwords and other personal details may now be cached all over the interwebs. Incident report from Cloudflare itself:

<https://blog.cloudflare.com/incident-report-on-memory-leak-caused-by-cloudflare-parser-bug/>

As described by the discoverer from Google's Project Zero:

<https://bugs.chromium.org/p/project-zero/issues/detail?id=1139>

For a shorter read, high level post with advice (to change all your passwords and use a password manager):

<https://medium.com/@octal/cloudbleed-how-to-deal-with-it-150e907fd165#.pluz827a3>

Fun
===

While you're changing all those passwords in the wake of Cloudbleed, see if you want to run them through this "slightly evil password strength checker". Don't miss the inspirational xkcd.

<https://github.com/SirCmpwn/evilpass>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
