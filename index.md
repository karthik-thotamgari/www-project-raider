---

layout: col-sidebar
title: OWASP Raider
tags: authentication hylang python
level: 2
type: tool
pitch: Automate or attack any web authentication system

---


![Raider logo](./assets/images/raider_logo.png)


**Raider** is a framework designed to test authentication for web applications. While web proxies like [ZAProxy](https://www.zaproxy.org/) and [Burpsuite](https://portswigger.net/burp) allow authenticated tests, they don't provide features to test the authentication process itself, i.e. manipulating the relevant input fields to identify broken authentication.

**Raider** treats the authentication as a finite state machine. Each authentication step is a different state, with its own inputs and outputs. Those can be cookies, headers, CSRF tokens, or other pieces of information.

**Raider** was developed with the following goals:

* To abstract authentication concepts using Python objects.
* To support most modern web authentication features.
* To make it easy to add new features for users.
