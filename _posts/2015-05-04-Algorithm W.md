---
author: scott
---
Hey everyone,
Thanks for what was for me at least a quite enlightening discussion on Friday, Pete continued guiding the reins of our exploration of Milner's type theory paper. I very much appreciated the extended recap discussion of sections 3.2 and 3.3, as I had missed the previous week's meeting, and in my own reading I definitely missed a number of important concepts, so thanks all of you!

Next Friday we will meet at Sud Forno at 6:30pm and try to get through the rest of the paper, section 3.7 and onwards. This will cover Milner's Algorithm W which Ben has graciously challenged us all to implement, and to this end Pete has provided a text summary of the algorithm, https://github.com/pbevin/milner-type-poly/blob/master/algw.txt .

Section 3.4 and 3.5 that we discussed on Friday stepped us out of the semantic equation realm of section 3.1 and introduced the definitions for a system of types and a system of rules on how to use those types. Though all of the rules are defined quite clearly, for a neophyte some of the consequences of them are not immediately obvious. Though Milner develops many of these ideas with examples, having a group to discuss them with seemed quite valuable here. For instance, the differences between how lambdas and fix statements are typed and how let statements are typed is of profound importance, and we spent quite a bit of time discussing the implications of typing these statements on some examples that might run into problems if they were typed differently.

Throughout the discussion Friday having access to the Haskell version of the rules that Pete has developed was invaluable, https://github.com/pbevin/milner-type-poly/tree/master/src and now I notice that Pete has already started taking up Bens Algorithm W challenge, go Pete!

I feel very much like I am still trying to digest this material, I think I have taken a few bites but the chunks of knowledge are still floating around and need time to settle in. For instance, something I missed completely in my own reading was that what Milner identifies as Semantic equations over domains in section 3.1 are an entirely different concept than types and type relations, though they look similar at the surface level. This I find difficult as it is hard to even talk about the relations without calling things types or having types, but in the semantic realm we don't have types, just domains. I still don't quite understand what this semantic theory gives us and why we couldn't start talking about types right away

All for now, See you all Friday!
Scott?