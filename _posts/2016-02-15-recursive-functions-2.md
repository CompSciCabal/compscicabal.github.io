---
author: scott
title: Turns out the base case is Pete
---
Hi everyone!
  In spite of the recent flurry of gravity waves, Friday night saw us return to recursive functions in chapter 19 and Pete return to the fold; welcome back we missed you :)
  This was an evening full of interesting digressions, which is more or less as planned since we decided to spend another week on this chapter because of the many digression worthy topics.
  
  Next week we will move to chapter 20: System FPC of Recursive Types, meeting at the usual time and place 6:30pm Friday at Bento Miso.
  
  I'm fairly certain we raised more questions than we resolved, turns out Church's Law, partial recursive functions, and Gödel numbering get one into fairly deep waters.  Jotting down a few that I remember, feel free to add to the post with others that I may have forgotten.
  
  - If I write an interpreter for language L in language L, is that sufficient to show L is universal?
  - Is there an expressive ordering hierarchy among total languages?  E.g. Something like having a total language T0 in which you can write an interpreter for another total language T1, which in turn can be used to write an interpreter for T2, and so on.
  - Clarification around the distinction between partial functions and partial recursive functions still seems necessary.
  - Can I choose an order of maximal complexity, e.g. n^2 and then find a system such that only total programs up to that complexity may be written?  This could be viewed as a variant on a language with primitive recursion, but no higher order functions.
  - How does Church's law relate to the breakdown of languages in the lambda cube?
  
  Thanks everyone for the mind bending questions, I may be recovering from this one for a while to come,
  Scott
