---
layout: default
---

# 1996-04-13 - Re: Entropy Estimator

## Header Data

From: tcmay<span>@</span>got.net (Timothy C. May)<br>
To: cypherpunks@toad.com<br>
Message Hash: dfe77caafa2efff8e38c6ece7c0ea323c3478eeb7bc9e63d49f711cb0c8ba512<br>
Message ID: \<ad946a8a010210047a9a@[205.199.118.202]\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-04-13 06:29:19 UTC<br>
Raw Date: Sat, 13 Apr 1996 14:29:19 +0800<br>

## Raw message

```
{% raw  %}From: tcmay@got.net (Timothy C. May)
Date: Sat, 13 Apr 1996 14:29:19 +0800
To: cypherpunks@toad.com
Subject: Re: Entropy Estimator
Message-ID: <ad946a8a010210047a9a@[205.199.118.202]>
MIME-Version: 1.0
Content-Type: text/plain


At 9:06 PM 4/12/96, rick hoselton wrote:
>At 12:19 AM 4/12/96 -0400, JonWienke@aol.com wrote:
>
>>I just added a feature to my entropy graphing program that
>>estimates the number of bits of entropy in the file,
>
>Hey, that's just what I need.  I have these two 8-million byte
>files.  One is a recording made by a geiger counter, every bit
>is uncorrelated with anything else in the universe and each bit
>is equally likely to be a one or a zero.  The second file is an
>IDEA encryption of all the four-byte numbers
>from one to two-million.
>
>Here's my problem.  I can't remember which file is which, and I've
>forgotten sixty-four bits of the key I used to produce the encrypted file.
>
>That's where your technique come in.  The first file has sixty-four
>million bits of entropy.  The second file has only sixty-four bits
>of entropy, total (the missing key bits).  Surely, your technique can
>tell me which file is which.

No, this is not the case. Suppose your file of 64 million bits of entropy
is stored as "Rick's Geiger Counter File," perhaps on your Web site. (Great
for use by various people as a "virtual one time pad" (patent pending).)

A year or so from now someone asks a program to measure the entropy of this
file. Nearly all programs will report that the file has lots of bits of
entropy...

However, is this the "true" entropy? A clever program, or a person, might
well remember that this file is Rick's Geiger Counter File, making the bits
_very_ predictable (or, equivalently, little "surprise," low entropy, great
compressibility, etc.).

Once again, one can never know for sure that a file, sequence, string is
maximally compressed.

The application to your stated problem is that the two files might very
well have similar statistics (a good cryptographic hash function is likely
to produce a regular output, for example) and that a program cannot tell
which one is the "really random" file and which is the "seemingly random"
file is not a failing of the program, necessarily, but is implicit in some
inevitable limitations of all programs.

--Tim May

Boycott "Big Brother Inside" software!
We got computers, we're tapping phone lines, we know that that ain't allowed.
---------:---------:---------:---------:---------:---------:---------:----
Timothy C. May              | Crypto Anarchy: encryption, digital money,
tcmay@got.net  408-728-0152 | anonymous networks, digital pseudonyms, zero
W.A.S.T.E.: Corralitos, CA  | knowledge, reputations, information markets,
Higher Power: 2^756839 - 1  | black markets, collapse of governments.
"National borders aren't even speed bumps on the information superhighway."








{% endraw %}
```

## Thread

+ Return to [April 1996](/archive/1996/04)

+ Return to "[tcmay<span>@</span>got.net (Timothy C. May)](/authors/tcmay_at_got_net_timothy_c_may_)"

+ 1996-04-13 (Sat, 13 Apr 1996 14:29:19 +0800) - Re: Entropy Estimator - _tcmay@got.net (Timothy C. May)_

