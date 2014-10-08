---
layout: page
title: Current Projects
permalink: /current-projects/
---

I often have something on the back burner, to keep my brain ticking over during those times when paid work isn't providing the challenge that it might. At the moment I'm working on a couple of BI-related projects:

* **Deployment Director** - This is a web application for managing MicroStrategy code deployments. It handles Object Manager packages, automatically applying them, in batches if necessary, and creating undo packages for you. You can instantly see which pieces of functionality are where in the deployment cycle.
* **Schema Source Code** - Version control is an area of weakness for MicroStrategy. Objects with identical definitions can have different Version IDs (unless you're careful with how you make changes; see Deployment Director). This Groovy-based project produces human-readable source files for all MicroStrategy schema objects. This files can then be traditionally source-controlled, and the real differences between projects can be easily visualised.