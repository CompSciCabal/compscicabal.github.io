---
title: Josephus Problem
author: scott
---
Friday night was the exciting round 2 of Cabal for 2015. We ventured forth, coloured pens in hand, into the realm of mathematical problem solving and the Josephus problem from Chapter 1.3 of Concrete Mathematics. Inspired by the getting your hands dirty approach taken in the text, we worked through the problem together, tackling a few different variations and related ideas with varying degrees of success, and enjoying ourselves and learning a few things in the process.

Next Friday, January 23 at 6:30pm we will back at Bento Miso and Leo will be moderating the discussion of the paper "Open, extensible object models" ( http://piumarta.com/software/cola/objmodel2.pdf ).

The Josephus problem for those unfamiliar with it is actually quite grim, it concerns a group of people in a circle under desperate circumstances who have decided to collectively commit suicide. They decide to do so by going around the circle and killing every third person until only one person is alive. Yikes! Josephus finds himself in this circle but has no desire to end his life, so he has to work out where to stand in the circle in order to survive.

One of the most interesting aspects of the chapter is that in the text, they follow a quite refreshing approach to introducing their results. Rather, than simply state the problem and the answer, they instead take us along on their problem solving process, first deciding on the problem to try and solve, making tables to look for patterns, trying out various hypothesis, and using induction to prove them once they have some degree of confidence in the result. In so doing we see several other approaches to the problem, some more amenable to programming the result into a computer others nicer for people to understand.

One thing we noticed about the text, was that after introducing the every 3rd person problem, they immediately switch to every 2nd person without any discussion of why and continue to work out the mathematics for that similar problem. We decided to follow their problem solving approach, but target the every 3rd person case right from the outset. We used a variety of methods to work things through; coloured pen and paper, Dann coded up a solver quickly, and we used these tools to explore some of the different variations on the problem introduced in the exercises. Hopefully, we will get some of this stuff up onto github to save for posterity.

Until next time,
Scott

p.s. Dann has included some code he did to brute force things: https://raw.githubusercontent.com/CompSciCabal/SMRTYPRTY/master/experiments/dann/josephus.js