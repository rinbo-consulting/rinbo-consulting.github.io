---
layout: post
title: Beyond Command Manager, into true source control
date: 2014-02-20 19:37
category: MicroStrategy
tags: Groovy SDK Technical Java
---

As MicroStrategy's declared plan to move away from desktops into the cloud progresses, there is one nice side effect. As their old COM-based applications (Desktop/Developer, Object Manager) are allowed to wither on the vine, more functionality moves into their Web API, which means Java, which means plenty of modern technologies for us to leverage.

I mentioned in an earlier post that Groovy is a Java-based scripting language that already allows us to move past the limited procedural functionality that comes in Command Manager. As more and more functionality (whether it be documented or documented) becomes visible in this API, a true MicroStrategy [Domain-specific Language][1] (DSL) becomes a possibility, [using Groovy][2].

Administrative tasks that were previously complex could be made trivially simple, particularly time-intensive ones involving lots of objects. As full creation of all types of objects becomes possible through the web interface, using a DSL to generate objects is also a reality, and that means full, text-based, version control, using whichever platform you decide. Whilst MicroStrategy's internal dependency checks will still prove useful, those version GUIDs could become irrelevant. True comparision, based on definitions, become the basis for checking the validity of objects between projects.

Now, this might very well be something MicroStrategy is already planning, but even if it isn't, it's a side effect of the move to the cloud, if they choose to do away with their desktop apps. A hugely powerful, mature, and broad, toolset is almost at hand. Exciting times, particularly for those of us working on large deployments.


[1]: http://en.wikipedia.org/wiki/Domain-specific_language
[2]: http://www.slideshare.net/glaforge/groovy-dsls-from-beginner-to-expert-guillaume-laforge-and-paul-king-springone2gx-2011