+++
title = 'Modern Authentication'
date = 2024-02-20T15:40:44+11:00
draft = true
tags = ['authentication', 'CISO']
revision = 1
+++

![Authentication](https://toobstar.github.io/images/caveman_door.jpg)

### A short history of user authentication 

Usernames & passwords on computers as a model for controlling access have been around for ever (well ... since the 1960s).  In the internet era this evolved to the username just being your email which meant only one additional thing to keep track of.  But as our use of the web exploded and eventually led into more sensitive activities like e-commerce our ability to keep track of passwords quickly fell apart.  This led to common and reused passwords, which led to techniques for brute-force cracking of passwords, which led to password expiration rules, which led to password complexity rules, which led to password management applications.  

The proliferation of passwords we needed to keep track of has largely been mitigated by Google and Microsoft dominating email services amongst personal users and enterprise cloud directory services for business users allowing for single-sign-on (SSO) to merge authentication control into a few highly trusted entities.  But as consolidation of trust has occured the increased value put on each log-in as well as the ability of modern graphics cards to crack passwords even more quickly has driven us towards multi-factorial techniques to provide secure access.  


### A multi-factorial approach (MFA)

The three basic approaches ("factors") used for authentication are:
- Something you know (such as a password)
- Something you have (such as a key)
- Something you are (such as your fingerprint)

In the early internet days, the focus was on what you knew as the ability to assess physical or biometric security was limited. Beyond your password, you might also have been asked to record your mother's maiden name or where you were born.  These highly sensitive personal details were willingly handed over to provide an ability to 'reset your password' more readily. 

Modern MFA typically involves a password plus an additional factor based on something you have or are.  There are many types of additional factors available and each has pros and cons which make them suitable for difference circumstances:


| MFA Type  | Pros      | Cons      | Risks     |
|:----------|:----------|:----------|:----------|
| Email | Simple & available in all cases | Requires internet access | Email could be compromised |
| SMS | Simple & commonly available | Requires phone & reception | Dependent on phone security |
| Printed codes | No exposure to online risks | Could be lost when needed | No control if lost |
| Time based one-time password (TOTP) App | Widely available | Inconvenient & requires phone | Minimal  |
| Physical security key (USB) | Convenient and no internet needed | Could be lost | Could be used by 3rd party if lost |
| Fingerprint | Convenient and easy | Won't work with gloves or a bandage  | Trusting 3rd party with non-replaceable sensitive information |
| Face scan | Convenient and easy | Won't work with a face mask  | Trusting 3rd party with non-replaceable sensitive information |

All of these approaches provide a significant uplift in security standard in comparision with a basic username and password. Each does have some potential risk or inconvenience that must be considered.  The ultimate in convenience and security is definitely a biometric approach which is the most user friendly whilst providing an excellent defence against potential risks.

### Current Best Practice

Thankfully we are getting convergence in the last few years on modern techniques known as **passwordless** authentication.  This "recent phenomenon" ([10 years in the making](https://fidoalliance.org/overview/history/)) is breaking into the mainstream via **passkey** implementations from [Apple](https://support.apple.com/en-au/guide/iphone/iphf538ea8d0/ios), [Google](https://blog.google/technology/safety-security/the-beginning-of-the-end-of-the-password/) and [Microsoft](https://www.microsoft.com/en-us/security/business/solutions/passwordless-authentication).  This allows your device (e.g phone, tablet or laptop) to utilise in-built biometric capabilities to provide a secure and private authentication on a trusted platform to a un-trusted 3rd party without revealing your private information.  This is a huge win as both the security outcome and the user experience is excellent.

As a user our deep relationship with these trusted partners (the Googles and Apples) may cause anxiety with respect to privacy but it allows them the opportunity to provide an incredibly powerful additional security capability.  Given they know what devices we use, when we work, where we live etc. they can discern what is likely to be a legitimate activity from a problematic one and act accordingly.  This capability is variously known as 'context aware access' or 'suspicious activity detection' or what I prefer to know as 'risk based authentication.