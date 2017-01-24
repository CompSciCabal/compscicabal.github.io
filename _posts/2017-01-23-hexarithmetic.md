---
author: scott
title: Counting in Hex
---

#Counting in hex
We all know how to count to 10; why, because we have ten fingers!  So passé!  Now that our fingers can touch keyboards and numpads have finally fallen out of fashion we should be counting to 16.  
##Naming
One of the first things I realized is that you can't repurpose "ten" the word to refer to `10` the numerals in base 16, this quickly gets very confusing as the concept of 10 is so deeply ingrained.  It's a lot easier if 10 remains ten, so that if you happen to slip back into base 10 to do a calculation the meanings of words don't depend on context.  This then means we need new names for common sequences that clearly identify that we are in base 16.  At first I replaced `t` everywhere with `h` or `hex` or `x`, but it didn't always work, so eventually I made the transition of `x` to `z` and then it works better and is pretty easy to pronounce and is more than a little hilarious and makes you sound a bit like Bilbo saying how old he is.  This swap will give you the following list of terms:

- `10`: zen
- `11`: zeleven
- `12`: zwelve
- the teens become zeens, I.e thirzeen, fourzeen,  up to eezeen, effzeen
 - `13`: thirzeen 
 - `1F`: effzeen
- double digits are twenzy, thirzy, ..., eezy, effzy
 - `31`: thirzy one
 - `3D`: thirzy dee
- `100`: zundred 
 - `152`: zundred and fifzy two
 - `7DF`: seven zundred and deezy eff
- `1,000`: zousand 
- `1,000,000`: milzion 
- `1,000,000,000`: bilzion 
- `1,000,000,000,000`: trilzion 

## Multiplying
Now we get to learn our number tables all over again, many of the simple tricks we learn in high school for base ten carry over directly since they are generic properties of any position based number representation.

- `10`: zen times anything just shifts the number over and adds a zero, same as multiplying by ten in base ten
- `F`: eff times any single digit number has a similar sequence to the nine times table in base ten, first digit counts up, second digit counts down.
- `8`: eight works like five does in base 10, alternating final digit of 8 or 0
- `4`: gets a nice pattern you don't get in base ten, final digit alternating between 0, 4, 8, C
- `2`: has the same even number pattern as in base ten: final digit of 0, 2, 4, 6, 8, A, C, E
- `F`: gets a rule a bit like the sum of digits must be divisible by 3 rule (this falls out of modulo arithmetic).

Since, I've often used hex for bit patterns, I thought multiplying by 2 might be easier if you think of it in base 2, and that does  seem to be the case,

- `E,25F * 2 = 1C,4BE`

but still won't help you calculate at speed in your head, you need to memorize some tables.

##Common big numbers

- 1024, KB: `400`, four zundred
- 1024^2, MB: `100,000`, zundred zousand
- 1024^3, GB: `40,000,000`, forzy milzion 
