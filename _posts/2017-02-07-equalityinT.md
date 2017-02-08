---
title: Intuitive T
author: scott
---

Hey everyone!
Friday night we finished off the rest of PFPL46: Equational Reasoning in System T, digging into the definitions some more and trying to understand how observational and logical equivalence complement each other.

Next week the group will continue with PFPL47: Equational Reasoning in PCF, otherwise known as "Coming to Grips with Fix".  The time and place will be the same as usual, Gamma Space at 6:30pm on Friday.  Unfortunately I won't be making it for the remainder of the book as I'm away on business, but will be trying to keep up on the reading and over slack.

I really enjoyed the discussion this week and feel like it helped me understand the concepts of observational and logical equivalence.  In some sense, they are intuitive in that we want to classify expressions into equivalence classes where expressions that always give the same result can be considered "equal".  

- Observational equivalence expresses this in a top-down kind of way, it says that for all possible programs with holes in them, two expressions are indistinguishable from one another based on the program output.
- Logical equivalence comes from the other direction, we start with some simple equivalences and then build up a full expression.  The surprising part is that they coincide!

This led us to the  following high level interpretation of this chapter; observational equivalence  is a highly desirable property of a language, but it's hard to work with.  How does one do computations over all possible programs?  Logical equivalence at first sight seems less powerful, but is much easier to work with.  By the happy coincidence that they coincide we can work out results that talk about observational equivalence while working only with logical equivalence relations.

This somewhat involved and technical work with the equivalences gives us at the end of the chapter our seemingly intuitive laws of equality in system T, but on a sound surfboard footing.  

Induction anyone?
Til next time,
Scott
