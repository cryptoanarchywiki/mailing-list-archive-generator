---
layout: default
---

# 1996-01-23 - Re: Hack Java

## Header Data

From: Matt Miszewski \<crypto@midex.com\><br>
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

+ 1996-01-25 (Thu, 25 Jan 1996 18:07:52 +0800) - [Hack Java](/archive/1996/01/af3cf466c88eb6d921167c1a0f9018c7b19523a984d33505834cf9035ec2ad8f) - _Rich Salz \<rsalz@osf.org\>_
  + 1996-01-23 (Wed, 24 Jan 1996 02:33:42 +0800) - [Re: Hack Java](/archive/1996/01/f589b0a50e1da44302f7fc0aa47985c58a9e15df09c60982df98d595be5c85c1) - _gback@facility.cs.utah.edu_
    + 1996-01-23 (Wed, 24 Jan 1996 07:41:38 +0800) - Re: Hack Java - _Matt Miszewski \<crypto@midex.com\>_

