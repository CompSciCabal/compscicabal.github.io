---
author: scott 
title: Recap Recap
---
Hey Team!
Friday night we met up to discuss the 'Go Meta' manifesto from Snapl 2015.  Dann had imagined this might wrap up our month of multi stage programming, but as it turns out it was more of a beginning and our one paper has exploded into a finite but large number of follow on readings.  

So next week we 'Go Meta' once more, but this time we are allocating everyone 10 mins to cover a follow up reference of interest to them from the paper, [Go Meta](http://drops.dagstuhl.de/opus/volltexte/2015/5029/pdf/19.pdf) .  Also we are having a potluck so bring along some food and we will be taking a 2 week hiatus after that before we start our next large book length commitment, Harper's Practical Foundations for Programming Languages.

This manifesto really seems primed for spurring discussion and pushing readers to explore the many references.  We tended to alternate between discussing the high level ideas in the document and trying to comb through the many motivating examples, for example the 500 line SQL compiler, or the parametrized code generator.

The authors put forward a development path that creates effective communication channels between the code that a developer writes in a high level language and the assembly code that gets generated on the other end.  Everyone of us has encountered the problems mentioned in the paper, I think because it is pretty much the standard development flow; write a first version in a high level interpreted language, then once all the kinks are worked out throw it away and write it again in a lower level language where you can have more control over performance.  Unfortunately, that often means your code loses a lot of its dynamism and makes future changes more expensive, and in addition there really is no 1 low level version that will satisfy all possible demands so often you end up with multiple versions and/or extensive parameter controls to guide the compilation.

The metaprogramming approach put forward in the paper isn't a solution to these problems, but it is a powerful tool that I think has the potential to become a very effective way to do development.  So maybe we can do away with the disjoint 2 stage development flow and create some better tools for ourselves.

Until Friday, 
Scott
