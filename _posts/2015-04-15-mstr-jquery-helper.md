---
layout: post
title: mstr-helper&#58; A jQuery plugin to help with MicroStrategy customisation
date: 2015-04-15 21:04
category: MicroStrategy
tags: Technical SDK JavaScript
---

So, today I've decided to do some of my exploratory work in the open. I've published a (very) small jQuery plugin, and accompanying MicroStrategy web plugin to make web customisation easier, and simpler to get started with.

The [source code is here](https://github.com/rinbo-consulting/jquery-mstr-helper), and [I've published to npm too](https://www.npmjs.com/package/mstr-helper), which is the new home for jQuery plugins.

It provides a simple lazy-loading mechanism, and will grow to include various helper functions to make selecting and manipulating elements on the dashboard more straightforward. At first, it just has a selector extension to make finding the appropriate elements to manipulate easier.