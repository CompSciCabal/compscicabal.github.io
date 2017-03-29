---
author: inaimathi
title: PFPL In Memoriam
---
This entry has been shamelessly cross-posted from [langnostic](http://langnostic.inaimathi.ca/posts/pfpl-in-memoriam).

For the past year or so, the [Toronto Comp Sci Cabal](http://compscicabal.github.io/) has been reading a book called [Practical Foundations of Programming Languages](https://www.cs.cmu.edu/~rwh/pfpl/2nded.pdf)(PFPL). And the sheer idea density in this thing was giving me enough fodder to chew over and blog about for something like a month after each reading. The trouble is, we met to discuss and read the next section about once a week, so chewing and blogging time has been getting very seriously truncated on a consistent basis. The end result of this will _eventually_ be a series of posts, each focusing on trying to understand a single topic we covered, but I won't embark on that journey today.

This past Friday, we held the concluding meeting of the reading of that book. It was pretty awesome. We got the entire group back together, and were joined by [Bob Harper](https://existentialtype.wordpress.com/) by video. Even though [we'd met him before](http://langnostic.inaimathi.ca/posts/arbitrary-update-5892#the-toronto-computer-science-reading-group-meets-bob-harper), it was nice to talk to him once we'd finished reading his work.

The conversation ranged from type theory, to language design, to the current state of programming as a discipline. The definite highlight for me was finally getting to thank him for explaining some of the things that get vaguely and inconclusively discussed in the comment sections of [his blog](https://existentialtype.wordpress.com/). The big ones are

- the distinction between Concurrency, Parallelism and Distribution, which typically get conflated in general programming conversation, and are covered separately in PFPL chapters 37 through 41.
- the idea that dynamically typed languaes are subsets of statically typed languages, which is something that seems deeply counter-intuitive from the perspective of most indusutry programmers. Bob mentioned that he's in a very small minority of people that actually understand this, so I don't feel bad for needing convincing. This one is covered in chapters 21 through 23.

Those _are_ highlights, but they're not even remotely the only ideas worth exploring in the book. In Harper's own mind, some[^he-also-mentioned] of the highlights of the tome are

- *Dynamic Dispatch*, covered in chapters 26 and 27, which defines and explains the entirety of the object oriented programming paradigm in a typed context
- *Variables are not Assignables*, covered in chapter 35. This is a conflation that most current languages accept, to the point that mainstream thought essentially makes them equivalent. I won't try to explain the concept here, because it's subtle and needs enough examples that it could be a blog-post on its own. The thumbnail is that a variable should be immutable; it's a name for a value, not a name for a box where you might put a value.
- *Exceptions are Shared Secrets*, covered in 33 (as well as [one of Bob's blog posts](https://existentialtype.wordpress.com/2012/12/03/exceptions-are-shared-secrets/)), which covers an implementation of exceptions that falis to fall into the typical pitfall of non-compositional handlers by making sure that exception classes are created at runtime. I'm honestly not sure about the general utility of this one, but it does seem like an interesting approach.

[^he-also-mentioned]: He also mentioned that he half considered re-writing the whole thing on the basis of Concurrency and Dynamic Classification. Which are apparently the two features you need in order to implement the rest of everything laid out in the book. I haven't _tried_ to do this, but it does seem plausible though difficult.

As that light sprinkling of topics should show you, [this book](https://www.cs.cmu.edu/~rwh/pfpl/2nded.pdf) is a comprehensive treatment of the art and science of programming language theory and design, from a perspective that isn't exactly mainstream in the industry at the moment. Despite all the bitching and silence, I thoroughly recommend reading it. Especially if you think you couldn't handle it at the moment. Because it will start you from the very basics of proofs, and take you to the height of building solid systems. Because it will challenge many notions that may have become intuitive, but are nevertheless wrong once you look at them closely. Because it will very probably force your brain through the wringer, and enlighten you as [few other tomes](https://mitpress.mit.edu/sicp/) can.

For our next book, Bob suggests we pick up [Reynolds' Theories of Programming Languages](https://www.amazon.ca/Theories-Programming-Languages-Author-Reynolds/dp/B010BEQ4EA?keywords=theories+of+programming+languages), which we very well may do. However, for the moment we're gearing up to start on [some interesting papers](https://github.com/CompSciCabal/SMRTYPRTY/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc), right after a short and well-earned rest.
