---
layout: post
title: Loading JavaScript libraries selectively in MicroStrategy Web
date: 2014-05-24 13:04
category: MicroStrategy
tags: Technical SDK JavaScript
---

Hacking JavaScript libraries (jQuery, Prototype, D3.js et al) into the MicroStrategy Web interface is pretty easy ([Bryan describes a couple of ways to do it here][1]), but there's a third way, that leverages some built-in MicroStrategy functionality, and allows you to easily execute code when the external libraries are asynchronously loaded.

It's an area that the formal documentation doesn't cover (yet), but [buried in this presentation from Las Vegas 2014][2] is a handy JavaScript function. It's only available in Express mode, but if you're customising a document in this manner, you're almost certainly planning on restricting the functionality to this mode.

{% gist paulbailey/22e06c91e7d41b51a010 %}

Adding a fragment like that to an HTML Container on your Report Services document will load an external script (or a number of scripts, as the function takes an array), and then call the function you specify once they've loaded. It's an ideal workflow if you need to load a library, and then immediately use it to customise the appearance of the document.

**Update: [I've created a simple plugin]({% post_url 2015-04-15-mstr-jquery-helper %}) to facilitate the sort of selective loading I describe in this post.**

[1]: http://www.bryanbrandow.com/2013/01/using-jquery-in-microstrategy-dashboards.html
[2]: https://www.microstrategy.com/us/microstrategyworld/resource?world-res=v1247