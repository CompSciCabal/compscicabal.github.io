---
title: Self Enlightenment
author: scott
---

Hi everyone!
Thanks for a very interesting session on Friday finishing up PFPL 20 on recursive types!  

Maybe it makes sense that a session on self reference started with all of us telling war stories of our first paid programming gigs :).  As we learned though, self reference is not narcissistic at all but rather a fundamental building block of programming languages and as a bonus if you hold "self" up to a mirror, "fles" is rarely lethal.

Next week we are changing gears and splitting the session into "practical" and "theory" (impractical?) parts.  One half will be discussions on the untyped lambda calculus from PFPL 21 and the other half is open ended discussion of any implementations of languages or exercises from or relating to the book.

We worked out some examples on the board using the self reference language found in section 20.3.  For myself this was very helpful and I think more concretely pinned down what the fix operator is doing.  I think one way of looking at this section is that it is providing the details of how to implement "recursive functions" in a language.  Often we use this feature in other languages but don't always think about what has to happen underneath the hood to make it work.  I found later reviewing the additional examples in chapter 7 "Recursive Functions" from Harper's SML tutorial (http://www.cs.cmu.edu/~rwh/smlbook/) helped ground the operation of the fix operator in some concrete code examples.  We also looked at how recursive values are perfectly normal in a lazy language but require the insertion of a delay or thunk operation in an eager language.

We ended up not leaving as much time for the origin of state section 20.4 but still got a poorly drawn RS latch on the board.  Instead of probing into latches we instead discussed what "state" was in this context, in particular in this language we don't have truly mutable state so instead you get larger expression trees that record their history and encode some notion of "time" into a discrete sequence of steps through that tree.  Having a discrete notion of time like this makes resolving the zen koan, "What time is it between the 15th and the 16th day of the month?", trivial since it is obviously not a time at all, but rather a state transition.  

If only enlightenment was that easy,
Scott
 
 
