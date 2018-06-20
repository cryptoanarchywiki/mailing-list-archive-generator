---
layout: default
---

# 1994-02-07 - RE: Magic Money attack

## Header Data

From: nobody@shell.portal.com<br>
To: cypherpunks@toad.com<br>
Message Hash: 9f00dc9e0b613eedfaf8e7af3d426dea2c1dfd97be8bbcb34ebc2cd6cfc3590b<br>
Message ID: \<199402070541.VAA25288@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-02-07 05:46:09 UTC<br>
Raw Date: Sun, 6 Feb 94 21:46:09 PST<br>

## Raw message

```
{% raw  %}From: nobody@shell.portal.com
Date: Sun, 6 Feb 94 21:46:09 PST
To: cypherpunks@toad.com
Subject: RE: Magic Money attack
Message-ID: <199402070541.VAA25288@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

hfinney@shell.portal.com wrote:

I think there may be a security weakness in Magic Money coins, and in
Chaum's "online" cash system from the Chaum/Fiat/Naor paper.

[ describes the Magic Money coins ]

[ only 18 bytes are checked ]

Easy enough to fix. Will code this. I just sent new PGP Tools and Magic
Money updates to MPJ. He must be getting tired of me sending him new code
all the time. :-) The latest version does protect against garbling of the
message from client to server.

>The other relevant point is that the bank has to sign everything you
>give to it (with payment) - it can't check the bit pattern for
>legality, since what it is signing is blinded.  So you can really get
>the bank to sign anything.

Any way to avoid this, other than a cumbersome cut-and-choose?

[ attacker gets a bunch of small primes signed ]

>The idea would be for him to try to factor a legal Y using just the
>primes he has.  If he can find a factorization using only small primes
>of a number which holds the magic 18-byte sequence in the right place,
>he can multiply together the signed forms of the primes to produce a
>signed version of that number.  This would be a successfully forged coin.

How many small primes would it take? How would he know what numbers to
multiply to get the coins? Just create random coins and look for one which
is made of all small factors? I should try this and see if I can find one.
Not being an expert in the math, would most coins have a large factor, or
would there be a fair number with only small factors?

>So, the question is whether it would be feasible to collect enough
>signed small primes to be able to generate more valid coins than you
>have primes.  (It costs you a coin each time you get the bank to sign
>something, so for this to be a money-making venture you want to get
>more out of it than you put into it!)  I think there are a reasonable
>fraction of numbers factorable by only small primes.  Since there are
>2^128 possible money values (based on the 16 random bytes) there
>should be quite a lot which are factorable by only small primes.

Any math whizzes out there care to run these numbers?

>Magic Money could help by checking the high bytes as well as the magic
>18; it would be take more time to factor 1024 bit numbers than 272 bit
>ones ((18+16)*8), and there would be fewer that are factorable by
>small primes.  But the problem would still exist.  The attacker can run
>a fast sieve to identify numbers which are factorable in his set.

The high-byte check I will code up right now, but I'll wait until we figure 
out what to do about this problem, before dumping any more code on MPJ.
Is anyone going to start up a server, when the program is debugged?

>The same attack would apply to Chaum's online cash.  His cash is of the
>form, (x,f(x)^(1/e)), where f() is a one-way function like MD5.  To forge
>this you would again get signed forms of the small primes, then keep
>picking random x's, until you got a f(x) which could be factored by your
>set.  Presto, you can create a fake coin.

Anyone know Chaum's email address? We could ask him...

>I don't know how this attack can be prevented.

I can think of one way. Redefine the coin format so the last 2 bytes or so
can be anything you want. Now when the user generates a coin, he sets these
last two bytes to 0001 and then tests for primality. He keeps adding 2 and 
checking until he finds a coin which is prime, or at least doesn't have any 
small factors.

When the server gets a coin, it checks it for primality, and only accepts
coins that pass the prime test. This way any coin made out of small factors
will not be accepted.

The small-factor sieve is fast, and with the proper #defines, it checks 
all primes below 8192 decimal. The slowtest() PGP uses is slow even for the
512-bit primes used to make 1024 bit PGP keys. It would be useless for a
full 1024-bit number. Would eliminating coins with factors below 8192 be
enough? Or how could one more quickly check the coin for primality?

                                          Pr0duct Cypher

-----BEGIN PGP SIGNATURE-----
Version: 2.3a

iQCVAgUBLVXKf8GoFIWXVYodAQHCsgQAmeUjeqb3utFdW2AwPU7a2Bs7dxRtVOPi
wzS3Jcp+QVZ4GgGLJpr2ZLW4EenX/kAkF5cLBeBebt+6RHD7jel2SxbXxeZ8Ab64
o45oibcrvN9xEnBUkEinfDfH9rkAobYFgNPfGDEs1ajDzw8ISwUDOmA+glm01xzg
XBZFLdyQWwM=
=H+UC
-----END PGP SIGNATURE-----




{% endraw %}
```

## Thread

+ Return to [February 1994](/archive/1994/02)

+ 1994-02-07 (Sun, 6 Feb 94 21:46:09 PST) - RE: Magic Money attack - _nobody@shell.portal.com_
  + 1994-02-07 (Mon, 7 Feb 94 03:06:15 PST) - [Re: Magic Money attack](/archive/1994/02/f3f70e355758f0deb6484d5024784fb59aa81aa35f62274c9eb41ba9d564c848) - _jkreznar@ininx.com (John E. Kreznar)_

