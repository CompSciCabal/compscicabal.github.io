---
author: scott
---
Friday night marked the latest installment of Cardelli and Wegner's paper, "On Understanding Types, Data Abstraction, and Polymorphism."

Next week will be the 4th and final chapter of Cardelli and Wegner, taking place in the usual time and place, Friday night at 6:30pm at Bento Miso.

This week covered type classification, and Universal and Existential quantification, sections 3, 4, and the start of 5. They describe their approach to types quite succinctly in the title of section 3, "Types are sets of values." In that context, the programmer or language designer then has the task of identifying which out of the infinite sets available are interesting to use, and what subset relations to make use of. An advantage of this approach is that monomorphic, polymorphic, or untyped languages may all be described using the same type model.

Universal and existential quantification, I'm having a harder time wrapping my head around, but I am beginning to suspect that associating universal quantification with parametric polymorphism and existential quantification with abstract interfaces and information hiding is the short form description in terms I'm more comfortable with. Seeing how they are able to use type quantification to build the other more complex concepts into their system is a continuous and surprising journey. I'm finding it fascinating to see them build up their fun language, often as a programmer you are simply handed a language to use fully formed and you have to adjust to the language's idiosyncrasies without really understanding what constraints went into the choices of designing that language. Here the language is as simple as possible and all of the additional concepts and ideas are being layered on top without additional language constructs being introduced.

Looking forward to next week where we will try to cover the rest of the paper!
Scott?