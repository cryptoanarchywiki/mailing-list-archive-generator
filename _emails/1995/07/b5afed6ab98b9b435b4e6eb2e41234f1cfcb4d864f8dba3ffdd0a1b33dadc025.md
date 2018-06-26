---
layout: default
---

# 1995-07-20 - Re: Netscape the Big Win

## Header Data

From: Hal \<hfinney<span>@</span>shell.portal.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: b5afed6ab98b9b435b4e6eb2e41234f1cfcb4d864f8dba3ffdd0a1b33dadc025<br>
Message ID: \<199507201722.KAA10382@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-07-20 17:23:43 UTC<br>
Raw Date: Thu, 20 Jul 95 10:23:43 PDT<br>

## Raw message

```
{% raw  %}From: Hal <hfinney@shell.portal.com>
Date: Thu, 20 Jul 95 10:23:43 PDT
To: cypherpunks@toad.com
Subject: Re: Netscape the Big Win
Message-ID: <199507201722.KAA10382@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


From: Adam Shostack <adam@bwh.harvard.edu>
> 	Actually, it also supports Kerberos (not relevant to most of
> us), and PGP messaging.  Although a KCA would be needed before anything
> useful came of the PGP support, at least its there.

It appears that support for PGP messaging has been removed from the
July 1995 SHTTP draft.  So it's X.500 all the way.
<URL:http://info.internet.isi.edu/in-drafts/files/draft-ietf-wts-shttp-00.txt>


From: Steven Champeon - Imonics Development <schampeo@imonics.com>
> The one "advantage" to SSL that they were pushing over SHTTP was that
> SSL is a socket-level encryption mechanism, as opposed to protocol-
> level. It doesn't conflict with SHTTP except in terms of adding to
> the processing time.
> 
> I guess I don't see why SSL is so awful from a crypto standpoint.
> Could someone a bit more educated on the nuts and bolts clue me
> in on its weaknesses? As compared to other schemes, perhaps?

Frankly I don't think SSL is particularly weak cryptographically.  It has
gone through several revisions as various problems were pointed out.

The one thing I would note is that there is considerable known plaintext
being exchanged in the handshake.  This helps with key guessing and will
be the foundation for the SSL challenge that Adam Back is organising.
IMO at least some of this material could have been sent encrypted with
the public key so that an eavesdropper couldn't know it.  OTOH this
might have run afoul of the NSA's rules on export for at least the 40 bit
version since you'd have more than 40 bits of secrecy in effect.

SSL includes a 16 byte checksum with each packet.  IMO this is overkill
and wasteful for small packets.  One thing about SSL is that it
provides both secrecy and immunity to certain kinds of active attacks.
These big checksums include a sequence number and key information to
prevent replay attacks.  For some purposes you might be satisfied with
secrecy and not want to pay this overhead.

I think a lot of the criticism of SSL was based on the thought that it
would be obsoleted by the new IP secure protocols.  That may be true
eventually but SSL is here today, in use.  Order something from
Netscape and it is secured with SSL.  Buy the domestic version if you
want real security.  For IP, many of us we will have to wait until
the new IP protocols get built into our OS's and other infrastructure.

People have also objected to the use of the X.500 certificate approach.
But that seems to be de rigeur for any serious Internet standard these
days.  IMO the real solution is to come up with a PGP-like X.500
certificate maker so people can easily set themselves up as Certificate
Authorities and go about their business while the anal hierarchy
fans argue about liability.  Actually I think there is a PD certificate
maker around, possibily from Eric Young down under.

Hal




{% endraw %}
```

## Thread

+ Return to [July 1995](/archive/1995/07)

+ Return to "[Hal <hfinney<span>@</span>shell.portal.com>](/author/hal_hfinney_at_shell_portal_com_)"

+ 1995-07-20 (Thu, 20 Jul 95 10:23:43 PDT) - Re: Netscape the Big Win - _Hal \<hfinney@shell.portal.com\>_

