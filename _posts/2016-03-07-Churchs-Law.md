---
title: Church's and Untyped Lambda Calculus
author: scott
---
Hi Everyone,
  Last Friday we pondered Church's Law and Scott's theorem, both found in the untyped lambda calculus chapter (PFPL 21).  It was also the first split theory/practice meeting and I think this worked well and hope to continue this in the future.  It was not however the first time that the structure of the universe came up in conversation...  nor do I expect it to be the last :)
  
  Next Friday we are again dividing the section to cover PFPL 22, Dynamic Typing and again allocating half then time to discuss implementations or other questions that come up.
  
  This was a wide-ranging discussion, the statement of Church's Law (Normally referred to as the Church Turing Thesis), stimulated a lot of interesting tangents into what types of systems can be captured by computable functions over the natural numbers and conversely what type of systems can be used to implement such a computation system.  At this point I think we can safely say, the outlook is unclear, though placing a computational hypothesis into the realm of a scientific theory is a tantalizing possibility.
  
  In slightly more grounded concepts, we found that when unpacking the Y-combinator  some of the properties we had observed of the fix point operator in the self language from PFPL 20.3 no longer held in the untyped lambda calculus version.  For instance, last week we found that applying the fix operator to a number would give back the number itself, so in the self language, `fix(5) = 5`, however this is no longer the case, and the fixed point of the church encoding of 5 will be whatever `Y(5)` gives you.  Similarly, unpacking `Y(succ)` shows that the fixed point of `succ` is definitely not `succ` and is in fact quite a complex expression, despite the fact that `succ` is not a recursive function.  I think this may be a manifestation of the `all elements have the recursive type` property of the untyped lambda calculus that Harper is developing in this chapter.  

Taylor also showed us the Turing fixed point combinator which though different from the more famous Y combinator seems to share many properties with it.  One thing that wasn't clear to me was whether the Turing and Y combinators would give you the same or different fixed points?

When we moved into the practical section, Ben gave us a lovely introduction to using the twelf environment to define and proof properties of our languages in a syntax that is very similar to the presentation in the book.  This seems like a very attractive tool and I'm looking forward to trying it out myself.  Jim has also gotten the cheat sheet into quite a complete state, and it looks really useful for being able to quickly identify the many different syntaxes used in the book.

All in all, a most excellent evening, thanks everyone and looking forward to next time,
Scott
