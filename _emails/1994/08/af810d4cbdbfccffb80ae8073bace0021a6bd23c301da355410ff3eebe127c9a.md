---
layout: default
---

# 1994-08-20 - Brands cash

## Header Data

From: Hal \<hfinney<span>@</span>shell.portal.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: af810d4cbdbfccffb80ae8073bace0021a6bd23c301da355410ff3eebe127c9a<br>
Message ID: \<199408201652.JAA29752@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-08-20 16:53:19 UTC<br>
Raw Date: Sat, 20 Aug 94 09:53:19 PDT<br>

## Raw message

```
{% raw  %}From: Hal <hfinney@shell.portal.com>
Date: Sat, 20 Aug 94 09:53:19 PDT
To: cypherpunks@toad.com
Subject: Brands cash
Message-ID: <199408201652.JAA29752@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


Last year, Stefan Brands announced that he had come up with improved
versions of Chaumian cash and credentialling protocols which were
smaller, faster, and had provable correctness.  He still hasn't gone
public with them, but I thought I'd write up an introduction to his
earlier work so people can see what direction things are going.  IMO, if
he plays his cards right his technology could be the foundation for
electronic commerce.  OTOH if he is too greedy he'll be bypassed.  It
appears he is seeking patents on everything, a necessary step for
commercial interest, but we'll see how he markets it.

This is based on Brands' "An Efficient Off-line Electronic Cash System
Based on the Representation Problem", which was available on the net for
a while before he took it off.  I'm not sure what its status is now.
Perhaps he removed it pending release of his improved version.

Brands' work is based on discrete logs rather than RSA.  The discrete
logarithm problem is the "other" widely-used foundation for crypto
primitives, underlying Diffie-Hellman key exchange, ElGamal, Schnorr, and
DSS signatures, and many others.  I'll do a brief intro to using discrete
logs and then get to Brands' cash.

Discrete-log based cryptosystems generally work with a modulus n which is
prime, along with a "generator" g < n such that the series g^0, g^1, g^2,
... , includes all values from 1 to n-1.  It is pretty straightforward to
find such n's and g's.  It is easy to compute g^x for any x, but
intractable to calculate x given just g^x.  (Notation: ^ represents
exponentiation, and all math is implicitly mod n).  x is called the
discrete log (to the base g) of g^x and the difficulty of solving this is
the foundation of these protocols.  Note that unlike RSA, where taking
eth roots is hard for everyone except the owner of the secret key, taking
discrete logs is hard for everyone, without exception.  There is no trap
door here.

Diffie-Hellman key exchange

As an introduction, consider Diffie-Hellman key exchange.  In this
protocol, two people, Alice and Bob, want to publicly exchange data and
end up with a secret value which only they know.

1.  Alice chooses a random x and sends GX = g^x to Bob.  Bob chooses a
random y and sends GY = g^y to Alice.

2.  Alice calculates GY^x, which is g^(y*x).  Bob calculates GX^y, which
is g^(x*y).

3.  These are equal, so they use them as their shared secret value.

An observer sees only GX and GY, and without knowledge of x and y is
unable to calculate g^(x*y).

DH-based identification protocol

An identification protocol allows someone to prove that he is really who
he claims.  In this context, the prover Paul will convince the verifier
Vicki that he knows the secret key corresponding to Paul's established
public key.  In this and the following systems, Paul has a secret key
x<n, and a public key GX = g^x.  Again, note that it is impossible to go
from GX to x assuming discrete logs are hard.

1.  Vicki chooses a random y and sends GY = g^y to Paul.

2.  Paul calculates GYX = GY^x = g^(y*x) and sends that back to Vicki.

3.  Vicki confirms that GYX = GX^y; both should be g^(x*y).

This is like DH except that Paul exposes the secret information he
calculated, and only he could have done this.  One problem with this
protocol is that perhaps Paul calculating xth powers for Vicki might
reveal something about x.  The next protocol solves that:

Schnorr identification protocol

This comes from Schnorr, Journal of Cryptology, v4 n3, 1991.

1.  Paul chooses a random w and sends GW = g^w to Vicki.

2.  Vicki chooses a random c and sends it to Paul.

3.  Paul calculates r = cx+w and sends that to Vicki.

4.  Vicki confirms that g^r = (GX^c)*GW.  Both should be g^(cx+w).

The extra step of Paul sending g^w for a random w makes this protocol
reveal less information about x.  For any one run of the protocol, there
is some value of w which would produce a given r for any x, so knowing r
and c doesn't tell you anything about x.

Chaum discrete-log interactive signature protocol

This is the basic signature used by Brands, but I believe it comes from
Chaum&Pederson, Crypto 92.  It is an extension of the previous protocol
to allow signatures.  A digital signature on a value m is a certificate
which could only have been produced by the owner of a particular public
key.

In this protocol, a message m (<n) is being signed.  The basic signature
value is MX = m^x, which Paul sends.  By itself, though, this signature
is not obviously correct.  Without knowing x, Paul's secret key, there is
no way to confirm it.  So, Vicki must engage in an interactive protocol
with Paul in which he will prove that MX is equal to m^x.  It is very
similar to the previous one:

1.  Paul chooses a random w and sends GW = g^w and MW = m^w to Vicki.

2.  Vicki chooses a random c and sends it to Paul.

3.  Paul calculates r = cx+w and sends that to Vicki.

4.  Vicki confirms that g^r = (GX^c)*GW.  Both should be g^(cx+w).  She
also confirms that m^r = (MX^c)*MW.  Both should be m^(cx+w).

This is the previous protocol plus one extra number, MW.  The fact that
the same r is used for both m and g shows that m was raised to the same
power as g in creating MX vs GX.

Chaum Discrete-Log Signature Protocol

Interactive signature protocols may have advantages in some
circumstances, but in most cases we would prefer a signature which can be
checked without help from Paul.  There is a simple trick which can turn
most interactive signature protocols into regular signatures.  The idea
is that instead of c being chosen at random by Vicki, it is calculated by
using a cryptographically strong hash function (such as MD4, MD5, or DHS)
on the values which are publicly known by that point in the protocol: m,
MX, GW and MW.  Since both Paul and Vicki could calculate the hash, there
is no need for Vicki to send c to Paul.  Instead, he can do everything in
one step.  This leads to:

1.  Paul calculates MX = m^x.  He then chooses a random w and
calculates GW = g^w and MW = m^w.  He then calculates c = hash(m,MX,GW,MW).
He calculates r = cx+w, and sends MX, GW, MW and r to Vicki.  The tuple
(MX,GW,MW,r) is the signature on m.

2.  Vicki calculates c = hash(m,MX,GW,MW).  She then verifies, as
before, that g^r = (GX^c)*GW.  Both should be g^(cx+w).  She also
confirms that m^r = (MX^c)*MW.  Both should be m^(cx+w).

This protocol is not interactive.  Once Paul has completed step 1,
the signature can be published and anyone can play Vicki's part in
checking it.  Such a signature is functionally similar to the PGP
signatures we see on messages on the net, but as you can see the
mathematics behind it is completely different.

OK, that's all for now.  Next comes the good part: blind signatures.
Unlike Chaum's original blind signatures, which are the foundation of his
cash system, the discrete-log blind signatures have "restrictive
blinding", where there are limitations on what kinds of changes can be
made to the number being signed during the blinding process.  This allows
Brands to dispense with the clumsy cut-and-choose techniques Chaum was
forced to use in his advanced cash and credential systems.  I'll write
more about this later today or tomorrow.

Hal




{% endraw %}
```

## Thread

+ Return to [August 1994](/archive/1994/08)

+ Return to "[Hal <hfinney<span>@</span>shell.portal.com>](/author/hal_hfinney_at_shell_portal_com_)"

+ 1994-08-20 (Sat, 20 Aug 94 09:53:19 PDT) - Brands cash - _Hal \<hfinney@shell.portal.com\>_
  + 1994-08-22 (Mon, 22 Aug 94 16:18:16 PDT) - [Re: Brands cash](/archive/1994/08/8748b9a96504d2df86c3ae4eab1e4ca65856298e1bcf5a3d9ed9a412c1032382) - _Hal \<hfinney@shell.portal.com\>_
  + 1994-08-23 (Mon, 22 Aug 94 22:10:25 PDT) - [Re: Brands cash](/archive/1994/08/9064083f68a5a59778855aef1f0879d53af943780a171d7460d2ca18ba8e2c0c) - _Hal \<hfinney@shell.portal.com\>_
  + 1994-08-25 (Thu, 25 Aug 94 09:23:46 PDT) - [Re: Brands cash](/archive/1994/08/6c25d8bb4721b5387403612909ff282472555fa4496d7ea0d34c4a8eb119bbbd) - _Hal \<hfinney@shell.portal.com\>_

