---
title: Ideal Hash Tries
author: scott
---
Happy New Year!
Welcome back everyone!

Friday night marked our first Cabal meeting of 2015 as well as the first meeting without sicp, though it will remain forever with us in spirit. We had a great time discussing ideal hash tries, as well as some suitable divergence towards transhumanist philosophy, quantum computing, and Asimov (Thanks Colin!).

Dann moderated our discussion of Phil Bagwell's excellent paper, Ideal Hash Tries (http://lampwww.epfl.ch/papers/idealhashtrees.pdf). This paper introduces using Array Mapped Tries (AMT) to implement a hash table interface as well as covers a variety of applications and extensions of the basic data structure.

We spent most of our time covering the basic principles by which AMTs operate, so maybe we should have started with the AMT paper. Confusingly for the non initiated the H in (Hash Array Mapped Trie) HAMT does not refer to the hashing that goes on in the AMT algorithm, but rather to the hash table interface that is implemented using the AMT. Although, this does mean we could easily come back to this paper and cover some other topics in the future. Dann also sketched out how this data structure could be used to implement persistent data structures which is an important application for HAMTs.

Clear low level implementation details are given in the paper for all aspects of the algorithm which we spent some time digesting into a more abstract representation we could understand. Over on github I've added a basic implementation of the Trie in python (https://github.com/CompSciCabal/SMRTYPRTY/blob/master/experiments/scott/Idealhashtrie/trie_v2.3.py). This implementation is not efficient, but does present the basic flow of the algorithm without implementing the efficient compressed array data structures used in each node. Implementing an AMT would require a bit more work replacing the python dicts with the bit maps and fixed size hash tables described in the paper.

Next week, we learn how to always get picked last for the baseball team, and be proud of it!
Concrete Mathematics Chapter 1.3 'The Josephus Problem' delves into the mathematical reasoning behind the Roman philosopher Josephus' brush with death in a cave near Jerusalem.

Until next week!

Scott