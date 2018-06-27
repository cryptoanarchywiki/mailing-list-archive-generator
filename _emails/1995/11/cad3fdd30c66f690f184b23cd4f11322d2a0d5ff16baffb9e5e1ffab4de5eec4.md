---
layout: default
---

# 1995-11-05 - Re: /dev/random - using up entropy?

## Header Data

From: Wei Dai \<weidai<span>@</span>eskimo.com\><br>
To: Bill Stewart \<stewarts@ix.netcom.com\><br>
Message Hash: cad3fdd30c66f690f184b23cd4f11322d2a0d5ff16baffb9e5e1ffab4de5eec4<br>
Message ID: \<Pine.SUN.3.91.951104163531.19656J-100000@eskimo.com\><br>
Reply To: \<199511042352.PAA07554@ix4.ix.netcom.com\><br>
UTC Datetime: 1995-11-05 01:10:47 UTC<br>
Raw Date: Sun, 5 Nov 1995 09:10:47 +0800<br>

## Raw message

```
{% raw  %}From: Wei Dai <weidai@eskimo.com>
Date: Sun, 5 Nov 1995 09:10:47 +0800
To: Bill Stewart <stewarts@ix.netcom.com>
Subject: Re: /dev/random - using up entropy?
In-Reply-To: <199511042352.PAA07554@ix4.ix.netcom.com>
Message-ID: <Pine.SUN.3.91.951104163531.19656J-100000@eskimo.com>
MIME-Version: 1.0
Content-Type: text/plain


On Sat, 4 Nov 1995, Bill Stewart wrote:

> Most of the designs I've seen look like this:
>         A Reservoir of entropy R = R1....Rn, where n is large, 1024 or 4096
>         An input stream I = I1....Ik, which is mixed into R
>         A mixing function F which is used to mix R <= F(R,I) 
>                 for some chunk of I, possibly empty.
>         A hash function H, typically MD5.
>         An output O = O1...Om = H(R), and E gets mixed after every output.
>                 (These are capital-o, not zero...)

I believe PGP uses this approach.  An implementation of it can also be
found in Crypto++ as randpool.cpp. 





{% endraw %}
```

## Thread

+ Return to [November 1995](/archive/1995/11)

+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/authors/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "["Theodore Ts'o" <tytso<span>@</span>MIT.EDU>](/authors/theodore_tso_tytso_at_mit_edu_)"
+ Return to "[Wei Dai <weidai<span>@</span>eskimo.com>](/authors/wei_dai_weidai_at_eskimo_com_)"

+ 1995-11-05 (Sun, 5 Nov 1995 08:08:41 +0800) - [/dev/random - using up entropy?](/archive/1995/11/9a1b5ac42ae31033a832e43686052c7593c7e3aa9153d04dcd2756281c4c8a5c) - _Bill Stewart \<stewarts@ix.netcom.com\>_
  + 1995-11-05 (Sun, 5 Nov 1995 09:10:47 +0800) - Re: /dev/random - using up entropy? - _Wei Dai \<weidai@eskimo.com\>_
  + 1995-11-07 (Tue, 7 Nov 1995 12:18:42 +0800) - [Re: /dev/random - using up entropy?](/archive/1995/11/8a45ec9c57cad23113b928eba8062a7ae4c43451d99c130f7f9507c9e64a5415) - _"Theodore Ts'o" \<tytso@MIT.EDU\>_

