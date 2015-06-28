---
author: dann
---
Happy Monday, Computer Scientist!

We had a great meeting last Friday, with Pete leading the charge on unpacking Milner's Exp language's semantics, its types, and their semantics (Sections 3.1 and 3.4 of A Theory of Type Polymorphism in Programming). We came to an understanding of Milner's syntax for this language and metalanguage*. We saw a roadmap for the paper, learned about lattices and complete partial orders, neatly skirted the topics of domain theory and retracts (though we may return to those later), talked about the type of wrong and the wrongness of types and how well-typed programs never go wrong, unless they fall in with a bad crowd and take up smoking and jitterbugging.

For this coming Friday we'll be reading sections 3.5, 3.6, and 3.7. It's not a lot of material, but it's quite dense. 3.5 covers the connection between expression in the Exp language from 3.1 and expression in the type language of 3.4. Section 3.6 is about substitutions, which are kind of the type language equivalent of lambda calculus reductions (or not). Then 3.7 is a formal proof that Well-Typed Expressions in this language Do Not Go Wrong. We'll dive as deep as we can in to the proof, but with an eye for coming away with an understanding of formal proofs in general and inductive proofs in particular, choosing breadth over depth if time gets short.

We're wading in to some heady waters, but like Dante's Virgil we have some excellent guides and guideposts along the way. Be sure to check out Pete's study notes as you make your way through this week's sections.

Have an amazing week!

Dann
* Perhaps a begrudging understanding, in that latter case*.
* Begrudging for me, at least*.
* Okay, fine, I still don't understand. The syntax appears intentionally obfuscatory and makes me act completely irrationally. Sorry, I get a little verklempt just thinking of it.