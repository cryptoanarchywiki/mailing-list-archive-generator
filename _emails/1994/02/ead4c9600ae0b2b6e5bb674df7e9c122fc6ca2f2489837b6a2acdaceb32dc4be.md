---
layout: default
---

# 1994-02-07 - RE: Magic Money attack

## Header Data

From: Hal \<hfinney@shell.portal.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: ead4c9600ae0b2b6e5bb674df7e9c122fc6ca2f2489837b6a2acdaceb32dc4be<br>
Message ID: \<199402070641.WAA27913@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-02-07 06:41:09 UTC<br>
Raw Date: Sun, 6 Feb 94 22:41:09 PST<br>

## Raw message

```
{% raw  %}From: Hal <hfinney@shell.portal.com>
Date: Sun, 6 Feb 94 22:41:09 PST
To: cypherpunks@toad.com
Subject: RE: Magic Money attack
Message-ID: <199402070641.WAA27913@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


From Pr0duct Cypher:

> [ only 18 bytes are checked ]
> 
> Easy enough to fix. Will code this. I just sent new PGP Tools and Magic
> Money updates to MPJ. He must be getting tired of me sending him new code
> all the time. :-) The latest version does protect against garbling of the
> message from client to server.

I think it's great that you are able to fix these things so quickly.
It's natural that there will be a lot of shaking out in any initial
release.

> How many small primes would it take? How would he know what numbers to
> multiply to get the coins? Just create random coins and look for one which
> is made of all small factors? I should try this and see if I can find one.
> Not being an expert in the math, would most coins have a large factor, or
> would there be a fair number with only small factors?

Knuth has some discussion of this in Seminumerical Algorithms.  The term
for numbers which have only small factors is that they are "smooth".  He
has some formulas for what fraction of numbers are smooth based on the
size of the largest allowed prime and the size of the numbers.  Unfortunately
I won't have access to my copy until Tuesday.  Perhaps someone else can
look it up.

> >I don't know how this attack can be prevented.
> 
> I can think of one way. Redefine the coin format so the last 2 bytes or so
> can be anything you want. Now when the user generates a coin, he sets these
> last two bytes to 0001 and then tests for primality. He keeps adding 2 and 
> checking until he finds a coin which is prime, or at least doesn't have any 
> small factors.

Clever idea.  If only it wouldn't be so slow.

> The small-factor sieve is fast, and with the proper #defines, it checks 
> all primes below 8192 decimal. The slowtest() PGP uses is slow even for the
> 512-bit primes used to make 1024 bit PGP keys. It would be useless for a
> full 1024-bit number. Would eliminating coins with factors below 8192 be
> enough? Or how could one more quickly check the coin for primality?

The 8192 cutoff might work.  We would have to check it out, but it
could be that finding 1024-bit numbers in a relatively narrow range of
+/- 2^64 which are composed solely of factors in the range, say, 8192
to 16384 would be infeasible.  I don't recall whether Knuth considers the
problem in this form.  This would be a great save if it works.

Hal




{% endraw %}
```

## Thread

+ Return to [February 1994](/archive/1994/02)

+ 1994-02-07 (Sun, 6 Feb 94 22:41:09 PST) - RE: Magic Money attack - _Hal \<hfinney@shell.portal.com\>_

