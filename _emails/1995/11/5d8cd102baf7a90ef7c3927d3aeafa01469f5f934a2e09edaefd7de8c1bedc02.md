---
layout: default
---

# 1995-11-06 - re:using PGP only for digital signatures

## Header Data

From: Bill Stewart \<stewarts<span>@</span>ix.netcom.com\><br>
To: James Black \<black@eng.usf.edu\><br>
Message Hash: 5d8cd102baf7a90ef7c3927d3aeafa01469f5f934a2e09edaefd7de8c1bedc02<br>
Message ID: \<199511062107.NAA29648@ix5.ix.netcom.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-11-06 21:41:42 UTC<br>
Raw Date: Tue, 7 Nov 1995 05:41:42 +0800<br>

## Raw message

```
{% raw  %}From: Bill Stewart <stewarts@ix.netcom.com>
Date: Tue, 7 Nov 1995 05:41:42 +0800
To: James Black <black@eng.usf.edu>
Subject: re:using PGP only for digital signatures
Message-ID: <199511062107.NAA29648@ix5.ix.netcom.com>
MIME-Version: 1.0
Content-Type: text/plain


At 04:12 PM 11/4/95 -0500, James Black <black@eng.usf.edu> wrote:
>Hello,
>  I am in a discussion (during the week) with a system administrator 
>about seeing if we can just make PGP publically available to everyone, 
>but now the discussion seems to be to just allow PGP to do digital 
>signatures, and I don't think that is the best choice, then.  They are 
>not against PGP being used, but there are legal issues as to whether they 
>can offer it to everyone, as some students are international students, 
>and are not allowed to use the version for the US, or so I have been 
>informed, so now I need to see if we can have the international version, 
>so these students can use it. :(
>  Is there any good programs (for the Unix, SunOS) that just does digital 
>signature encryption?  What they are trying to do is make certain that no 
>one can send a message to anyone, claim to be in the faculty, and cause 
>problems that way.  My position is just a student programmer, but I am 
>trying to learn as much as I can, to answer questions and deal with problems.

Yeah, there's RIPEM-SIG, which is approved for export so you can even give it
to your non-Yankee students, and it's compatible with the RIPEM secure email
stuff.
So your US students, and anyone else who wants to download the software from
England, can send secure email, and everybody can check the signatures.
I'm not sure if RIPEM-SIG has caught up with the features in the latest
versions of RIPEM, which include an X.509 variant on Web of Trust.

Somebody else has brought up the insecurity of using security software
on multi-user machines, where the system administrator or anybody who cracks
root can steal your passphrases and even replace the trustable software with
trojan-horse versions; your students will be safer if they only trust stuff
running on PCs from software they've verified themselves.  But you can at least
do signature-checking safely on a multi-user machine if the software is
protected adequately.
#---
#                                       Thanks;  Bill
# Bill Stewart, Freelance Information Architect, stewarts@ix.netcom.com
# Phone +1-510-247-0664 Pager/Voicemail 1-408-787-1281
#---





{% endraw %}
```

## Thread

+ Return to [November 1995](/archive/1995/11)

+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/author/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "[James Black <black<span>@</span>eng.usf.edu>](/author/james_black_black_at_eng_usf_edu_)"

+ 1995-11-06 (Tue, 7 Nov 1995 05:41:42 +0800) - re:using PGP only for digital signatures - _Bill Stewart \<stewarts@ix.netcom.com\>_
  + 1995-11-07 (Tue, 7 Nov 1995 11:55:32 +0800) - [re:using PGP only for digital signatures](/archive/1995/11/70bb6981c5e30644377d6d79a47fbc0dfb6cb0a9f3cf9f67af532bc30f2151ea) - _James Black \<black@eng.usf.edu\>_

