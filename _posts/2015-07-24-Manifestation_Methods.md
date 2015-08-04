---
author: dann 
title: Manifestation Methods
---

Hello, computer people!

We had a perfectly lovely meeting on Friday, covering part two of part two of A Gentle Introduction to Multi-stage Programming. We started by revisiting Leo's question from part one of part one of AGIMP, on the advantages brought by performing a CPS transformation on our exception handling interpreter. We made it further up the hill this time, but got a bit bogged down trying to understand precisely when evaluation of the various staged components occurs, how often that evaluation occurs, and how those answers impact the overall performance of the evaluation. 

The primary focus of this pair of papers is interpreters, which turn out to be quite a bit different than regular programs when it comes to optimizations. If a regular program isn't fast enough in Ruby, you rewrite the slow parts in C. But an interpreter could be orders of magnitude slower than desired -- rewriting the interpreter in C isn't likely to help in that case. Instead you need to write a compiler, which is an entirely different type program than the interpreter you'd like to speed up. Multi-stage programming is a way to speed up programs in general, but in particular it can speed up interpreters so they have compiler-like performance, which is really pretty fantastic. 

After the break we spent some time simplifying and debugging Pete's Haskell-based JS interpreter, which doesn't use multi-stage programming but did reveal an interesting quirk in Haskell's instance resolution procedure, which we initially thought was a bug in the FlexibleInstances extension due to the method of manifestation. Perhaps this coming Friday we'll rewrite it in MetaOCaml, and stage a race between them. 

Happy coding!

Dann
