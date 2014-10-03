---
layout: post
title: Hacking MicroStrategy the right way; jQuery and the Tasks API
date: 2014-05-18 22:37
category: MicroStrategy
tags: jQuery "Tasks API" Technical SDK
---

The time has come - you want to customise some aspect of MicroStrategy's web interface, but you're scared of the SDK and its documentation (although it's not as frightening as you think), and the functionality you need is based around user interactions. You're okay with a little JavaScript, so you tentatively add a customisation to load the jQuery library ([make sure you do that the smart way though](load-libraries-selectively)).

Just because you're going off-piste with your own front-end code that MicroStrategy doesn't know about, you're not disconnected entirely. There's a whole simple API available to you to assist with functionality far beyond what you can achieve with just jQuery; the **Tasks API**.

This API is pretty powerful, in fact it's used to power the Visual Insights flash mode.