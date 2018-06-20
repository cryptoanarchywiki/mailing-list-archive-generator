---
layout: default
---

# 1996-09-17 - really undetectable crypto made somewhat practical

## Header Data

From: jim@suite.suite.com (Jim Miller)<br>
To: cypherpunks@toad.com<br>
Message Hash: 594bed7bdbccd8278ee005be60efef943ce21baea0eb8bbfd61133c14f923ecb<br>
Message ID: \<9609162334.AA17481@suite.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-09-17 05:24:56 UTC<br>
Raw Date: Tue, 17 Sep 1996 13:24:56 +0800<br>

## Raw message

```
{% raw  %}From: jim@suite.suite.com (Jim Miller)
Date: Tue, 17 Sep 1996 13:24:56 +0800
To: cypherpunks@toad.com
Subject: really undetectable crypto made somewhat practical
Message-ID: <9609162334.AA17481@suite.com>
MIME-Version: 1.0
Content-Type: text/plain



The primary drawback to the stego scheme I described in the previous post  
was the ratio of stego bits per message.  The scheme would only transmit  
an estimated 4 stego bits per message.  Then it occurred to me that I can  
improve the ratio by basing the scheme on the hashes or words rather than  
the hashes of entire messages.

Previous Scheme:  construct a sequence of plaintext messages such that the  
first 4 bits of the MD5 hashes of the messages combine to produce the  
cyphertext of the true stego message.  The sender would only need to send  
the plaintext messages.  The recipient would calculate the MD5 hash of  
each plaintext message, extract the first four bits from each hash, append  
them together, then decrypt the result to obtain the true stego message.

New Scheme:  First, calculate the MD5 hash of all the words in the various  
dictionary files used by the password cracker program and create a  
database containing every word and the first 4 bits of its MD5 hash.   
Given such a database, it would be possible to write a program that  
accepts as input a block of cyphertext (the stego message, encrypted),  
chunks it up in to groups of 4 bits and then, for each chunk, displays the  
words that have hashes that start with those same four bits.  The person  
running the program would select words that form meaningful sentences but  
also produce hashes that combine into the encrypted stego message.  This  
scheme would send 4 stego bits per word.

In addition to ordinary words, the database could contain names,  
misspelled words, abbreviations, words with alternate capitalization,  
slang terms, technical jargon, whatever.

Fortunately, senders and receivers don't need to synchronize word  
databases.  The recipient doesn't need to have any word database.  The  
receiver can reconstruct the hidden encrypted message simply by  
calculating the MD5 hash of each word in the plaintext message, gathering  
up the appropriate hash bits and decrypting the result.

This scheme could send more than 4 stego bits per word, but as you  
increase the number of stego bits per word (sbpw), you reduce the number  
of words that will work for a given chunk of cyphertext, making it harder  
to construct meaningful sentences (e.g. given a 40,000 word database, 4  
sbpw yields 16 word groups with approx 2500 words per group; 8 sbpw yields  
256 word groups with approx 156 words per group.  8 sbpw would probably  
not work well).

Would this scheme work?  It works in the sense that you can use it to send  
arbitrary encrypted messages through channels that don't allow anything  
but human-readable plaintext messages, but does it do so in an  
undetectable manner?  I think so, but I don't know for sure.

Jim_Miller@suite.com




{% endraw %}
```

## Thread

+ Return to [September 1996](/archive/1996/09)

+ 1996-09-17 (Tue, 17 Sep 1996 13:24:56 +0800) - really undetectable crypto made somewhat practical - _jim@suite.suite.com (Jim Miller)_

