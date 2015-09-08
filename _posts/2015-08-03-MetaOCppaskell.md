---
author: scott 
title: MetaOCppaskell
---

Hey everyone, 
  Reporting in from our Friday night session with Leo giving a demo of his Lisp DSL implementation and going over Taha's comparison of implementing a DSL in 3 different languages, MetaOCaml, Template Haskell, and C++ Templates.  
  
  Next week is more MetaOCaml and we will cover Oleg Kiselyov's paper "The Design and implementation of BER MetaOCaml", in the usual time and place, Friday at  6:30pm at Bento Miso.
  
  Also everyone who is available, on Wednesday at 6:30 Ben is giving the monthly papers we love talk at shopify, <a href="http://www.meetup.com/Papers-We-Love-Toronto/events/224152792/">meetup link</a> on programming with Algebraic Effects which he already started dropping some interesting facts from on Friday.
  
  As for Friday, the discussion of Taha's paper devolved somewhat into lamenting unresolved emotional issues stemming from overexposure to generic programming in C++. Since we were already familiar with the gentler MetaOCaml papers the material was already fairly comfortable for us which gave us lots of time for Leo to demo his Lisp DSL implementation, which in a cabal first was projected onto the big screen!  With all this talk of metaprogramming, Lisp was certain to make an appearance sooner or later, since you know metaprogramming is kind of a thing in Lisp...
  
  His code is available at [his github](https://github.com/CompSciCabal/SMRTYPRTY/blob/master/experiments/inaimathi/dsl-gen.lisp).  It was neat to see some of the strengths and weaknesses of the different implementations, as some of the approaches Leo used involved a few subtleties involving the Lisp macro system.  Also, really cool was when he just quickly dropped down into inspect mode and drilled down to the actual assembly code that had been generated for his function, right from the interpreter!  That is so cool, I had no idea you could do that.
  
 Thanks again everyone,
 Until Next Time,
  Scott
