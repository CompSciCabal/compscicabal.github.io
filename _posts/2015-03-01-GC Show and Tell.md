---
author: scott
---
Garbage Collector Month Wrap-up!

Friday night we had garbage collector show and tell to show our implementations and ideas for garbage collectors to close off our month of delving into garbage collector development.

Next week we will kick off our new Polymorphic month with part 1 of Cardelli and Wagner's paper, "On understanding types, data abstraction, and polymorphism" (http://phobos.ramapo.edu/%7Eldant/oop/cardelli_wegner.pdf) 6:30pm Friday night at Bento Miso. You can check out the full reading list over on the github page, https://github.com/CompSciCabal/SMRTYPRTY/wiki/Reading-Schedule.

Earlier in the month, Chris gave a talk at papers we love on teaching garbage collectors (http://www.meetup.com/Papers-We-Love-Toronto/events/219961100/) and he introduced us to an excellent environment for building garbage collectors called plai (http://docs.racket-lang.org/plai/collector.html.), built on top of Dr. racket. Chris couldn't make it out unfortunately but when working on this myself I referred to his excellent blog posts, talk notes and he also has a few collectors implemented all findable from his blog (http://learningtolearn.sndrs.ca/blog/2015-02-11-garbage-collector-notes-plus-pwl-content/).

Leo showed us his mark and sweep collector which he built in C and which he has used as part of a larger interpretor implementation he also showed us. His mark and sweep collector is checked into the github, https://github.com/CompSciCabal/SMRTYPRTY/blob/master/experiments/inaimathi/memory-management/g.c. Leo brought up a lot of interesting questions from his experience of putting this collector to use in an interpretor. For instance, how do you handle symbols? What about special symbols that are defined by the language? Do they get garbage collected the same as everything else or do you give them there own little box of memory? As just a couple of examples of issues that can arise, among others. It underlined for me just how much the plai environment must help with teaching about garbage collection, as it lets you focus on the collector aspect without worrying about how to build the interpretor at the same time.

We then spent some time going over the trio of collectors I wrote in racket, the mark and sweep, stop and copy, and then a mark and compact approach (https://github.com/CompSciCabal/SMRTYPRTY/tree/master/experiments/scott/garbage_collector/plai/tests/gc/good-collectors). These are all somewhat ancient approaches to garbage collection but seemed like the right place to start for learning about these things. Implementing them in the plai environment was rather fun and helped me understand the subtleties involved a lot better. A couple of comments about the plai environment; one it's awesome, two the heap visualizer is really cool and useful, and three the assert and test features are boss, I just wish I had used them. I found it quite satisfying to use the heap profiler in debug mode and see the GC mutating the heap step by step. In future if I try a more complex design I would definitely try to break things down into a bit smaller chunks that can be tested individually as it will likely pay off very rapidly in time savings. Debugging by using the heap profiler was cool, but I don't know that I want to depend on that for debugging again as it can be quite time consuming.

We finished off the night by discussing Dann's very interesting proposal for a concurrent garbage collector inspired by the field of vermiculture. This was really cool, though we may still be some distance away from an implementation.

See you all next week!
Scott
