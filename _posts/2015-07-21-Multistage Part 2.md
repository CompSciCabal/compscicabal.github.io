---
title: Multistage Meta Programming Part 2
author: scott 
---
Hey everyone!
  Thanks for some stimulating discussion Friday night, we spent the night discussing [Gentle Introduction to multi stage programming part 2](http://www.cs.rice.edu/~taha/publications/journal/gttse07.pdf).  
  
  Next week we are covering the second half of the paper, meeting at the usual time and place 6:30pm Friday at Bento Miso.
  
  Leo spent some time elaborating on his point that the eval 6 in the previous paper was benefitting not so much from the  various optimization a as from raising an exception instead of using Maybes everywhere, to settle this Pete fired up the MetaOCaml interpreter and patched in the modification and we compared the generated source code.  At a glance they look similar, but we couldn't quite decide if there was some subtle but important difference to the different generated code objects.
  
  We seemed to pick up on a lot of the same comments in the text, for instance the comment about what if Haskell had been written with S expression syntax?  Ben quipped, "Then they never would have found the Curry-Howard correspondence."  He is joking of course, maybe they would have anyway, but it started a rather wide ranging discussion on how syntax influences thought, touching upon a variety of languages as well as the distinctions between Newton's calculus of fluxions syntax and Leibniz' in many ways superior calculus of infinitesimals.

It's intriguing as humans that we tend to be quite aware of what new powers our tools give us but rarely do we see as clearly how our tools in turn shape us.
  
  Until next time, 
  Scott
