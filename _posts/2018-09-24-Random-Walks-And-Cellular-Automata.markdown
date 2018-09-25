---
layout: post
title:  "Random Walks and Cellular Automata"
date:   2018-09-24 20:38:03 -0500
categories: masterpost update
---

As my junior year is starting to spool up I've started to think about what my next personal project is going to be. I've been playing with a few ideas but just one has stuck firmly in my head: mathematical visualization as art. I've always enjoyed the primordial beauty of mathematics and I think sculpture and visual art is one of the best ways to get that basic understanding across. The visual proof of the Pythagorean theorem is my favorite example of this idea.

I've made a few toy projects that demonstrate the sort of basic beauty of these concepts. I included a sample of my random walk simulation below.

![Random Walk Visualization]({{ "/files/RandomWalk.jpg" | absolute_url }})

Random walks are an extremely simple but fascinating and appealing concept for casual mathematics. The idea is simple: create a pointer, then at each time step move the pointer a set distance in a random direction and record where it steps. My code is a bit crude since it doesn't prevent the pointer doubling back on itself, but it creates very nice cloudlike patterns. I've used a few choice output patterns as continents in my fantasy cartography projects.

But, despite the stunning results one can achieve with a random walk it doesn't quite have the properties I am most interested in. Specifically, universality and elements of order in the chaos. Fortunately, my next example does.

![Sample ASCII Cave]({{ "/files/CellularCave.jpg" | absolute_url }})

This image is an example output of a function I wrote to generate cave terrain. Note that the characters are ASCII monocode, so their width is even but they aren't proper squares. I say this to explain the tall and slim look of the caves.

The function depends on an old but still thoroughly interesting concept called cellular automata(CA). The basic idea here is to create a landscape of 'cells' in one of two states, and a set of rules that define the state of a cell in terms of its neighboring cells' states. For example, the CA that creates my caves counts the number of #'s around the cell of interest and if it's at least 7 then it returns a floor(.) and if there are fewer than seven but at least three walls(#) then it returns a wall. This code is based on a [tutorial][ttrl] I found online.

I'm planning to do a deep dive into this topic for the next few weeks under the guidance of Dr. Patitz in hopes of finding a project for this year. In any case, I absolutely love these little parallel computers and the surprising emergent complexity they offer.

More to come soon.

[ttrl]:		https://gamedevelopment.tutsplus.com/tutorials/generate-random-cave-levels-using-cellular-automata--gamedev-9664