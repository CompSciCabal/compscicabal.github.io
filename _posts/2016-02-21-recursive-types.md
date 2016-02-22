---
author: scott
title: System FPC for Recursive Types
---
Hey Team!
Thanks for another great meeting, we had a full crew for our first crack at Chapter 20 and System FPC for recursive types.  

Next week at the usual time and place (Friday @ 6:30 pm at Bento Miso) we will have a dual session, first we will continue with the rest of chapter 20 and then we will move into a meta session where we plan out what to do next.  There seems to be some interest, myself included in spending some time to do some more hands on implementations of things we have been learning in PFPL.  So bring your ideas next week!

I found this chapter quite challenging, and still isn't sitting well, but I think that may be more a reflection of a lot of ideas that have been being built up over the last few chapters never being fully digested.  We started by discussing Dann's resolution to the problem Pete posed last week of could you give an upper complexity bound and be guaranteed to always find a language that had it as an upper bound on programs that could be written in it. 

We then went through the number of intriguing but difficult to understand statements in the introduction and I think we just had to move on, Ben pointed out that perhaps we didn't have the necessary machinery to understand it just yet.  I think the most useful for me was the concrete examples we worked out on the board (great idea Pete), these helped us explore the meaning of the examples for natural numbers and lists that he gives in the text.  An interesting question that came out of this was how does one specify the type of arbitrarily long but finite lists?  

Harper discusses at length the greater expressive power of eager languages in comparison to lazy, by going through some examples and comparing with Haskell, I'm starting to get at what he is trying to say, though I can't say I fully appreciate why it is so important.

We ended the night going through the self referencing language examples but ran out of time to discuss state.  Looking at the self referencing it felt like maybe some examples in a language with a bit more normalcy to it, e.g. with plus and numbers might help to clarify what is going on there.

See you all next week,
Scott
