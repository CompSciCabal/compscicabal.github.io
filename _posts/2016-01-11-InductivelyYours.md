---
author: scott
title: New Year's Resolutions and Other Fresh Renamings
---

Hi Everyone!
  Welcome back fellow PFPL reading group members, Friday night at Bento Miso we got caught up on Chapters 14 and 15 among other diversions.  Next Friday at 6:30pm at Bento Miso we will continue into Chapter 16.

For the uninitiated, PFPL is an acronym for Bob Harper's book, Practical Foundations of Programming Language which we have been reading since September 2015 at a rate of about a chapter a week.  We meet Friday nights, however we have an active discussion channel on slack so remote readers are welcome to join the fun.

Next week is exciting as in Chapter 16 Harper introduces us to System F, Girard's highly influential typed lambda Calculus that includes polymorphic types and is the most powerful system we have seen so far in the book. Hopefully everyone will have been able to read Chapter 16 by then and for those who were there on Friday your homework is exercise 15.1.

Last week saw us through most of Chapter 15 which covers Inductive and Coinductive types.  By adding Inductive and Coinductive types into our system we gain the ability intrinsically define infinitely large types like natural numbers.

Leo summed up the difference between Inductive and Coinductive types quite well, an inductive type starts from a single fixed starting point (e.g. zero) and then they build outwards indefinitely.  Coinductive types go in the opposite direction, you start with an infinitely large bag and then remove elements from it.

We then went through a number of fairly straightforward examples of the dynamic types on nats and conats (introduced in section 15.4) and Ben gave a ton of helpful explanation, thanks Ben!  I've started compiling some of the [examples over on GitHub](https://github.com/CompSciCabal/SMRTYPRTY/blob/master/pfpl/15-inductive-and-coinductive-examples.md).

Another topic that came up and garnered a lot of attention was what are the differences between a language that is Turing complete, and a language in which you can write an interpreter for itself.  We weren't able to resolve that question and it has been deferred until futher investigation, with some already lengthy discussion in slack.

Alrighty then,
Scott

