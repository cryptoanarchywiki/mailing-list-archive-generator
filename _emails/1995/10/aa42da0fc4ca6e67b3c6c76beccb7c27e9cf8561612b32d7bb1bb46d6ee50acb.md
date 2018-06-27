---
layout: default
---

# 1995-10-19 - Re: digital cash and identity disclosure

## Header Data

From: chen<span>@</span>intuit.com (Mark Chen)<br>
To: cypherpunks@toad.com (cypherpunks)<br>
Message Hash: aa42da0fc4ca6e67b3c6c76beccb7c27e9cf8561612b32d7bb1bb46d6ee50acb<br>
Message ID: \<9510192017.AA26270@doom\><br>
Reply To: \<acabe4df3f021004b9f5@[205.199.118.202]\><br>
UTC Datetime: 1995-10-19 20:20:57 UTC<br>
Raw Date: Thu, 19 Oct 95 13:20:57 PDT<br>

## Raw message

```
{% raw  %}From: chen@intuit.com (Mark Chen)
Date: Thu, 19 Oct 95 13:20:57 PDT
To: cypherpunks@toad.com (cypherpunks)
Subject: Re: digital cash and identity disclosure
In-Reply-To: <acabe4df3f021004b9f5@[205.199.118.202]>
Message-ID: <9510192017.AA26270@doom>
MIME-Version: 1.0
Content-Type: text/plain


Tim wrote:

> "Double spending" detection is a REAL MESS. That's my basic conclusion. It
> tends to require schemes for going after double spenders, it tends to make
> identity-revealing attacks possible (such as the attack I alluded to, and
> that Hal more completely describes), and it's INELEGANT.
> 
> "Immediate clearing" is much more elegant, and is, I think, truer to the
> spirit of "annonymous digital cash" than most of these other schemes are.
> (Grep the FAQ for "online" or "online clearing" or "clearing" and you
> should find some stuff. Also, several articles--including one recently by
> me, about a month ago--go into the differences between the types of
> clearing.)

I also suggest taking a look at Stefan Brands' solution, which, while
requiring hardware, has some favorable properties.  Among these are:

   - prior restraint of double spending through hardware-based
   "secret-key certificates"

   - in the case of hardware tampering, double spenders are traceable
   as in Chaum's system; however, the protocol used to achieve this is
   much more efficient than Chaum's "cut-and-choose"

   - no possibility of a subliminal channel between the
   tamper-resistant device and the payee or bank


--
Mark Chen 
chen@intuit.com
415/329-6913
finger for PGP public key
D4 99 54 2A 98 B1 48 0C  CF 95 A5 B0 6E E0 1E 1D



{% endraw %}
```

## Thread

+ Return to [October 1995](/archive/1995/10)

+ Return to "[Bryce <wilcoxb<span>@</span>nag.cs.colorado.edu>](/authors/bryce_wilcoxb_at_nag_cs_colorado_edu_)"
+ Return to "[chen<span>@</span>intuit.com (Mark Chen)](/authors/chen_at_intuit_com_mark_chen_)"
+ Return to "[Hal <hfinney<span>@</span>shell.portal.com>](/authors/hal_hfinney_at_shell_portal_com_)"
+ Return to "[tcmay<span>@</span>got.net (Timothy C. May)](/authors/tcmay_at_got_net_timothy_c_may_)"

+ 1995-10-19 (Thu, 19 Oct 95 11:26:28 PDT) - [Re: digital cash and identity disclosure](/archive/1995/10/3e3945bd506dc2ae2ef4d8c1850961dd590d230b2a7fc88dd0321bcf91a2472f) - _tcmay@got.net (Timothy C. May)_
  + 1995-10-19 (Thu, 19 Oct 95 12:49:07 PDT) - [Re: digital cash and identity disclosure](/archive/1995/10/aaffb1038aca1615900181cb1c4ab293cc8fa78bac605283e978892585538028) - _Bryce \<wilcoxb@nag.cs.colorado.edu\>_
  + 1995-10-19 (Thu, 19 Oct 95 13:01:33 PDT) - [Polymorphic e-cash schemes  was: digital cash and identity disclosure](/archive/1995/10/6b7f123e67544ddfbd78941e9cc45a4cf99702d249dbedd3517e5fb78c63d291) - _Bryce \<wilcoxb@nag.cs.colorado.edu\>_
    + 1995-10-20 (Fri, 20 Oct 95 07:05:01 PDT) - [Re: Polymorphic e-cash schemes was: digital cash and identity disclosure](/archive/1995/10/d046c610c63101c6b8f43446300a2ee2decc4d31f5dc466784a996c77073aac9) - _Hal \<hfinney@shell.portal.com\>_
  + 1995-10-19 (Thu, 19 Oct 95 13:20:57 PDT) - Re: digital cash and identity disclosure - _chen@intuit.com (Mark Chen)_

