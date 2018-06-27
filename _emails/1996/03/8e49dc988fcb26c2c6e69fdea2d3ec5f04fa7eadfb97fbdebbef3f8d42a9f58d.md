---
layout: default
---

# 1996-03-11 - Re: FCC & Internet phones

## Header Data

From: Adam Shostack \<adam<span>@</span>lighthouse.homeport.org\><br>
To: wlkngowl@unix.asb.com (Mutant Rob)<br>
Message Hash: 8e49dc988fcb26c2c6e69fdea2d3ec5f04fa7eadfb97fbdebbef3f8d42a9f58d<br>
Message ID: \<199603100507.AAA02942@homeport.org\><br>
Reply To: \<199603100222.VAA06105@bb.hks.net\><br>
UTC Datetime: 1996-03-11 00:05:58 UTC<br>
Raw Date: Mon, 11 Mar 1996 08:05:58 +0800<br>

## Raw message

```
{% raw  %}From: Adam Shostack <adam@lighthouse.homeport.org>
Date: Mon, 11 Mar 1996 08:05:58 +0800
To: wlkngowl@unix.asb.com (Mutant Rob)
Subject: Re: FCC & Internet phones
In-Reply-To: <199603100222.VAA06105@bb.hks.net>
Message-ID: <199603100507.AAA02942@homeport.org>
MIME-Version: 1.0
Content-Type: text


Mutant Rob wrote:
| >         Q: Is it practically possible to find netphone traffic on a
| > generic network at any level above the source and target addresses?
| 
| Good question.

Presumably, the signal has a number of charictaristics.  Some of them
have a central switchboard, where preople go to set up calls.  Most
presumably use a mix of a UDP data connection and tcp for control
functions.  They all consist of high volume, long duration connections
(or data flows in the case of UDP.)  Many probably use a standardized
destination port.  They might use the urgent pointer to force data up
the stack quickly.

	In short, yes the data streams can be easily found, if one can
tap and grep a T3 in real time.

Adam


-- 
"It is seldom that liberty of any kind is lost all at once."
					               -Hume





{% endraw %}
```

## Thread

+ Return to [March 1996](/archive/1996/03)

+ Return to "[Adam Shostack <adam<span>@</span>lighthouse.homeport.org>](/authors/adam_shostack_adam_at_lighthouse_homeport_org_)"
+ Return to "[Loren James Rittle <rittle<span>@</span>comm.mot.com>](/authors/loren_james_rittle_rittle_at_comm_mot_com_)"
+ Return to "[Mutant Rob <wlkngowl<span>@</span>unix.asb.com>](/authors/mutant_rob_wlkngowl_at_unix_asb_com_)"
+ Return to "[Simon Spero <ses<span>@</span>tipper.oit.unc.edu>](/authors/simon_spero_ses_at_tipper_oit_unc_edu_)"

+ 1996-03-10 (Sun, 10 Mar 1996 12:00:44 +0800) - [Re: FCC & Internet phones](/archive/1996/03/8dd218f09386c63d1254835b46ca42a6d8835f17a957c9ea726da1b2dc267be8) - _Mutant Rob \<wlkngowl@unix.asb.com\>_
  + 1996-03-10 (Sun, 10 Mar 1996 13:31:07 +0800) - [Re: FCC & Internet phones](/archive/1996/03/46375f9bc9d7930f65c9f2fc5f4a7e7181e163fe2631630d6f3e60c45a4c80a7) - _Simon Spero \<ses@tipper.oit.unc.edu\>_
  + 1996-03-11 (Mon, 11 Mar 1996 08:05:58 +0800) - Re: FCC & Internet phones - _Adam Shostack \<adam@lighthouse.homeport.org\>_
    + 1996-03-12 (Tue, 12 Mar 1996 18:59:58 +0800) - [Re: FCC & Internet phones](/archive/1996/03/66463b274acb098d0c77535cee033fe0eeaa37ea8d4dacf98be91210110743c8) - _Loren James Rittle \<rittle@comm.mot.com\>_
      + 1996-03-13 (Wed, 13 Mar 1996 14:25:57 +0800) - [Re: FCC & Internet phones](/archive/1996/03/41658ee4ddc870ca54b4009c4fd0646046cc86d6fe0aa560fad373f9d45f616f) - _Adam Shostack \<adam@lighthouse.homeport.org\>_

