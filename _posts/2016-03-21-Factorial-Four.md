---
author: scott
title: My Factorial is Bigger than Four's
---

Hi Everyone, 

Double Recap for the last 2 weeks, so a few things have happened, but I'll get to that.

Next week Good Friday there will be no meeting as most people are away, we will reconvene the following week, Friday April 1st, 6:30PM at Bento Miso.  Since many people were away for PFPL 22 this week, topics will be open to anything from PFPL 22 or 23 and all projects welcome.  Dann also suggested discussing other people's projects that you have found is also fair game and I agree.  See you all then!  

Two weeks back we covered PFPL 21.4 'Untyped means Uni-typed' which evolved into a lot of discussion around dynamic and static typing and what do they really mean.  Taylor also pointed us at Harper's [blog post on the topic](https://existentialtype.wordpress.com/2011/03/19/dynamic-languages-are-static-languages/).  Later, Pete demoed his really really cool [System T Interpreter in the browser](https://github.com/pbevin/primrec); though he kept trying to say it wasn't cool, but this of course is a patent lie not to be believed.  I encourage you all to try and compute the largest factorial you can without crashing your browser, mine bombs out pretty quickly once memory gets over 600MB of memory; you could use his decimal number optimization but where's the fun in that.  Also Jim's Cheatsheet is looking great and should be a great resource for future readers, [Jim's Cheatsheet](https://github.com/CompSciCabal/SMRTYPRTY/blob/master/pfpl/cheatsheet.pdf).

This last Friday we read through PFPL 22 'Dynamic Typing' which means Lisp!  Harper provides the full dynamics rules for DPCF and there are some interesting things lurking in these rules.  One thing that popped out to me was that no where in the rules can you specify something like, 'this function expects an int', which is normally how one thinks about "typing" a function in a dynamic language, instead the error will pop out later.  

After that Harper goes into great detail on all the problems with dynamic languages.  A lot of these seemed quite familiar, as they often come up in practice in many different languages; e.g. The difficulty of noticing a malformed list in Scheme, or the requirement to repeatedly type check the same argument over again in recursive calls.  Jim had some interesting ideas on how you could build a system that could do remove the repeated type checking, but my suspicion is that such a system would no longer be able to give the same dynamics rules as DPCF.

Near the end of the chapter and in the exercises, things get distinctly practical in nature, and I enjoyed going over the different approaches to implementing multi argument or multi return value functions.  Leo had lots of great examples of different approaches taken by different languages, even a quick example for me of using pattern matching on the number and type of return values since apparently Haskell's read function does this.

All for now, see you all after Easter,
Scott


