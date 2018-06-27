---
layout: default
---

# 1994-03-05 - Re:  more steganography talk

## Header Data

From: wcs<span>@</span>anchor.ho.att.com (bill.stewart<span>@</span>pleasantonca.ncr.com +1-510-484-6204)<br>
To: cypherpunks@toad.com<br>
Message Hash: a2aebe608ea85ab4f2d2d970eeb8f4adaf838d76faeb564a3cfb1d3863f5f0a5<br>
Message ID: \<9403050500.AA01957@anchor.ho.att.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-03-05 05:01:04 UTC<br>
Raw Date: Fri, 4 Mar 94 21:01:04 PST<br>

## Raw message

```
{% raw  %}From: wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)
Date: Fri, 4 Mar 94 21:01:04 PST
To: cypherpunks@toad.com
Subject: Re:  more steganography talk
Message-ID: <9403050500.AA01957@anchor.ho.att.com>
MIME-Version: 1.0
Content-Type: text/plain


Eric Hugher, replying to somebody, writes:	
> > The idea:  Encrypt a widely known value with the recipient's  
> > public-key and use the result as an initialization vector for a  
> > clever transformation/steganography algorithm.  
> 
> How many public keys are there can there be?
> Assume one hundred each for 10 billion persons.  That's 2^40 keys, or
> an effective key length of 40 bits.  Since there are not more than
> 2^16 public keys right now (a generous estimate) we can assume that
> this technique is insecure for public keys.

If you're going to go to the trouble of using a public key,
including handling generation, distribution and validation of public keys,
you might as well use a "clever transformation/steganography algorithm"
that's good enough that a brute-force search of all the public keys
won't reverse it.  A good candidate for such an algorithm would be IDEA -
and if this sounds like I'm reinventing PGP, it's intentional :-)

Essentially, you're proposing wrapping PGP in PGP, or in weakened-PGP.
Better to just use Stealth-PGP to eliminate the distinctive markers
that make PGP easy to find, maybe run the code through tran for
extra scrambling if you're not running pnmstega, and then steganize.
And make sure that if you write PGP, The Next Generation, you make
it stealthy so people who don't have the right keys just see noise.

		Bill




{% endraw %}
```

## Thread

+ Return to [March 1994](/archive/1994/03)

+ Return to "[wcs<span>@</span>anchor.ho.att.com (bill.stewart<span>@</span>pleasantonca.ncr.com +1-510-484-6204)](/authors/wcs_at_anchor_ho_att_com_bill_stewart_at_pleasantonca_ncr_com_15104846204_)"

+ 1994-03-05 (Fri, 4 Mar 94 21:01:04 PST) - Re:  more steganography talk - _wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)_

