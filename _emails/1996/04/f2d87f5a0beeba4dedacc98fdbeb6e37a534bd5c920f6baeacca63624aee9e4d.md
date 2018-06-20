---
layout: default
---

# 1996-04-19 - Re: why compression doesn't perfectly even out entropy

## Header Data

From: JonWienke@aol.com<br>
To: cypherpunks@toad.com<br>
Message Hash: f2d87f5a0beeba4dedacc98fdbeb6e37a534bd5c920f6baeacca63624aee9e4d<br>
Message ID: \<960418184409_378088479@emout09.mail.aol.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-04-19 06:35:29 UTC<br>
Raw Date: Fri, 19 Apr 1996 14:35:29 +0800<br>

## Raw message

```
{% raw  %}From: JonWienke@aol.com
Date: Fri, 19 Apr 1996 14:35:29 +0800
To: cypherpunks@toad.com
Subject: Re: why compression doesn't perfectly even out entropy
Message-ID: <960418184409_378088479@emout09.mail.aol.com>
MIME-Version: 1.0
Content-Type: text/plain


In a message dated 96-04-18 15:05:51 EDT, Perry Metzger writes:

>Before making pronouncements like "You are still OK" you ought to
>learn a bit more about cryptanalysis. Its tiny little statistical
>toeholds like that which permit breaks. I don't know for sure, but my
>intuition says that there may very well be instances in which a couple
>of little nicks like that into the entropy of a key are sufficient to
>radically lower the time to crack something. Since there are far
>better techniques available (hash distillation, for instance) for
>assuring the quality of a random stream, Jon's suggested techniques
>should be regarded as unnecessary and dangerous.
[Slightly ad hominem PSA deleted]

1.  If "cooking" a byte sequence in a manner that reduces its maximum entropy
by less than 1% allows an attacker to break your cryptosystem, then it is
crap to begin with.  With only a little more effort, he could break it
anyway.

2.  All I was trying to say was that applying cooking technique X to a byte
sequence will reduce the maximum entropy of the sequence by a factor of Y;
adjust entropy expectations accordingly.  I said nothing about the origin of
the byte sequence, the techniques used to generate it, or the exact method
for "cooking" it.  I did not recommend against using hash distillation,
hardware RNG's, or any other commonly accepted method of generating
cryptographically useful random or pseudo-random numbers.

Jonathan Wienke




{% endraw %}
```

## Thread

+ Return to [April 1996](/archive/1996/04)

+ 1996-04-19 (Fri, 19 Apr 1996 14:35:29 +0800) - Re: why compression doesn't perfectly even out entropy - _JonWienke@aol.com_
  + 1996-04-19 (Fri, 19 Apr 1996 13:05:40 +0800) - [Re: why compression doesn't perfectly even out entropy](/archive/1996/04/e445b9bcde7eaebf21d0300b44e649480d03d5d67d491923a8bd30a8c6dea030) - _"Perry E. Metzger" \<perry@piermont.com\>_

