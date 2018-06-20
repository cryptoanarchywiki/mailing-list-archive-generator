---
layout: default
---

# 1993-03-03 - Re: anon.penet.fi hacking

## Header Data

From: Eli Brandt \<ebrandt@jarthur.Claremont.EDU\><br>
To: cypherpunks@toad.com<br>
Message Hash: fd4bae87bd4baa2917237da385aceb09c8af9a4a14fd5ca5ba8d7bfda1569e5c<br>
Message ID: \<9303030740.AA11601@toad.com\><br>
Reply To: \<930301171036_74076.1041_DHJ55-1@CompuServe.COM\><br>
UTC Datetime: 1993-03-03 07:40:45 UTC<br>
Raw Date: Tue, 2 Mar 93 23:40:45 PST<br>

## Raw message

```
{% raw  %}From: Eli Brandt <ebrandt@jarthur.Claremont.EDU>
Date: Tue, 2 Mar 93 23:40:45 PST
To: cypherpunks@toad.com
Subject: Re: anon.penet.fi hacking
In-Reply-To: <930301171036_74076.1041_DHJ55-1@CompuServe.COM>
Message-ID: <9303030740.AA11601@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


> Eric shows a complicated regular expression, but I don't think it
> will match just --, because this line provides nothing to match the
> "." and "[^B]", etc.

Instead of these ballooning regexps, how about just using Chael
Hall's standardized "end of body" marker?  Even if some people had
to add it manually to each message, well, that's not a big deal.
But I suspect that the people who have sigs being added by BBS
software are going to have trouble adding strange header lines, even
if they have the regexp expertise to construct them.  

Anyone who does control their sig, but doesn't want to take the
trouble to include it only some of the time, can just add the
marker.  People might even be able to convince BBS sysops to add it
to their autosigs.  Or if this just looks too cluttered, maybe the
sig-clipper header could just be "Signature-Lines:" -- clip that
many, or none by default, and you're done.

> Hal

	 PGP 2 key by finger or e-mail
   Eli   ebrandt@jarthur.claremont.edu




{% endraw %}
```

## Thread

+ Return to [March 1993](/archive/1993/03)

+ 1993-03-01 (Mon, 1 Mar 93 09:34:08 PST) - [anon.penet.fi hacking](/archive/1993/03/6ccbeac6e64cfd3ced62682c2b33ee7aea01ee92a418ca4e23ab6c170c4aac50) - _Hal \<74076.1041@CompuServe.COM\>_
  + 1993-03-03 (Tue, 2 Mar 93 23:40:45 PST) - Re: anon.penet.fi hacking - _Eli Brandt \<ebrandt@jarthur.Claremont.EDU\>_
    + 1993-03-03 (Wed, 3 Mar 93 00:34:30 PST) - [ANON: Re: anon.penet.fi hacking](/archive/1993/03/0f76851010afce15af6f83ea28aa7cc3b5638b8290ecff7bfb71ec7ce921a2ca) - _Johan Helsingius \<julf@penet.FI\>_

