---
author: scott
title: A Few Good Kinds
---


Hello fellow Cabalers!

Thanks for an insightful intro to higher kinds on Friday, we were ostensibly reading chapter 43 on Singleton Kinds, but we spent a lot of time on Chapter 18 on Higher Kinds as well.  The refresher was welcome since 25 chapters is a long time to wait for an encore.  

Next week we continue with chapter 44, which is a big one, type abstractions and type classes.  Meeting as usual on Friday at 6:30pm at Bento Miso/Gamma Space.

The terminology and interplay between Kinds and types provided us with a vast trove of confusion, but in spite of this I felt like I learned some things.  The first was simply why do we have these kinds in the first place, why not just more types?  

This can be motivated by the desire to express a concept independent of the underlying data type, we can employ type constructors to make new type out of old, e.g. a list data structure, `list<T>` should work for any element type `T`.  This is a pretty common concept that people use quite frequently in many languages, however it raises the question what is a `list<>` before the `T` has been supplied?   Since a type constructor is not a type instead we need a new concept, hence Kinds.

Type constructors and type abstraction are important for providing polymorphic functions or data structures, like the list above, and also for modularity and packaging of code.  Since we saw last week that an API is a type definition selected as a hard boundary between sections of otherwise independent code, type abstraction is important as it lets you supply implementations separate from the API proper.

Singleton Kinds introduced in 43 are a bit harder to motivate, but what they provide us with is a means of giving an identity to a Kind such that we can keep information about it with us to do type-checking even through type abstraction boundaries.  The full import of this is still a bit hazy to me, but I think this is important for the packaging and module approaches we will look at in upcoming chapters.

Until next time,
Scott

p.s. It turns out you don't bind types to type constructors in the same way as variables,  so 

>Ben: You don't bind it, but kind it

>Leo: Be kind, don't bind
