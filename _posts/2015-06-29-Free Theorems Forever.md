---
author: scott 
---
Friday Night Recap!
Thanks for a fantastic evening everyone!  We spent our time going over a variety of Free Theorems from Wadler's paper and some examples of their use.  So though we didn't fully penetrate the details of section 5 and 6, I found this discussion of examples and the consequences of the various theorems highly enlightening.  Again a big thanks to Pete, who I think can safely hold the title of resident Wadler guru :).

This Friday night we meet again at the usual time and place (Bento Miso at 6:30pm) we will be starting a new paper and a new month, "Miranda ML MetaML MetaMetaML and MegaMetaML", beginning with the paper, "How to make ad-hoc polymorphism less ad-hoc", by our dear old friend Philip Wadler [adhocminus](http://people.csail.mit.edu/dnj/teaching/6898/papers/wadler88.pdf "The paper").

We first looked at a fold over cons with a plus 2 map and we worked out what the functions had to be on the other side of the equation,
`map (+2) . fold (:) [] = fold (:) [] . map (+2)`
This says that you can either add 2 to each value and then cons them into a new list, or you can cons them into a list and then add 2.  This type of transformation can be combined with map fusion and applied automatically by a compiler to transform inefficient code into something more efficient.  For instance in the two equivalent expressions, 
`map (+2) . fold (:) [] . map (*3) = fold (:) [] . map (+2) . map (*3)`
the left hand side will have to traverse the data twice, while on the right hand side only once.  This is because of the map after the fold which makes it wait until the new list is constructed before proceeding.

This was one of a few different examples, we also looked into the fold fusion law which is related but more confusing somehow.  Pete brought up a fascinating example where the fold plus map law can theoretically be applied even if the g function is something like sha1, making the other side of the equation difficult (impossible?) to compute, 
`sha1 . fold ++ u = fold ++' u' . map a`
Where here ++ is concatenation and u is a string, and the expression accepts as input a list of strings.  The problem is then what is the function a?  And what is this other concatenation operator ++'?  We know you can't compute the sha1 piecewise, so it's quite unclear what these operators would be or how to write them down.  

We also went through polymorphic equality in section 3.4 in some detail as it is quite different from the other laws, what he is describing is close to Haskell type classes.  It's really quite an interesting result,  it shows that for equality we can't have a fully parametric function, instead we need to restrict to a set of types related by the function in a one to one way, so for instance strings and integers with the function strlen will have problems since all the strings of the same length would seem equal to each other.  The type classes approach lets us keep using our Free theorems by restricting the scope of the parametricity, so no longer is the function fully parametric but only over some subset of the types satisfying a given set of conditions. 

See you all next week,
Scott
