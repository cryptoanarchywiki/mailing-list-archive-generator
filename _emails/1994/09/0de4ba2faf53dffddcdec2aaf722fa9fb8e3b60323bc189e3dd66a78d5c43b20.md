---
layout: default
---

# 1994-09-28 - Re: 3DES

## Header Data

From: Jim Gillogly \<jim<span>@</span>acm.org\><br>
To: cypherpunks@toad.com<br>
Message Hash: 0de4ba2faf53dffddcdec2aaf722fa9fb8e3b60323bc189e3dd66a78d5c43b20<br>
Message ID: \<9409282204.AA01197@mycroft.rand.org\><br>
Reply To: \<9409282126.AA00174@focis.sda.cbis.COM\><br>
UTC Datetime: 1994-09-28 22:04:44 UTC<br>
Raw Date: Wed, 28 Sep 94 15:04:44 PDT<br>

## Raw message

```
{% raw  %}From: Jim Gillogly <jim@acm.org>
Date: Wed, 28 Sep 94 15:04:44 PDT
To: cypherpunks@toad.com
Subject: Re: 3DES
In-Reply-To: <9409282126.AA00174@focis.sda.cbis.COM>
Message-ID: <9409282204.AA01197@mycroft.rand.org>
MIME-Version: 1.0
Content-Type: text/plain



> pstemari@bismark.cbis.com (Paul J. Ste. Marie) writes:
> triple DES uses:

> Eabc(x) = Ea(Db(Ec(x)))

> as opposed to:

> Eabc(x) = Ea(Eb(Ec(x)))

> in order to preserve some symmetry properties.  Can anyone give a
> better explanation?

OK -- if you want to retain compatibility with old 56-bit DES chips
in your same network, you can set a = b = c and get:

  Eaaa(x) = Ea(Da(Ea(x)))

using the first form, which reduces to Ea(x), or a single 56-bit DES
encryption instead of the 168 bits your TripleDES chip can handle.  The
second form doesn't have this property or any other useful property other
than standalone security, since DES isn't a group.

	Jim Gillogly
	Highday, 7 Winterfilth S.R. 1994, 22:03




{% endraw %}
```

## Thread

+ Return to [September 1994](/archive/1994/09)

+ Return to "[Jim Gillogly <jim<span>@</span>acm.org>](/authors/jim_gillogly_jim_at_acm_org_)"
+ Return to "[mccoy<span>@</span>io.com (Jim McCoy)](/authors/mccoy_at_io_com_jim_mccoy_)"
+ Return to "[Phil Karn <karn<span>@</span>qualcomm.com>](/authors/phil_karn_karn_at_qualcomm_com_)"
+ Return to "[pstemari<span>@</span>bismark.cbis.com (Paul J. Ste. Marie)](/authors/pstemari_at_bismark_cbis_com_paul_j_ste_marie_)"

+ 1994-09-28 (Wed, 28 Sep 94 14:26:46 PDT) - [3DES](/archive/1994/09/806e5b20585f871e786b1c4237074be320c7308453bcd7d451bbc34b33d9a100) - _pstemari@bismark.cbis.com (Paul J. Ste. Marie)_
  + 1994-09-28 (Wed, 28 Sep 94 15:00:52 PDT) - [Re: 3DES](/archive/1994/09/2380e8290008fe0134eb55b3eecdc6784cd933980e629d57257731d7c6451ca7) - _Phil Karn \<karn@qualcomm.com\>_
  + 1994-09-28 (Wed, 28 Sep 94 15:04:44 PDT) - Re: 3DES - _Jim Gillogly \<jim@acm.org\>_
  + 1994-09-28 (Wed, 28 Sep 94 15:31:29 PDT) - [Re: 3DES](/archive/1994/09/6798ef2bc0f10bf5b7ed528e7c13fb4c6c0e303acdf8586d5b92f5ab53554e49) - _mccoy@io.com (Jim McCoy)_

