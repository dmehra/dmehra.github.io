---
title: "Tester's Digest #44: Security Risks"
excerpt: In the aftermath of Spectre and Meltdown, let's talk about security risks.
---

TESTER'S DIGEST
===============
ISSUE #44 - January 22, 2018

In the aftermath of Spectre and Meltdown, let's talk about security risks. A lot of my links in this issue are to The Morning Paper blog because its awesomeness is unsurpassed. Many modern security vulnerabilities are based on observable side effects, and Adrian Colyer has covered various kinds in his writeups.

Topic: Security Risks
======================

The new OWASP list of top security risks is out! See the 2017 PDF for the application security, and 2016 for mobile. This is a great resource for testers and developers alike.

<https://www.owasp.org/index.php/Category:OWASP_Top_Ten_Project>

How does Meltdown attack work, really? The Morning Paper tells all. In a nutshell, the attacker's makes an access to the memory location whose content they wish to know, but are not authorized to access; however, just before that access, the code throws an exception. The plucky CPU will speculatively execute the post-exception code instruction anyway, as a performance optimization (it didn't know you'd be throwing an exception, and optimized for the happy path). After the exception, the speculative execution path gets rolled back, but leaves a side effect - values in the cache. Now the attacker can do Flush+Reload, iterating over the pages (inside the exception handler) until it finds the cache hit and can recover the secret.

<https://blog.acolyer.org/2018/01/15/meltdown/>

What about Spectre? It's like Meltdown's scarier sibling, since it can achieve similar outcome without needing to trigger an exception, by exploiting speculative execution of branched code. My favorite blog has it covered as well, with a code sample in Javascript if you'd like to run your very own exploit.

<https://blog.acolyer.org/2018/01/16/spectre-attacks-exploiting-speculative-execution/>

Required reading for all your friends who are front-end developers - here's how to (not) potentially leak all the sensitive information from your user-data-collecting webpage via nefarious npm modules. A fun read.

<https://hackernoon.com/im-harvesting-credit-card-numbers-and-passwords-from-your-site-here-s-how-9a8cb347c5b5>

A look at the attacks on databases that use access leakage, or communication volume leakage (which all known systems suffer from!); also known as "side channel attacks", these approaches latch on to the information revealed by the communication pattern itself, even though its contents are encrypted. Think of the thin vs thick envelope received by the college applicants - the postman knows whether you got admitted... The obvious defense is padding of the records (ie: everybody gets a fat envelope stuffed with blank pages), but as it is expensive, most existing practical systems are non-storage-inflating.

<https://blog.acolyer.org/2016/11/16/generic-attacks-on-secure-outsourced-databases/>

Systems built on property revealing encryption promise to allow private unencrypted data to stay only in the user's browser, while all communication with the server and server-side processing is encrypted (while still allowing operations such as search and sharing by the server). However, there are types of attacks this setup is open to. Observing access patterns can be enough to infer private information, for example: if the user's shopping cart (items and prices) is encrypted, but the user's search history on the shopping website is not, it's a good guess that the shopping cart consists of recently visited items.

<https://blog.acolyer.org/2016/11/15/breaking-web-applications-built-on-top-of-encrypted-data/>

All your base are belong to us... with a simple USB stick inserted into a locked (!) PC - Raspberry Pi-based PoisonTap by the white-hat hacker Samy Kamkar. The malicious code is hidden in the browser cache (you clean that out regularly don't you? :-)) and the preconditions are Wi-Fi access and at least one open browser tab that periodically downloads updates. Once PoisonTap is unplugged, the backdoor remains in the browser cache, giving the hacker a way in using standard exploits.

<https://www.wired.com/2016/11/wickedly-clever-usb-stick-installs-backdoor-locked-pcs/>

Code signing is a standard technique that you "just do" to validate integrity of software updates, right? Not in cars, apparently:

<https://www.wired.com/2016/09/tesla-responds-chinese-hack-major-security-upgrade/>

Weaknesses of password managers, types of attack against them, and possible defenses (secure filling). Based on this, 1Password is the better choice, with LastPass a possible alternative (they both must have improved since 2014 when studied):

<https://blog.acolyer.org/2017/02/06/password-managers-attacks-and-defenses/>

Off-Topic
=========

The Hawaii incident of erroneously triggered missile warning has its roots in the UX design of the selection screen. What would you have clicked, the DRILL link, or the link right under TEST MESSAGE? Don Norman, the author of "The Design of Everyday Things", walks through the many problems with Hawaii UI and the proper design of systems with "test mode".

<https://www.fastcodesign.com/90157153/don-norman-what-went-wrong-in-hawaii-human-error-nope-bad-design>

---

If you received this email directly then you're already signed up, thanks! Else
if this newsletter issue was forwarded to you and you'd like to get one weekly,
then you can subscribe at <http://testersdigest.mehras.net>

If you come across content worth sharing, please send me a link at
<mailto:testersdigest@mehras.net>

---
