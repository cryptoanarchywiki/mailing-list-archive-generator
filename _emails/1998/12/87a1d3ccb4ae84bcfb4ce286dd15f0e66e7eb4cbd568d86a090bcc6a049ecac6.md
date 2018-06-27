---
layout: default
---

# 1998-12-03 - Re: open-pgp / s/mime interoperability

## Header Data

From: pgut001<span>@</span>cs.auckland.ac.nz (Peter Gutmann)<br>
To: aba@dcs.ex.ac.uk<br>
Message Hash: 87a1d3ccb4ae84bcfb4ce286dd15f0e66e7eb4cbd568d86a090bcc6a049ecac6<br>
Message ID: \<91269213708678@cs26.cs.auckland.ac.nz\><br>
Reply To: _N/A_<br>
UTC Datetime: 1998-12-03 14:01:30 UTC<br>
Raw Date: Thu, 3 Dec 1998 22:01:30 +0800<br>

## Raw message

```
{% raw  %}From: pgut001@cs.auckland.ac.nz (Peter Gutmann)
Date: Thu, 3 Dec 1998 22:01:30 +0800
To: aba@dcs.ex.ac.uk
Subject: Re: open-pgp / s/mime interoperability
Message-ID: <91269213708678@cs26.cs.auckland.ac.nz>
MIME-Version: 1.0
Content-Type: text/plain



Adam Back <aba@dcs.ex.ac.uk> writes:
>Peter Gutmann writes:
>>>open-pgp public keys aren't based on X.509 keys, so I would've thought
>>>s/mime implementation would barf on them.  
>> 
>>Actually S/MIME *could* support the use of PGP keys, but there's a field
>>(the SubjectKeyIdentifier) missing from the CMS SignerInfo which prevents
>>this.  
 
>Surely this in itself should be a compelling argument for inclusion of the 
>SubjectKeyIdentifier?  
 
I'm trying to get this adopted for CMS, the underlying data format for 
S/MIME.  The silly thing about this is that alternative key identifiers (like 
PGP keys) were going to be included in RSADSI's PKCS7v2, but aren't included 
in the IETF version of the same thing.  The result is that you have a private 
company going out of its way to accomodate open standards, and the IETF going 
out of its way to lock them out.  Weird.
 
>If it allows conversion of PGP keys into S/MIME X.509 keys.
 
You don't need this conversion, with key identifiers you can use both SPKI and 
PGP keys directly within S/MIME.  There's no need to convert them into an 
X.509-like format first.
 
Peter.




{% endraw %}
```

## Thread

+ Return to [December 1998](/archive/1998/12)

+ Return to "[pgut001<span>@</span>cs.auckland.ac.nz (Peter Gutmann)](/authors/pgut001_at_cs_auckland_ac_nz_peter_gutmann_)"

+ 1998-12-03 (Thu, 3 Dec 1998 22:01:30 +0800) - Re: open-pgp / s/mime interoperability - _pgut001@cs.auckland.ac.nz (Peter Gutmann)_

