---
layout: post
title:  "Auburn REU on Smart UAVs"
date:   2018-06-19 13:23:03 -0500
categories: masterpost update
---

![Auburn Samford Hall]({{ "/files/SamfordHall.jpg" | absolute_url }})

I'm spending eight weeks of summer at Auburn University in Alabama working at an NSF REU on the topic of smart UAVs. My team consists of [Harrison Welch][harrison] and myself. We've been given broad creative and individual freedom to pursue essentially any subtopic within the scope of the program, and as a result Harrison Welch and I have chosen to work on UAV navigation in the absence of GPS.

What this means is that we have been trying to develop a system to navigate a blind, deaf, and dumb drone with as few caveats as possible while being as precise as possible. The method we've decided on is a delightful callback to my general fascination with the old and dusty: astronavigation.

Our plan is to develop a system that turns many aspects of general drone design on their heads. The camera will be mounted above the drone and facing the sky; and rather than the usual high-tech lasers and sonar approach to problems, we will be taking a picture and doing chapters worth of mathematics. There's something a little romantic about it.

The program being developed currently depends on one main source: [Astrometry.net][astrometry]. Astrometry.net is a public, open-source website hosting a program that analyzes starfield images and finds a host of useful metadata without any outside information. It's a general solution to the 'lost in space' problem.

We've used this information to develop a completely novel approach to celestial navigation that we're calling Zenith Image Analysis.

Essentially, instead of finding the angle of the observer to a set of reference stars like in traditional astronavigation, we're using mathematics to determine the celestial coordinates of the observer's zenith, or the point directly overhead, and using various facts of geometry to convert that into latitude and longitude.

Results are promising, being able to penetrate light cloud cover and function even under slight lunar light pollution.

For more information, I've attached the [paper][paper], [presentation][pres], and [poster][pstr].

6/25 Edit: Extremely unsorted collection of [links][lnks] to references in the paper.

[astrometry]: 	https://astrometry.net
[harrison]: 	https://harrisonwelch.github.io
[paper]:		https://akreulach.github.io/files/AUBPaper.pdf
[pres]: 		https://akreulach.github.io/files/FinalPowerpoint.pptx
[lnks]:			https://akreulach.github.io/files/links.txt
[pstr]:			https://akreulach.github.io/files/finalPoster.pdf