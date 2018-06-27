---
layout: default
---

# 1993-08-28 - Attacks on remailers (LONG)

## Header Data

From: b44729<span>@</span>achilles.ctd.anl.gov (Samuel Pigg)<br>
To: cypherpunks@toad.com<br>
Message Hash: 298bea12cac3b56d2e28bfccd250db7ce3ecf7bcd9972a1c9ee2e14bf44aec09<br>
Message ID: \<9308280446.AA01688@achilles.ctd.anl.gov\><br>
Reply To: \<199308280353.AA02675@gaea.synopsys.com\><br>
UTC Datetime: 1993-08-28 04:48:30 UTC<br>
Raw Date: Fri, 27 Aug 93 21:48:30 PDT<br>

## Raw message

```
{% raw  %}From: b44729@achilles.ctd.anl.gov (Samuel Pigg)
Date: Fri, 27 Aug 93 21:48:30 PDT
To: cypherpunks@toad.com
Subject: Attacks on remailers (LONG)
In-Reply-To: <199308280353.AA02675@gaea.synopsys.com>
Message-ID: <9308280446.AA01688@achilles.ctd.anl.gov>
MIME-Version: 1.0
Content-Type: text/plain



>>>>> On Fri, 27 Aug 93 20:53:51 -0700, eric@Synopsys.COM said:

>>>>> On Fri, 27 Aug 93 05:52:43 CDT, b44729@achilles.ctd.anl.gov (Samuel Pigg) said:

Samuel> Correct me if I'm wrong, but as I see it, there are two goals
Samuel> for the remailers:

Samuel> (1) 	Anonymous addresses to which mail can be sent, but the recipient
Samuel> 	is unknown and cannot be determined (receiving anonymous mail).

Samuel> (2)	The ability to send mail to someone without anyone
Samuel> (including 	the recipient) determing that you did so
Samuel> (sending anonymous mail).

Samuel> Number 2 can be mostly taken care of with nested encryption of
Samuel> mail headers.

	[...]

Samuel> To construct an anonymous address block might be something like:

Samuel> 	Anonymous Anne wants an anonymous address.
Samuel> 	First she generates a set of N keys (IDEA, DES or .......

	eric> That's basically the way SASE works.  It's important
	eric> that some of the keys be public key pairs, however; as
	eric> you need to be able to publish one half of a key, and
	eric> seal the other half for an unpublished remailer to
	eric> decrypt with.

I don't see why some of the keys need to be public key pairs.
The intermediate encryptions done by the remailers are only to be
undone by the anonymous recipient correct?

So why would one part of the keys need to be published?
(the anonymous address block would have these keys sealed in the various
nested encryption levels, as you said.)

	eric> One thing is certain, these protocols are not simple.
	eric> We definitely need people thinking about them...

..and discussing them! (as we are doing now.)

-Sam





{% endraw %}
```

## Thread

+ Return to [August 1993](/archive/1993/08)

+ Return to "[b44729<span>@</span>achilles.ctd.anl.gov (Samuel Pigg)](/authors/b44729_at_achilles_ctd_anl_gov_samuel_pigg_)"
+ Return to "[eric<span>@</span>Synopsys.COM](/authors/eric_at_synopsys_com)"
+ Return to "[hfinney<span>@</span>shell.portal.com](/authors/hfinney_at_shell_portal_com)"
+ Return to "[hughes<span>@</span>ah.com (Eric Hughes)](/authors/hughes_at_ah_com_eric_hughes_)"
+ Return to "[Karl Lui Barrus <klbarrus<span>@</span>owlnet.rice.edu>](/authors/karl_lui_barrus_klbarrus_at_owlnet_rice_edu_)"

+ 1993-08-27 (Thu, 26 Aug 93 22:25:53 PDT) - [Attacks on remailers](/archive/1993/08/2d0143add3aefa25c1b4c6687cf1dbd4cb2bbf92c8501de40438fe312ba46dcb) - _hfinney@shell.portal.com_
  + 1993-08-27 (Fri, 27 Aug 93 03:55:54 PDT) - [Re: Attacks on remailers (LONG)](/archive/1993/08/e39512221a01dd44ed892180469fdf0cfbcf81e535953dd5ddfb9e1c6a72270a) - _b44729@achilles.ctd.anl.gov (Samuel Pigg)_
    + 1993-08-27 (Fri, 27 Aug 93 10:22:51 PDT) - [REMAIL: Attacks on remailers](/archive/1993/08/7efa6aa6db3e901b579d14ce0ca029b750f10a671a6350549c5241dd2b009b02) - _hughes@ah.com (Eric Hughes)_
      + 1993-08-28 (Sat, 28 Aug 93 03:03:02 PDT) - [Re: REMAIL: Attacks on remailers (LONG (again))](/archive/1993/08/d0d8ed987740b365e2f1af1de8f011ff88f87a0752126b68726cf18b1c87d0b0) - _b44729@achilles.ctd.anl.gov (Samuel Pigg)_
        + 1993-08-30 (Mon, 30 Aug 93 07:23:44 PDT) - [REMAIL: Attacks on remailers](/archive/1993/08/50ae30dff5f57d385214d57d832cec272b1e1cdc3dfc6c13e6ba05b898f514c6) - _Karl Lui Barrus \<klbarrus@owlnet.rice.edu\>_
          + 1993-08-31 (Tue, 31 Aug 93 10:54:04 PDT) - [REMAIL: Attacks on remailers](/archive/1993/08/01d6d5f82705881d3a447c2e66fa0713e99cf0f4c088cf9a998494bd6363a7ac) - _hughes@ah.com (Eric Hughes)_
    + 1993-08-28 (Fri, 27 Aug 93 20:56:02 PDT) - [Re: Attacks on remailers (LONG)](/archive/1993/08/44bab7b05ee301f704f2274658d5033cc62f0f9e4af039c820ddf1993dbdd9f6) - _eric@Synopsys.COM_
      + 1993-08-28 (Fri, 27 Aug 93 21:48:30 PDT) - Attacks on remailers (LONG) - _b44729@achilles.ctd.anl.gov (Samuel Pigg)_

