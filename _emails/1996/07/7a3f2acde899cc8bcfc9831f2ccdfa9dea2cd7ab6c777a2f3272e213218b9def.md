---
layout: default
---

# 1996-07-01 - Re: Hardware RNG

## Header Data

From: jamesd@echeque.com<br>
To: cypherpunks@toad.com<br>
Message Hash: 7a3f2acde899cc8bcfc9831f2ccdfa9dea2cd7ab6c777a2f3272e213218b9def<br>
Message ID: \<199607011504.IAA24410@dns2.noc.best.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-07-01 19:03:35 UTC<br>
Raw Date: Tue, 2 Jul 1996 03:03:35 +0800<br>

## Raw message

```
{% raw  %}From: jamesd@echeque.com
Date: Tue, 2 Jul 1996 03:03:35 +0800
To: cypherpunks@toad.com
Subject: Re: Hardware RNG
Message-ID: <199607011504.IAA24410@dns2.noc.best.net>
MIME-Version: 1.0
Content-Type: text/plain


At 06:23 AM 6/30/96 -0700, Timothy C. May wrote:
> While radioactive decay is unpredictable (so are a lot of things, by the
> way), there are all kinds of biases that reduce the apparent entropy.
> Detector "dead time" is a classic one (basically, the detector can't detect
> counts during a post-pulse recovery time...probably not a problem at low
> count rates, but an example of how subtle things can sneak in).

If he has more than eight bits of timing resolution, such biases will
have no affect.

He is using his non uniformly distributed random number to select a
uniformly distributed pseudo random number.

Provided that the does not attempt to get more entropy out than he
puts in, the result should be a uniformly distributed truly random
number.
 ---------------------------------------------------------------------
              				|  
We have the right to defend ourselves	|   http://www.jim.com/jamesd/
and our property, because of the kind	|  
of animals that we are. True law	|   James A. Donald
derives from this right, not from the	|  
arbitrary power of the state.		|   jamesd@echeque.com





{% endraw %}
```

## Thread

+ Return to [July 1996](/archive/1996/07)

+ 1996-07-01 (Tue, 2 Jul 1996 03:03:35 +0800) - Re: Hardware RNG - _jamesd@echeque.com_

