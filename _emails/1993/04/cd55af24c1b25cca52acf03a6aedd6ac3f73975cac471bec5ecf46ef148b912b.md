---
layout: default
---

# 1993-04-20 - Re: Another Clipper weakness

## Header Data

From: Hal \<74076.1041@CompuServe.COM\><br>
To: CYPHERPUNKS \<CYPHERPUNKS@toad.com\><br>
Message Hash: cd55af24c1b25cca52acf03a6aedd6ac3f73975cac471bec5ecf46ef148b912b<br>
Message ID: \<930420195747_74076.1041_FHD36-1@CompuServe.COM\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-04-20 20:13:48 UTC<br>
Raw Date: Tue, 20 Apr 93 13:13:48 PDT<br>

## Raw message

```
{% raw  %}From: Hal <74076.1041@CompuServe.COM>
Date: Tue, 20 Apr 93 13:13:48 PDT
To: CYPHERPUNKS <CYPHERPUNKS@toad.com>
Subject: Re: Another Clipper weakness
Message-ID: <930420195747_74076.1041_FHD36-1@CompuServe.COM>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

From: "Perry E. Metzger" <pmetzger@lehman.com>

> I've just looked over the proposal again, and I've seen no mention of
> random inputs -- only that the 30 bit key would get a "fixed 34 bit
> padding" added to it.

Here is what Denning's writeup says:

  At the beginning of a session, a trusted agent from each of the two key
  escrow agencies enters the vault.  Agent 1 enters an 80-bit value S1
  into the laptop and agent 2 enters an 80-bit value S2. These values
  serve as seeds to generate keys for a sequence of serial numbers.
  
  To generate the unit key for a serial number N, the 30-bit value N is
  first padded with a fixed 34-bit block to produce a 64-bit block N1.
  S1 and S2 are then used as keys to triple-encrypt N1, producing a
  64-bit block R1:
  
          R1 = E[D[E[N1; S1]; S2]; S1] .
  
  Similarly, N is padded with two other 34-bit blocks to produce N2 and
  N3, and two additional 64-bit blocks R2 and R3 are computed:  
  
          R2 = E[D[E[N2; S1]; S2]; S1] 
          R3 = E[D[E[N3; S1]; S2]; S1] .
  
  R1, R2, and R3 are then concatenated together, giving 192 bits. The
  first 80 bits are assigned to U1 and the second 80 bits to U2.  The
  rest are discarded.  The unit key U is the XOR of U1 and U2.  U1 and U2
  are the key parts that are separately escrowed with the two escrow
  agencies.

Here, the notiation E[X; Y] means to encrypt 64-bit number X using 80-bit
key Y with the Skipjack algorithm.

U1 and U2 come from concatenating R1, R2, and R3.
Each of R1, R2, and R3 is a function not only of N, the serial number,
along with the 3 fixed 34-bit blocks, but also S1 and S2, the two random
numbers entered by agents from the escrow organizations.


> > The one problem is that S1 and S2 are not changed for each chip, but are
> > rather kept the same in programming a batch of about 300 chips.  Then
> > they are supposed to be destroyed.
> 
> This was not clearly implied, either. Furthermore, no clear reason has
> been stated why all this complexity is needed and U1 and U2 can't just
> be randomly generated.

  All Clipper Chips are programmed inside a SCIF (secure computer
  information facility), which is essentially a vault.  The SCIF contains
  a laptop computer and equipment to program the chips.  About 300 chips
  are programmed during a single session.  The SCIF is located at
  Mikotronx.

I agree that the process seems complex.  Why should the keys
U1 and U2 be correlated with the serial number in this way?  Here is
one thought:

The most straightforward approach would be to get two random seeds,
S1 and S2, and use them to run a PRNG that produces U1 and U2, the
two key-halves, and N, the serial number.

But the problem with this is that you are depending on the security
of your PRNG to ensure that there is no correlation between N and
U1/U2.  Ordinary PRNG's might allow some correlation to exist.  This
would be weak because then just knowing the N of your chip might allow
a good organization like NSA to crunch out U1 and U2 without going
through the escrow agencies, by exploiting weaknesses in the PRNG.

Instead, they go through a roundabout process which appears to show that
the relationship between N and U1/U2 is as strong as the Skipjack
algorithm itself, in fact when run in a triple-encryption mode.
If NSA had a way, given N, to produce U1/U2, then it would appear
that they must be able to break Skipjack, in which case they wouldn't
need U1/U2.  So this key generation process can be argued not to
introduce any new vulnerability in the system.

Hal

-----BEGIN PGP SIGNATURE-----
Version: 2.2

iQCVAgUBK9QrV6gTA69YIUw3AQGGrAP/Rmx0H603b1EdBIsiGuc637wptW133IFU
/irxw+aCPrL3yOzuBTQbUW+LeMIwpC+Y8DARkAohxnIjhuu/aQXVnIvJPPiUSPr0
fz2PLxhA5tgjVAH0e5xvl9K+CgWnRXazd9Tp+Zbi/xAiWz0PI6kff4QtNG13p1xw
/V0dGDb4tec=
=XgfH
-----END PGP SIGNATURE-----





{% endraw %}
```

## Thread

+ Return to [April 1993](/archive/1993/04)

+ 1993-04-20 (Tue, 20 Apr 93 13:13:48 PDT) - Re: Another Clipper weakness - _Hal \<74076.1041@CompuServe.COM\>_
  + 1993-04-20 (Tue, 20 Apr 93 13:32:50 PDT) - [Re: Another Clipper weakness](/archive/1993/04/b1ff47955c4a1982d903fc83b9e7fdfd54df8170aa889ce981ed5797e340bb7b) - _"Perry E. Metzger" \<pmetzger@lehman.com\>_

