---
layout: default
---

# 1995-11-08 - Re: using pgp to make an otp

## Header Data

From: Derek Atkins \<warlord@MIT.EDU\><br>
To: Adam Shostack \<adam@lighthouse.homeport.org\><br>
Message Hash: a46013ef7d2bcc03cf48cd8f25fcbd1e6cedb5b03e99d9f6083fda6815aaaac0<br>
Message ID: \<199511070431.XAA17598@toxicwaste.media.mit.edu\><br>
Reply To: \<199511070407.XAA04557@homeport.org\><br>
UTC Datetime: 1995-11-08 21:33:52 UTC<br>
Raw Date: Thu, 9 Nov 1995 05:33:52 +0800<br>

## Raw message

```
{% raw  %}From: Derek Atkins <warlord@MIT.EDU>
Date: Thu, 9 Nov 1995 05:33:52 +0800
To: Adam Shostack <adam@lighthouse.homeport.org>
Subject: Re: using pgp to make an otp
In-Reply-To: <199511070407.XAA04557@homeport.org>
Message-ID: <199511070431.XAA17598@toxicwaste.media.mit.edu>
MIME-Version: 1.0
Content-Type: text/plain


> 	PGP output is not random enough to be used for a one time pad.
> The security of a OTP is *entirely* based on the quality of the random
> numbers; they should come from some strong generator.  Building good
> one time pads is tough, and usually not worth the effort.

No, however the output of "pgp +makerandom=XXX filename.dat" _IS_
random enough for an OTP.  The problem then becomes distributing this
data.

-derek




{% endraw %}
```

## Thread

+ Return to [November 1995](/archive/1995/11)

+ 1995-11-07 (Tue, 7 Nov 1995 11:03:53 +0800) - [RE: using pgp to make an otp](/archive/1995/11/e76e643c743afaac610b3d241d43cc4a5d5d3bc127f7385cdfbcd300eff9d241) - _amp \<Alan.Pugh@internetMCI.COM\>_
  + 1995-11-07 (Tue, 7 Nov 1995 13:35:43 +0800) - [Re: using pgp to make an otp](/archive/1995/11/13437d697a03f7d3dac31adfba2395ef376e02a9953ee5a9da082dc8bf85ab07) - _Adam Shostack \<adam@homeport.org\>_
    + 1995-11-08 (Thu, 9 Nov 1995 05:33:52 +0800) - Re: using pgp to make an otp - _Derek Atkins \<warlord@MIT.EDU\>_

