---
layout: default
---

# 1996-11-29 - Re: Is /dev/random good enough to generate one-time pads?

## Header Data

From: Steve Reid \<steve@edmweb.com\><br>
To: The Deviant \<deviant@pooh-corner.com\><br>
Message Hash: 8fa20d87f4e8f8cdecacf96867e79e56dc794a5c2eb6ccc8feabbf48c5cff5f5<br>
Message ID: \<Pine.BSF.3.91.961128153422.182A-100000@bitbucket.edmweb.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-11-29 00:27:33 UTC<br>
Raw Date: Thu, 28 Nov 1996 16:27:33 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: Steve Reid <steve@edmweb.com>
Date: Thu, 28 Nov 1996 16:27:33 -0800 (PST)
To: The Deviant <deviant@pooh-corner.com>
Subject: Re: Is /dev/random good enough to generate one-time pads?
Message-ID: <Pine.BSF.3.91.961128153422.182A-100000@bitbucket.edmweb.com>
MIME-Version: 1.0
Content-Type: text/plain


> > Subj sez it all.
> Yes, as a matter of fact it is.  /dev/random is based on an entropy pool
> taken from hardware interrupts and such, thus is a RNG, not a PRNG

I expect it would be "good enough", but it is not _perfectly_ random, and 
so it wouldn't be a true one-time pad.

Because it uses MD5, the bits are not all provably independent. You get 
(very strong) cryptographic security instead of perfect security.

The one-time pad is easy to explain in theory, but implementing it
perfectly is extremely difficult. Many people believe that quantum events
are the only source of perfect randomness, but most methods for harvesting
that randomness could introduce statistical properties. For example, a
radioactive substance may have exactly a 50% chance of emitting a particle
given a certain amount of time, but what happens if your timer isn't
perfect? 

One-way hashes are good at removing such obvious and not-so-obvious
statistical properties, but like a PRNG, you can't prove that the bits it
produces are all completely independent. It's definately "good enough",
but it's not perfect. 





{% endraw %}
```

## Thread

+ Return to [November 1996](/archive/1996/11)

+ 1996-11-29 (Thu, 28 Nov 1996 16:27:33 -0800 (PST)) - Re: Is /dev/random good enough to generate one-time pads? - _Steve Reid \<steve@edmweb.com\>_
  + 1996-11-29 (Thu, 28 Nov 1996 20:24:08 -0800 (PST)) - [Re: Is /dev/random good enough to generate one-time pads?](/archive/1996/11/c1c2d93535dd866723c6f82e5521a74b1e2c42975177d11a5b156b621ef8234a) - _The Deviant \<deviant@pooh-corner.com\>_

