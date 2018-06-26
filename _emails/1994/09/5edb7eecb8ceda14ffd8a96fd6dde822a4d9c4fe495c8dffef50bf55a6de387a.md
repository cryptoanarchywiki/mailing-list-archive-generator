---
layout: default
---

# 1994-09-01 - Re: Art Gallery on internet needs PGP signatures

## Header Data

From: tcmay<span>@</span>netcom.com (Timothy C. May)<br>
To: bdolan@well.sf.ca.us (Brad Dolan)<br>
Message Hash: 5edb7eecb8ceda14ffd8a96fd6dde822a4d9c4fe495c8dffef50bf55a6de387a<br>
Message ID: \<199409011818.LAA09850@netcom13.netcom.com\><br>
Reply To: \<199409011330.GAA19093@well.sf.ca.us\><br>
UTC Datetime: 1994-09-01 18:18:45 UTC<br>
Raw Date: Thu, 1 Sep 94 11:18:45 PDT<br>

## Raw message

```
{% raw  %}From: tcmay@netcom.com (Timothy C. May)
Date: Thu, 1 Sep 94 11:18:45 PDT
To: bdolan@well.sf.ca.us (Brad Dolan)
Subject: Re: Art Gallery on internet needs PGP signatures
In-Reply-To: <199409011330.GAA19093@well.sf.ca.us>
Message-ID: <199409011818.LAA09850@netcom13.netcom.com>
MIME-Version: 1.0
Content-Type: text/plain



> A Mr. Ken Nahan (of New York, *I think*) was on the NBC Today show 
> this morning, discussing his plans to set up a commercial art gallery 
> on the internet.  He intends to set up some kind of server with graphic 
> images and text descriptions of works of art which are for sale.  He 
> also wants to be able to accept bids via the internet.
> 
> Some knowledgeable person should talk to him about digital signatures,
> PGP, etc.  

There's an interesting connection between art, forgeries, and public
key crypto. I heard about this some years ago, and not since, so I
guess the idea never really caught on.

A company in L.A., "Light Signatures" as I recall, was selling a
system that took an optical scan, a line scan from one corner of an
object to another. (On a paiting, for example.)

The resulting bit sequence (of pixel values) could then be encrypted
with the private key of the creator, or appraiser, or whatever. This
would be the "provenance" of the work.

Out in the "field," in the auction houses, for example, the signature
could be verified by taking the digital signature, applying the
_public_ key, which would then generate the sequence of pixel values,
and comparing it what a field scanner actually saw.

(The idea is the familiar one, applied slightly differently.)

A main use was predicted to be making "unforgeable" machine parts,
like crankshafts, engine blocks, etc. The pattern of scratches,
surface marks, etc., could be 'signed' by Harley-Davidson, Ferrari,
etc. (apparently they are plagued by forgeries).

There are some obvious technical issues of error tolerance (have to
tolerate a few new scratches, marks without compromising the
security), where to stamp the number, etc.

I thought it a novel idea, back in 1988, and I'm somewhat surprised
the idea seems to have never reached commercialization.

--Tim May


-- 
..........................................................................
Timothy C. May         | Crypto Anarchy: encryption, digital money,  
tcmay@netcom.com       | anonymous networks, digital pseudonyms, zero
408-688-5409           | knowledge, reputations, information markets, 
W.A.S.T.E.: Aptos, CA  | black markets, collapse of governments.
Higher Power: 2^859433 | Public Key: PGP and MailSafe available.
"National borders are just speed bumps on the information superhighway."



{% endraw %}
```

## Thread

+ Return to [September 1994](/archive/1994/09)

+ Return to "[Brad Dolan <bdolan<span>@</span>well.sf.ca.us>](/author/brad_dolan_bdolan_at_well_sf_ca_us_)"
+ Return to "[tcmay<span>@</span>netcom.com (Timothy C. May)](/author/tcmay_at_netcom_com_timothy_c_may_)"

+ 1994-09-01 (Thu, 1 Sep 94 06:31:10 PDT) - [Art Gallery on internet needs PGP signatures](/archive/1994/09/d9726c9324da9ceba767a670b4c5bbb4bf8c1cc1598358a7f83cd0bb9f859dda) - _Brad Dolan \<bdolan@well.sf.ca.us\>_
  + 1994-09-01 (Thu, 1 Sep 94 11:18:45 PDT) - Re: Art Gallery on internet needs PGP signatures - _tcmay@netcom.com (Timothy C. May)_

