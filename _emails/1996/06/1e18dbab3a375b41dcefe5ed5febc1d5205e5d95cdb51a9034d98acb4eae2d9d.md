---
layout: default
---

# 1996-06-05 - S/MIME key sizes

## Header Data

From: Raph Levien \<raph<span>@</span>cs.berkeley.edu\><br>
To: Lucky Green \<shamrock@netcom.com\><br>
Message Hash: 1e18dbab3a375b41dcefe5ed5febc1d5205e5d95cdb51a9034d98acb4eae2d9d<br>
Message ID: \<31B45529.747B@cs.berkeley.edu\><br>
Reply To: \<v02120d0badd919d1ddb3@[192.0.2.1]\><br>
UTC Datetime: 1996-06-05 00:59:30 UTC<br>
Raw Date: Wed, 5 Jun 1996 08:59:30 +0800<br>

## Raw message

```
{% raw  %}From: Raph Levien <raph@cs.berkeley.edu>
Date: Wed, 5 Jun 1996 08:59:30 +0800
To: Lucky Green <shamrock@netcom.com>
Subject: S/MIME key sizes
In-Reply-To: <v02120d0badd919d1ddb3@[192.0.2.1]>
Message-ID: <31B45529.747B@cs.berkeley.edu>
MIME-Version: 1.0
Content-Type: text/plain


Lucky Green wrote:
> 
> At 15:58 6/3/96, Raph Levien wrote:
> 
> >   Basically, an exportable S/MIME client can transmit messages up to
> >1024/40 bit RSA/RC2 (or RSA/DES), and receive messages up to 512/64 bit
> >RSA/RC2 (or RSA/DES, but in the latter case I would imagine it's actually
> >restricted to 512/56 because of the keysize of DES). Note that the
> >asymmetry actually points in different directions for the public and
> >symmetric keysizes.
> 
> What will be the maximum keysize for a domestic encryption client? It it is
> larger than 1024 bits, there will be interoperability problems with foreign
> clients. If the domestic client is limited to 1024 bits, it would set a bad
> precedence, since it would effectively require that the encryption key is
> smaller than the largest signature key.

   There is no restriction on non-export keysize, as far as I know. Of 
course, if you do use a key larger than 1024 bits, then export clients 
can not encrypt to you. I don't consider this to be a serious 
limitation. I'd far rather see an error message of "cannot encrypt to 
client - your software is crippled" than "encrypting to recipient with 
super-duper 40-bit cipher". The more crippled the export version appears 
to be, the more pressure there is to upgrade to a non-export version.

   I object to the word "domestic" to refer to non-crippled encryption 
programs. I use "non-export" because that seems least likely to cause 
confusion. Keep in mind that clients developed outside the US are also 
non-crippled. The word "domestic" seems to unfairly exclude them.

Raph




{% endraw %}
```

## Thread

+ Return to [June 1996](/archive/1996/06)

+ Return to "[Raph Levien <raph<span>@</span>cs.berkeley.edu>](/author/raph_levien_raph_at_cs_berkeley_edu_)"
+ Return to "[shamrock<span>@</span>netcom.com (Lucky Green)](/author/shamrock_at_netcom_com_lucky_green_)"

+ 1996-06-04 (Tue, 4 Jun 1996 11:35:42 +0800) - [Re: NRC Session Hiss](/archive/1996/06/0f637f10d9f20d70d5858a5728550c46f40d750e084d4b6306e0a55f4612da13) - _shamrock@netcom.com (Lucky Green)_
  + 1996-06-05 (Wed, 5 Jun 1996 08:59:30 +0800) - S/MIME key sizes - _Raph Levien \<raph@cs.berkeley.edu\>_

