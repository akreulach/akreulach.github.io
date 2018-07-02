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

The program being developed currently depends on two main sources: the [PyEphem][pyephem] Python library and [Astrometry.net's][astrometry] offline application.

This post will slowly grow as I attach progress reports, papers, presentations, and resources related to the work. For now, however, I will end this simply: Carthago delenda est.

6/24 Edit: Now including links to my project partner, our working [paper][paper], and our [presentation][pres].

6/25 Edit: Extremely unsorted collection of [links][lnks] to references in the paper.

7/01 Edit: We've created our first batch of [star photos][photos]. Still to be analyzed, results to come.

[astrometry]: 	https://astrometry.net
[pyephem]: 		https://rhodesmill.org/pyephem
[harrison]: 	https://harrisonwelch.github.io
[paper]:		https://akreulach.github.io/files/AUBPaper.pdf
[pres]: 		https://akreulach.github.io/files/midterm.pptx
[lnks]:			https://akreulach.github.io/files/links.txt
[photos]:		https://akreulach.github.io/files/star_photos.zip