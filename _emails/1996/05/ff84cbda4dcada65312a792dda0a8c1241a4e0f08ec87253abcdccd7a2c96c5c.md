---
layout: default
---

# 1996-05-29 - Re: Remailers - What exists?

## Header Data

From: "E. ALLEN SMITH" \<EALLENSMITH@ocelot.Rutgers.EDU\><br>
To: stewarts@ix.netcom.com<br>
Message Hash: ff84cbda4dcada65312a792dda0a8c1241a4e0f08ec87253abcdccd7a2c96c5c<br>
Message ID: \<01I58Z1TPRZY8Y50T6@mbcl.rutgers.edu\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-05-29 04:33:43 UTC<br>
Raw Date: Wed, 29 May 1996 12:33:43 +0800<br>

## Raw message

```
{% raw  %}From: "E. ALLEN SMITH" <EALLENSMITH@ocelot.Rutgers.EDU>
Date: Wed, 29 May 1996 12:33:43 +0800
To: stewarts@ix.netcom.com
Subject: Re: Remailers - What exists?
Message-ID: <01I58Z1TPRZY8Y50T6@mbcl.rutgers.edu>
MIME-Version: 1.0
Content-Type: text/plain


From:	IN%"stewarts@ix.netcom.com"  "Bill Stewart" 28-MAY-1996 05:27:38.19

>It helps a lot to have an account that isn't your main email
>account, because it's going to get lots of junk in it
>that you want to discard most of, so you'd be better
>off without your real mail going there, unless you're
>a procmail wizard.

	A related question is about the cover traffic generators. With those,
I've gathered you've got the two choices of loops and nowhere-ending chains
(e.g., directing it to "nobody" on most systems). If it's done using a loop,
is there any way for a procmail script to determine that and toss them into
/dev/null?

>Mixmaster-style remailers are more secure than vanilla ones,
>but of course you need to use the Mixmaster client software
>to use them, which could be a problem if you're a DOS or Mac user.

	Or a VAX/VMS user; there are, I have been informed, enough
UNIX-specific system calls in Mixmaster that porting it isn't a trivial task. 

>- ability to mess with the sendmail logs
>- ability to tell the backup software not to back up your
>  spool directory (which would be Really Bad, especially
>  if your computer provider keeps backups forever.)
>  The alternative is to put it under /tmp somewhere,
>  and just make sure it recovers if too much stuff gets 
>  deleted by regular daemons.

	What mechanisms are available to make sure it will recover if /tmp
gets deleted? I suspect also that many ISPs might be quite willing not to
bother backing up some directory or another - it saves them time and space.
	Thanks,
	-Allen




{% endraw %}
```

## Thread

+ Return to [May 1996](/archive/1996/05)

+ 1996-05-29 (Wed, 29 May 1996 12:33:43 +0800) - Re: Remailers - What exists? - _"E. ALLEN SMITH" \<EALLENSMITH@ocelot.Rutgers.EDU\>_

