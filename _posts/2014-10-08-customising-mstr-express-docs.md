---
layout: post
title: Customising MicroStrategy Report Services Documents
date: 2014-10-08 13:04
category: MicroStrategy
tags: Technical SDK JavaScript
---

Express mode is in many ways ideal for customisation (or customization, as our American cousins have it) with JavaScript. By locking down the amount of interactivity the user can have with objects you've placed on the screen, you have fewer scenarios that your customisations have to cater for.

There are problems though. If you're doing something very superficial with jQuery, you've probably discovered that it's not easy to get a reference to the DOM element you want to manipulate, and if you do (usually by finding the 'K value' of the object you're interested in), you also find that it changes when changes are made to the document in MicroStrategy. There's also the problem of objects not rendering in the DOM until they become visible on screen.

This is why I would strongly encourage you to become familiar with the developer console in your web browser. There are plenty of objects beyond the HTML DOM to look at.

In particular, there is the `mstrmojo` object, which contains all the JS functionality MicroStrategy uses. It has an `all` property which contains references to all of the objects that are on the document, rendered or not. It also has properties that you can use to find the appropriate object every time, which won't change accidentally when some seemingly-unrelated change is made elsewhere on the document.

As I say, I encourage you to have a dig around the objects that you can see in the console, but here's a useful example function to get you started.

{% gist paulbailey/02c150eac6cd72c38e08 %}