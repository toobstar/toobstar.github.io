+++
title = 'Modern Authentication'
date = 2024-02-20T15:40:44+11:00
draft = true
tags = ['authentication']
revision = 1
+++

![Authentication](https://toobstar.github.io/images/caveman_door.jpg)

### A short history of user authentication security 

Usernames & passwords on computers as a model for controlling access have been around for ever (well ... since 1961).  In the internet era this quickly evolved to the username just being your email which meant only one additional thing to keep track of.  But as our use of the web exploded our ability to keep track of passwords quickly fell apart.  This led to common and reused passwords, which led to techniques for brute-force cracking of passwords, which led to password expiration rules, which led to password complexity rules, which led to password management applications.  

The explosion of passwords we needed to keep track of has largely been mitigated by Google and Microsoft dominating email services amongst personal users and enterprise cloud directory services amongst business users allowing for single-sign-on (SSO) to merge authentication control into a few highly trusted entities.  But as consolidation of trust has occured the increased value put on each log-in as well as the ability of modern graphics cards to crack passwords even more quickly has driven us towards multi-factorial techniques to provide secure access.  


### A multi-factorial approach (MFA)

The three basic approaches ("factors") used for authentication are:
- Something you know (such as a password)
- Something you have (such as a USB key)
- Something you are (such as your fingerprint)

In the early internet days, the focus was on what you knew as the ability to assess physical or biometric security was quite limited. Beyond your password, you might also have been asked to record your mother's maiden name or where you were born.  These highly sensitive personal details were willingly handed over to provide an ability to 'reset your password' more readily. 

Modern MFA typically involves a password plus an additional factor based on something you have or are.  There are many types of additional factors available and each has pros and cons which make then suitable for difference circumstances:


| MFA Type  | Pros      | Cons      | Risks     |
|:----------|:----------|:----------|:----------|
| Email | Simple & available in all cases | Requires internet access | Email could be compromised |
| SMS | Simple & commonly available | Requires phone & reception | Security on phone not always consistently strong |
| Printed codes | No exposure to online risks | Could be lost when needed | No control if lost |
| Time based one-time password (TOTP) App | Widely available | Slow / inconvenient & requires phone | Minimal  |
| Physical security key (USB) | Convenient and no internet needed | Could be lost | Could be used by 3rd party if lost |
| Biometric (finger-print / face-scan) | Convenient and easy | May require additional device (e.g phone)  | Trusting 3rd party with non-replaceable sensitive information |

