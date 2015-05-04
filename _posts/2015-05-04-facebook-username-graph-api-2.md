---
layout: post
title:  "Getting Facebook Username using Graph API 2.0"
date:   2015-05-04 01:11:00
categories: PHP Facebook
---

Facebook started upgrading all apps to Graph API v2.0 on April 30, 2015. As with every change, this may bring some headaches to those of us using Graph API v1.0, for instance one important endpoint was removed in v2.0 > *username* [Facebook Platform Changelog].

This change broke the authentication process for one of my customers' web applications, whenever someone tried to log in they were redirected to the login form without error or warning notices. Besides that, they were being registered with a fallback username I put in place when none was specified.

After some testing I succeeded in adapting my application (using CodeIgniter) to work with Graph API v2.0. Here it is how I get the Facebook username which is needed for new users to get registered the first time they log in using their Facebook account:

<script src="https://gist.github.com/josesayago/47ef06fb094fdc0893a9.js"></script>

[Facebook Platform Changelog]:	https://developers.facebook.com/docs/apps/changelog