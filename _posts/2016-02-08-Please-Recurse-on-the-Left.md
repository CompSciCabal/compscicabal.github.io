---
author: scott
title: (PFPL (PFPL (PFPL ...
---
Hey Everyone, 
  Thanks for another stimulating session on Friday, starting our foray into General Recursion and as it turns out Chapter 19 packs in so much that we will continue on with it next week too and discuss the many intriguing comments in the second half of the chapter.

  The meeting next week will be at the same time and place as usual, 6:30pm Friday at Bento Miso and will be starting from section 19.3.

Since the last update we have covered a fair bit of ground in the book, Girard's System F in 16, Abstract Types in 17, and Higher Kinds in 18.  Unfortunately I've been a bit remiss in making notes so I don't remember too much.  I was spending most of normal PFPL time instead reading about RPython and preparing for the Paper's We Love Toronto talk on [Meta-Tracing JITs](http://www.meetup.com/Papers-We-Love-Toronto/events/228164451/) which was a lot of fun.  

In Chapters 16 and 17 we devoted significant discussion to comparing the presentation with the one we had seen in Cardelli and Wegner's heavily cited paper, "On Understanding Types, Data Abstraction, and Polymorphism."  Higher Kinds in chapter 18, I don't feel like I understand deeply, however in many applications you can see how they are used, so they feel like an eminently practical idea.

This week we went through the statics and dynamics of the language PCF introduced in 19.  PCF has general recursion and so is the first language we have met that is not total, i.e. that does not contain a proof of its termination in the code.   The presentation in the first part of the chapter presents the fixed point operator in a mathematical way which was pleasantly familiar from taking functional analysis courses back in University.  Once we started going through it though, I found the comparison perhaps a bit misleading since what we are using the fix operator for here is very different from many of the tasks you might do with a fixed point in math class, e.g. find a fixed point, or prove the dimensionality of a null space.

Instead the fixed point operator here is being used to allow us to reference the definition of a function within the definition of that function.  Ben and Leo did a nice job illustrating with examples how fix and define are effectively equivalent in enabling general recursion.  I've encountered the problem before, if you try using different data structures for the definition of the environment in a simple scheme-like interpreter you can find yourself missing a fix operator.  

Next week I think will stir some interesting discussion as there are more than a few brain warping statements in the latter half of the chapter.
See you all there,
Scott

