---
layout: default
---

# 1994-01-31 - Re:  Remailer Tearline Conventions

## Header Data

From: Eli Brandt \<ebrandt@jarthur.Claremont.EDU\><br>
To: cypherpunks list \<cypherpunks@toad.com\><br>
Message Hash: 83bcfd4b9e0c9bd0f5fe516fe3e2ba1e4b856b2c90edc4ddfbb28ec9fa273258<br>
Message ID: \<9401312103.AA02297@toad.com\><br>
Reply To: \<9401310923.AA04199@anchor.ho.att.com\><br>
UTC Datetime: 1994-01-31 21:04:33 UTC<br>
Raw Date: Mon, 31 Jan 94 13:04:33 PST<br>

## Raw message

```
{% raw  %}From: Eli Brandt <ebrandt@jarthur.Claremont.EDU>
Date: Mon, 31 Jan 94 13:04:33 PST
To: cypherpunks list <cypherpunks@toad.com>
Subject: Re:  Remailer Tearline Conventions
In-Reply-To: <9401310923.AA04199@anchor.ho.att.com>
Message-ID: <9401312103.AA02297@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


Bill Stewart said:
> Julf's anon.penet.fi remailer  cuts off anything resembling a signature,
> using the convention that a -- line (or maybe an all-dash line?)
> is a signature, since some of the common mail and news programs use that,

Picking any fixed sig marker is likely to cause problems -- notice
how often anon.penet.fi messages show up truncated due to a line of
hyphens.  A more flexible possibility: allow an X-Sig-Marker: header,
which specifies a pattern/regexp to strip after.  Actually, the
sig marker line itself should be stripped as well, in case it
contains identifying information.

> formal and mimeish, or a simpler '--truncate here--' sort of line
> that gets retained across remailing so additional junk doesn't accrete.

I don't see the problem you're guarding against.  Could you explain?
Seems that sig elision needs to be done once, by the first hop, and
then you're home free.

   Eli   ebrandt@jarthur.claremont.edu




{% endraw %}
```

## Thread

+ Return to [January 1994](/archive/1994/01)
+ Return to [February 1994](/archive/1994/02)

+ 1994-01-31 (Mon, 31 Jan 94 01:29:12 PST) - [Re:  Remailer Tearline Conventions](/archive/1994/01/46ee7a2e171c207bab2c7de42377c41857800c767d80388138b8d9a7601e131b) - _wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)_
  + 1994-01-31 (Mon, 31 Jan 94 13:04:33 PST) - Re:  Remailer Tearline Conventions - _Eli Brandt \<ebrandt@jarthur.Claremont.EDU\>_
    + 1994-02-05 (Sat, 5 Feb 94 11:15:40 PST) - [Remailer Tearline Variant](/archive/1994/02/3cff1a885cf964bc68f85f81a65d7a17dbb29f4baa6951491234986f0415880a) - _garet.jax@nitelog.com (Garet Jax)_

