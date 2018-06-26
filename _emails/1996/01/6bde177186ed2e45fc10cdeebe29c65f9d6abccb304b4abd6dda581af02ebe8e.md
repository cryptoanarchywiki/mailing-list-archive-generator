---
layout: default
---

# 1996-01-23 - Re: Hack Java

## Header Data

From: Matt Miszewski \<crypto<span>@</span>midex.com\><br>
To: gback@facility.cs.utah.edu<br>
Message Hash: 6bde177186ed2e45fc10cdeebe29c65f9d6abccb304b4abd6dda581af02ebe8e<br>
Message ID: \<Pine.3.89.9601232225.B4292-0100000@shaq.midex.com\><br>
Reply To: \<199601231756.KAA03101@sal.cs.utah.edu\><br>
UTC Datetime: 1996-01-23 23:41:38 UTC<br>
Raw Date: Wed, 24 Jan 1996 07:41:38 +0800<br>

## Raw message

```
{% raw  %}From: Matt Miszewski <crypto@midex.com>
Date: Wed, 24 Jan 1996 07:41:38 +0800
To: gback@facility.cs.utah.edu
Subject: Re: Hack Java
In-Reply-To: <199601231756.KAA03101@sal.cs.utah.edu>
Message-ID: <Pine.3.89.9601232225.B4292-0100000@shaq.midex.com>
MIME-Version: 1.0
Content-Type: text/plain


On Tue, 23 Jan 1996 gback@facility.cs.utah.edu wrote:

[much elided stuff]

> > Now suppose, I fake a compiler (or I have a malicious compiler)
> > and I generate by hand malicious byte code such that
> > in the symbol tables, tricky_pointer and data have the same
> > offset.
> > 
> 

[more stuff taken out]

Godmar Said:

> 
> To my knowledge, the Java, and Java bytecode does not imply
> any memory layout. I doubt it makes sense to demand to check
> that 'offset do not overlap in memory'.
> 

Both of you are correct if you look carefully at the assumptions.  Rich 
assumes that you have a 'malicious compiler'.  Godmar is right that Java 
does not utilize pointers in the byte code.  What would make the entire 
scenario work is a malicious interpreter or a 'NotJava Browser'(TM) that 
allowed malicious code to be executed.  Couple a bad compiler and a bad 
interpreter and you are in buisness (nasty business that is).

Matt




{% endraw %}
```

## Thread

+ Return to [January 1996](/archive/1996/01)

+ Return to "[gback<span>@</span>facility.cs.utah.edu](/author/gback_at_facility_cs_utah_edu)"
+ Return to "[heesen<span>@</span>zpr.uni-koeln.de (Rainer Heesen)](/author/heesen_at_zpr_unikoeln_de_rainer_heesen_)"
+ Return to "[Matt Miszewski <crypto<span>@</span>midex.com>](/author/matt_miszewski_crypto_at_midex_com_)"
+ Return to "[Matthew Sheppard <Matthew.Sheppard<span>@</span>Comp.VUW.AC.NZ>](/author/matthew_sheppard_matthew_sheppard_at_comp_vuw_ac_nz_)"
+ Return to "[Rich Salz <rsalz<span>@</span>osf.org>](/author/rich_salz_rsalz_at_osf_org_)"
+ Return to "[Simon Spero <ses<span>@</span>tipper.oit.unc.edu>](/author/simon_spero_ses_at_tipper_oit_unc_edu_)"

+ 1996-01-25 (Thu, 25 Jan 1996 18:07:52 +0800) - [Hack Java](/archive/1996/01/af3cf466c88eb6d921167c1a0f9018c7b19523a984d33505834cf9035ec2ad8f) - _Rich Salz \<rsalz@osf.org\>_
  + 1996-01-23 (Wed, 24 Jan 1996 02:33:42 +0800) - [Re: Hack Java](/archive/1996/01/f589b0a50e1da44302f7fc0aa47985c58a9e15df09c60982df98d595be5c85c1) - _gback@facility.cs.utah.edu_
    + 1996-01-23 (Wed, 24 Jan 1996 07:41:38 +0800) - Re: Hack Java - _Matt Miszewski \<crypto@midex.com\>_
  + 1996-01-23 (Wed, 24 Jan 1996 06:22:05 +0800) - [Re: Hack Java](/archive/1996/01/ffc19185c6c38224f03b974dab05841d0b6b2f0c9f5fff93f2ee0f718f374a9b) - _Simon Spero \<ses@tipper.oit.unc.edu\>_
  + 1996-01-24 (Wed, 24 Jan 1996 14:05:38 +0800) - [Re: Hack Java](/archive/1996/01/71f536405244aba6358ed5960f54484ae6dd42a4a00830c0f32ed193d5da3996) - _Matthew Sheppard \<Matthew.Sheppard@Comp.VUW.AC.NZ\>_
    + 1996-01-24 (Wed, 24 Jan 1996 17:07:39 +0800) - [Re: Hack Java](/archive/1996/01/b5265f2820a79f6a069ffd26383de00b499b39db80ec9606835c978a75479f7f) - _heesen@zpr.uni-koeln.de (Rainer Heesen)_

