---
layout: default
---

# 1996-08-29 - Elliptic Curve Y**2 = x**3 + a * x**2 + b

## Header Data

From: trollins<span>@</span>interactive.visa.com (Tom Rollins)<br>
To: cypherpunks@toad.com<br>
Message Hash: 002ce9e11dcb9b1e2debd88edbb26baeb1acad236c0caf62723871a6fad0f865<br>
Message ID: \<199608291905.PAA16350@rootboy.interactive.visa.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-08-29 23:13:53 UTC<br>
Raw Date: Fri, 30 Aug 1996 07:13:53 +0800<br>

## Raw message

```
{% raw  %}From: trollins@interactive.visa.com (Tom Rollins)
Date: Fri, 30 Aug 1996 07:13:53 +0800
To: cypherpunks@toad.com
Subject: Elliptic Curve Y**2 = x**3 + a * x**2 + b
Message-ID: <199608291905.PAA16350@rootboy.interactive.visa.com>
MIME-Version: 1.0
Content-Type: text


Hello all,

I have a math question concerning implementation of elliptic
curve systems. In coding some elliptic curve source, I
need to pick a random point on the following elliptic
curve in field F_p where p is a prime number.

       Y**2 = x**3 + a * x**2 + b
       where 4a**3 + 27b**2 is not equal to 0 mod p

In selecting a random point, I pick a random value for
x in the range 0 < x < p, compute the right hand side
of the equation and find myself needing to take the
square root for the two solutions.

Questions are:

  1: How can I take the suqare root mod p ?

  2: How to determine if a solution exists for a
     selected value of x ?

  3: Is the a simpler method than find a square root ?

Thanks for any ideas you may have about this...
-tom





{% endraw %}
```

## Thread

+ Return to [August 1996](/archive/1996/08)
+ Return to [September 1996](/archive/1996/09)

+ Return to "[chen<span>@</span>chen.com (Mark Chen)](/authors/chen_at_chen_com_mark_chen_)"
+ Return to "[Justin Card <Wyntermute<span>@</span>worldnet.att.net>](/authors/justin_card_wyntermute_at_worldnet_att_net_)"
+ Return to "[trollins<span>@</span>interactive.visa.com (Tom Rollins)](/authors/trollins_at_interactive_visa_com_tom_rollins_)"
+ Return to "[Wei Dai <weidai<span>@</span>eskimo.com>](/authors/wei_dai_weidai_at_eskimo_com_)"

+ 1996-08-29 (Fri, 30 Aug 1996 07:13:53 +0800) - Elliptic Curve Y**2 = x**3 + a * x**2 + b - _trollins@interactive.visa.com (Tom Rollins)_
  + 1996-08-29 (Fri, 30 Aug 1996 07:37:26 +0800) - [Re: Elliptic Curve Y**2 = x**3 + a * x**2 + b](/archive/1996/08/0351784cd22765b68bebe625d0ab446497d17f6dc3e549a6e355eb9d73561b78) - _Wei Dai \<weidai@eskimo.com\>_
    + 1996-09-01 (Sun, 1 Sep 1996 12:43:41 +0800) - [Re: Elliptic Curve Y**2 = x**3 + a * x**2 + b](/archive/1996/09/5579f5a691e48ca692194a618b6e2a5be31fb1baf364843b7ad88029bcf5ecf7) - _chen@chen.com (Mark Chen)_
  + 1996-08-30 (Fri, 30 Aug 1996 17:30:09 +0800) - [Re: Elliptic Curve Y**2 = x**3 + a * x**2 + b](/archive/1996/08/41be00b0c7c71012af99c541052c3880511127c3cb9c8a1f8aede2dfdefd7c6c) - _Justin Card \<Wyntermute@worldnet.att.net\>_
    + 1996-08-30 (Sat, 31 Aug 1996 01:14:47 +0800) - [Re: Elliptic Curve Y**2 = x**3 + a * x**2 + b](/archive/1996/08/f581318633e8b83cafdcf63f721697e10daa467175b6ad82bf8edc1d748b118e) - _trollins@interactive.visa.com (Tom Rollins)_

