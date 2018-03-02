---
layout: post
title: Menangani Salah Ketik di Chatbot Bahasa Indonesia
date: 2018-3-2
---
That the typo simply called as misspelling.

While that the chatbot is combining messaging and AI.

Many people take less care the right spell of a word these day. (Sapul, 2016).

There will be another rule on chatbot to handle any misspelling case. (Nawaf Ali, 2014: 00).

But it would be user satisfying (TELUS International, 2015)
since not pretend to be human. (Tiwari et al, 2017)

To detect spelling case in indonesian word by using Soundex.
It will keep the first letter, so the mistaken of the word depend on first letter.

Just handle some like
tjuan
tjn
Can be known as tujuan.

The Soundex can achieved by the use of sql query. It has implemented as function. Soundex() different with sounds like query.

The result from Soundex string given still need to
String similarity measurement
Measure the similarity of word or string

the smallest distance the correct word is. Still word dictionary based. The challenge to time access and  more on less space.

Note that it just not wise if the mistaken word can be considered as one distance but then create or save any record only for it.

Can also limit the distancing as 1 distance.

Since 80% can be handled allowing one operation of four: they are deletion, insertion, replacement and transposition.
While transposition is on interest. Using only classical Levenshtein distance, it not considering transposition as 1 operation.

Damerau-Levenshtein distance knowing transposition as 1. May still the Damerau-Levenshtein not support triangle equality.

Although on a research Jaro-Winkler take being the better. Since chatbot is about natural language.

As Wikipedia says here on Damerau-Levenshtein topic.
Damerau-Levenshtein plays an important role on natural language. In natural language string are short and the number misspelling rarely exceed 2.
