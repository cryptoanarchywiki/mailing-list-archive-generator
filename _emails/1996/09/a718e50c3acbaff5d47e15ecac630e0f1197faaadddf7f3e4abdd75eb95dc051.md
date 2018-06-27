---
layout: default
---

# 1996-09-03 - [BEATING A NOT QUITE DEAD] Passive Trojan [HORSE] (was:Re: HAZ-MAT virus)

## Header Data

From: Bill Stewart \<stewarts<span>@</span>ix.netcom.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: a718e50c3acbaff5d47e15ecac630e0f1197faaadddf7f3e4abdd75eb95dc051<br>
Message ID: \<199609030151.SAA07328@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-09-03 05:11:22 UTC<br>
Raw Date: Tue, 3 Sep 1996 13:11:22 +0800<br>

## Raw message

```
{% raw  %}From: Bill Stewart <stewarts@ix.netcom.com>
Date: Tue, 3 Sep 1996 13:11:22 +0800
To: cypherpunks@toad.com
Subject: [BEATING A NOT QUITE DEAD] Passive Trojan [HORSE] (was:Re: HAZ-MAT virus)
Message-ID: <199609030151.SAA07328@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


>The key to the success is that the application in question has to be 
>compromised to respond to these codes, either by design or by hacking. 
>Either way the individual responsible must modify the execution 
>mechanism, not just the data itself.

A well-written program is hard to exploit, but badly written programs
can often be exploited in ways that allow execution of untrusted code.
For instance, the fingerd bug exploited so spectacularly by Robert Morris
handed a program more input that it was ready to accept, and the program
stupidly kept writing the input into the array, past the end, and out
into the stack, where it could be later interpreted as executable code.

If a popular GIF or JPEG interpreter was written that badly, you could 
possibly devise a GIF that lies about how big it is and encourages
the program to scribble on its stack.  Now, there probably aren't any
like that, and it'd probably have to be Netscape or MSIE or Lview
to be widespread enough to make an attack like that worthwhile.
(I'd bet on MSIE, of the three of them :-)  Does Microsoft have some sort
of Really Cool Extension to JPEG, allowing Macros for Self-Modifying JPEGs,
trying to out-do Netscape's animated GIFs?)

>Let's see -current examples of computing items with this kind of a 
>"feature"... magic cookies, macros, OLE, DDE, MS Objects, JAVA, and the 
>list keeps growing.

Back when Good Times came out, everyone denied that it was possible
for there to be any risk from a text file (though, as I pointed out,
escape-sequence hacks have been used occasionally for over 15 years),
and not long after that, the MSWord Macro Viruses started appearing.
Bad Code can't always be hacked usefully, but it can always be hacked...

#			Thanks;  Bill
# Bill Stewart, +1-415-442-2215 stewarts@ix.netcom.com
# <A HREF="http://idiom.com/~wcs"> 	
# You can get PGP software outside the US at ftp.ox.ac.uk/pub/crypto





{% endraw %}
```

## Thread

+ Return to [September 1996](/archive/1996/09)

+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/authors/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "["Paul S. Penrod" <furballs<span>@</span>netcom.com>](/authors/paul_s_penrod_furballs_at_netcom_com_)"

+ 1996-09-03 (Tue, 3 Sep 1996 13:11:22 +0800) - [BEATING A NOT QUITE DEAD] Passive Trojan [HORSE] (was:Re: HAZ-MAT virus) - _Bill Stewart \<stewarts@ix.netcom.com\>_
  + 1996-09-03 (Tue, 3 Sep 1996 18:59:29 +0800) - [Still more mileage from the old grey mare... was: Trojan Horse](/archive/1996/09/cd96af4edb1d170a6525cab527fa3e5cb175ffb9e081d063735d392a0e34ce38) - _"Paul S. Penrod" \<furballs@netcom.com\>_

