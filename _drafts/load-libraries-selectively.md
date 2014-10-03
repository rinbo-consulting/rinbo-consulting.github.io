---
layout: post
title: Loading JavaScript libraries selectively in MicroStrategy Web
date: 2014-05-24 13:04
category: MicroStrategy
tags: Technical SDK
---

Hacking JavaScript libraries into the MicroStrategy Web interface is pretty easy ([Bryan describes a couple of ways to do it here](http://www.bryanbrandow.com/2013/01/using-jquery-in-microstrategy-dashboards.html)), but there's a third way, that's a little bit more involved, that gives you the best of both worlds.

We'll be adding an extended property to the metadata for Report Services documents (or even reports, if they're the category of object you need to use an external library with), and then adding a plugin in that generates the appropriate `<script>` tags in the HTML if the extended property is set. This way, with a little more effort up front, we can avoid adding custom HTML to load the library into the document (simplifying debugging), and also avoid the unnecessary overhead of code that's not needed to render our "normal" pages. Additionally, the extended property is moved around correctly by Object Manager and its relatives, so there's nothing manual to do once the setting's in place.