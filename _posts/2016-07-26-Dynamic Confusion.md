---
author: scott
title: Dynamic Confusion
---
Greetings fellow CS Entusiasts!
Thanks for another wonderful Friday night, filled with some mysterious Cobol, a first appearance of the latest Toliver, and some more mysterious Dynamic Classification from Chapter 33 of PFPL.

Next week at the usual time and place, Friday night at Gamma Space (aka Bento Miso) at 6:30pm we will continue into the long awaited Chapter 34 on Modernized Algol.  For those keeners among us, and who is kidding who, that's everyone, there is a Modernized Algol Interpreter from Jon Sterling available [Modernized-Algol](https://github.com/jonsterling/sml-modernized-algol).  So we should be able to work through more examples than usual, and may help us get our many-flavours of PCF project off the ground.

The Chapter on Dynamic Classification proved quite interesting and the mechanism seems quite useful, especially once we hit on the use-case of a server that executes callback functions submitted by users.  In that situation if an exception is raised by the server, it becomes entirely possible that the user code could improperly catch that exception and head off in a different direction.  By defining exceptions dynamically, it makes that type of improper exception handling impossible.  That application did lead us into some interesting discussions on what types of secrets and confidentiality we could expect to handle this way, and our interpretation was that they were less secrets and more like ways of keeping the programmer from messing up, since anyone who steps outside of the system can always access the raw data however they please. 

Apologies, on missing the update last week on Fluid binding, but it was a busy week.  I felt like I learned a lot over the course of the evening as the whiteboard examples and exceptionally precise yet confusing questions helped us separate the concepts of scope and binding.  In particular, Ben's example that demonstrated how the scoping depended on lexical visibility settled a misunderstanding I had brought with me about how the scope-free dynamics worked and dann summarized the effect nicely by saying that scope-free doesn't mean that a symbol can exist free of a context, but it does mean that a symbol can be exported back into an existing context via a lambda.

Until next time,
Scott
