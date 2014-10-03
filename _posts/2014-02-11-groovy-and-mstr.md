---
layout: post
title: Getting Groovy with the MicroStrategy SDK
date: 2014-02-11 20:14
category: MicroStrategy
tags: Groovy SDK Technical
---

MicroStrategy has a reasonably well-documented Web SDK, using Java, but don't think that you're restricted to just developing customisations to the web interface.

Although the functionality of Command Manager has been extended to include procedures, which allows programatic manipulation of objects, it's still quite limited. It takes one beyond using Excel to create repetitive scripts, but non-trivial tasks are still harder than they should be. This is primarily because Command Manager's vocabulary is still limited, even though it's extending with each release.

Become familiar with the slightly more complicated Web SDK, equip yourself with an installation of [Groovy][1], and we can easily create straightforward scripts that accomplish tasks far beyond the realms of what is possible with Command Manager.

To give a real world example, I recently needed to edit around 2,000 reports which had prompts embedded in their templates. These reports needed the template prompts answered, and then saved in the definition of the report, such that the only prompts that remained were in the report filters.

There is no mechanism to do this within Command Manager, and I shudder to think how long it would have taken to do manually. The script probably took around 30 minutes to put together (after I had reacquainted myself with the appropriate classes in the SDK), and 10 minutes to execute. Even allowing 30 seconds per report that would have taken over 16 hours to do manually.

My intention is to build up an open sourced library of useful generic scripts, so I'll expand on how to install and use Groovy with the MicroStrategy SDK in a future post.

[1]: http://groovy.codehaus.org