---
title: Genteel Types
author: scott
---

Hey everyone!

Bit of a hiatus on recaps but that hasn't slowed us down, since the last time I wrote up something we have covered chapters 23, 24, and 25 of PFPL, which all illustrate different ways of organizing your language; hybrid typing, structural typing, and type refinement respectively.

Next week will be Chapter 26 on classes and methods which I suspect is one of those topics everyone knows experientially but probably not seen presented in the PFPL way before.  We are sticking to the usual time and place, Friday 6:30pm at Bento Miso / Gamma Space.  I'd also like to demo the synesthetic numbers I've implemented in terralang, and if anyone else has something cool they'd like to show or just talk about, please bring your ideas.

Type refinement as introduced in chapter 25 is a way of resolving the ambiguous nature of the dyn type in the hybrid-dynamic language presented in chapter 23.  Since applying the same generic dyn type to all dyn classes effectively erases all information about the underlying class and forces the language to treat every dyn variable the same way; thereby unnecessarily restricting the number of programs that can be safely typed.

Refinements provide a mechanism for capturing information about the class of a dynamic type as part of a refinement of that type.  One way to think about this is that refinements represent subsets of the total class, so for instance the set of even integers is a refinement of the class of all integers.

The section on Boolean blindness seems like a very important thing to internalize, I still don't know that I fully appreciate what is happening there.  My understanding is that when handling conditional statements, if the language treats the condition as a single Boolean bit then it will not have enough contextual information to type the subsequent then and else clauses.  His resolution is to disallow the separation of testing for a type class and casting a dyn type to that class, so that the information about the type being tested is directly tied to the clauses.

All for now, see you all next week,
Scott
