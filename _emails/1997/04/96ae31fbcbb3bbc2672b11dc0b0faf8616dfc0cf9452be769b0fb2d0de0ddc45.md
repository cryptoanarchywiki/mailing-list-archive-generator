---
layout: default
---

# 1997-04-01 - Re: [NTSEC] Re: Internet Explorer Bug #4 (fwd)

## Header Data

From: Bill Stewart \<stewarts<span>@</span>ix.netcom.com\><br>
To: chris@breakwater.net<br>
Message Hash: 96ae31fbcbb3bbc2672b11dc0b0faf8616dfc0cf9452be769b0fb2d0de0ddc45<br>
Message ID: \<3.0.1.32.19970331201125.0064f4f8@popd.ix.netcom.com\><br>
Reply To: \<Pine.SUN.3.91.970331111923.18046H-100000@beast.brainlink.com\><br>
UTC Datetime: 1997-04-01 04:15:11 UTC<br>
Raw Date: Mon, 31 Mar 1997 20:15:11 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: Bill Stewart <stewarts@ix.netcom.com>
Date: Mon, 31 Mar 1997 20:15:11 -0800 (PST)
To: chris@breakwater.net
Subject: Re: [NTSEC] Re: Internet Explorer Bug #4 (fwd)
In-Reply-To: <Pine.SUN.3.91.970331111923.18046H-100000@beast.brainlink.com>
Message-ID: <3.0.1.32.19970331201125.0064f4f8@popd.ix.netcom.com>
MIME-Version: 1.0
Content-Type: text/plain


At 11:19 AM 3/31/97 -0500, Ray Arachelian forwarded:
>---------- Forwarded message ----------
>Date: Sat, 29 Mar 1997 14:37:43 -0800
>From: Chris Plunkett <chris.plunkett@opensys.com>
>To: pmarc@cmg.FCNBD.COM
>Cc: Romulo Moacyr Cholewa <rmcholewa@poboxes.com>,
>    Windows NT BugTraq Mailing List <NTBUGTRAQ@rc.on.ca>,
>    "ntsecurity@iss.net" <ntsecurity@iss.net>, hughtay@microsoft.com
>Subject: Re: [NTSEC] Re: Internet Explorer Bug #4

	[Amusing story deleted "486 with 'YMP' sticker on it]
>I heard a story one time.  It evolved around a college student in
>France doing some cyptography work in school,  working nights 
>as a backup operator at some large computer center.  He didn't need
>a cray.   A little knowledge and some creative programming,  and 
>a center full of computers (problably around the size of a Sparc 10).
>The story ended explaning how one of the encryption schemes that 
>would tale a Cray week to break,  was broken in one night,  by a 
>bunch of computers running backups.

This is almost certainly the RC4/40 crack in August 1995 by
Damien Doligez in response to Hal Finney's challenge.
It had actually been broken a few hours earlier by an
English (Anglo-American?) team using a coordinated
Internet attack, but Damien noticed his success before
they noticed theirs.  Much noise was made in the press by
various people about "Using $10,000 worth of supercomputer time",
but in fact the antique KSR-1 contributed far less crunching than
the bunch of DEC Alpha workstations, and the amount of money
per crack (if you'd been renting computer time) would have been
far less.  Subsequent cracks were run by the Internet team,
which ran even faster, once they were organized.
Various Cypherpunks were quoted in the press talking about
how the US export laws were bogus, and how the maximum-strength
crypto allowed by US law could be broken by a grad student over
a weekend.

Since then, there have been other cracks - the RC5/40 crack by
Ian Goldberg took 3.5 hours on a Network of Workstations at Berkeley,
winning the RSA challenge a few minutes before Germano Caronni's
distributed Internet team, which subsequently broke the RC5/48 challenge.
It's been popular in the press to refer to these talented researchers as
"a grad student" when trying to make the point that "anybody could
break this wimpy stuff" or as "a university research team with a 
room full of expensive supercomputers" when trying to pretend
the export limits are reasonable for the real world.

The news article below is from "NB", presumably "NewsBytes",
and was posted without permission to the cypherpunks list
by an anonymous remailer user.
======================================================
Date: Sat, 19 Aug 1995 00:01:18 +0200
Subject: WhiSSLing in the Dark 
To: cypherpunks@toad.com
From: nobody@REPLAY.COM (Anonymous)

Netscape Encrypted Data Cracked

Tokyo, Japan, Aug. 18 (NB) -- Two computer users have
managed to break Netscape's Secure Sockets Layer (SSL)
encryption code in response to a challenge posted to the
Internet. But far from scaring people away from using the
system for online purchases, the results could reassure
people of the safety.

In mid July Hal Finney, a US computer user, posted data
in an Internet message that he recorded when he sent an
order, containing a fake name and credit card details, to
Netscape's own computer. Setting a task for the hacking
community, he wrote, "The challenge is to break the
encryption and recover the name and address info I
entered in the form and sent securely to Netscape."

Early this week, news came from Damien Doligez, a French
computer user, that he had cracked the code and revealed
the contents of the message. Several hours later a
message from an American team also claimed the same feat,
actually cracking it two hours earlier than Doligez.

While the results look damaging on the surface, Netscape,
and Doligez, pointed out the amount of computer
processing power needed to hack just one message and the
difficulty in repeating the process.

Roseanne Siino of Netscape told Newsbytes, "The real
issue is whether this compromises security on the net. He
used 120 computers for 8 days just to crack one message."
Siino points out that to break into another message would
require another eight days at the same 120 workstations
and 2 parallel computers.

In home computer terms, Doligez guesses a network of
about 80 Intel Pentium-based machines would be equivalent
to the system he had access to via his workplace, INRIA
in Paris, and computers an Ecole Polytechnique and ENS.

Netscape estimates the total cost of this computing time
at around $10,000, meaning there are many more economical
ways of getting credit cards numbers than hacking into
Netscape SSL messages.

Doligez agrees, writing on his home page: "The technical
implications are almost zero. Everybody who understands
the technical details knew perfectly well that this was
do-able and even easy. You have to understand what
happened exactly. I did not break SSL itself. I did only
break one SSL session that used the weakest algorithm
available in SSL. If I want to break another session, it
will cost another 8 days of all my machines."
The vulnerability of the encryption system is shown by
its international use. The coding system available via
Netscape software from the Internet makes use of a 40-bit
encryption key. A stronger version, using a 128-bit key,
is available to US citizens but restricted from export
outside the United States by government regulations.

Netscape's Siino explained the US government allows
export of the lower security version "because they can
break it."

There are some hopes that this demonstration will help
persuade the US government to lift export restrictions on
some harder-to-crack versions of the code.

Netscape is currently developing a new Secure Courier
code which just encrypts the financial data in the
messages using 56-bit keys. Siino explained, "You can
export over 40-bit keys for a specific application." The
new system should be available early next year.

Many companies working on secure transaction systems hope
the much more secure 128-bit code version of the system
will be available for export eventually. This is said to
be almost unbreakable, requiring a trillion times more
processing power to crack than the 40-bit version.

Internet users can view a copy of the original challenge,
access Doligez's home page with details of his result,
get copies of the program used to crack the code and read
Netscape's response to the news through a special section
at Netscape,

http://home.netscape.com/newsref/std/key_challenge.html

Press contacts : Roseanne Siino, Netscape,
+1-415-528-2619 , Internet email roseanne@netscape.com;
Damien Doligez, Internet email damien.doligez@inria.fr ;
Hal Finney, Internet email hfinney@shell.portal.com)

=========================================================================




#			Thanks;  Bill
# Bill Stewart, +1-415-442-2215 stewarts@ix.netcom.com
# You can get PGP outside the US at ftp.ox.ac.uk/pub/crypto/pgp
#     (If this is a mailing list, please Cc: me on replies.  Thanks.)





{% endraw %}
```

## Thread

+ Return to [March 1997](/archive/1997/03)
+ Return to [April 1997](/archive/1997/04)

+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/author/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "[Ray Arachelian <sunder<span>@</span>brainlink.com>](/author/ray_arachelian_sunder_at_brainlink_com_)"

+ 1997-03-31 (Mon, 31 Mar 1997 08:16:44 -0800 (PST)) - [Re: [NTSEC] Re: Internet Explorer Bug #4 (fwd)](/archive/1997/03/e531cf8cda06709cd3598f10a670a26855f3d37e929168141fea99a7e8b0bfda) - _Ray Arachelian \<sunder@brainlink.com\>_
  + 1997-04-01 (Mon, 31 Mar 1997 20:15:11 -0800 (PST)) - Re: [NTSEC] Re: Internet Explorer Bug #4 (fwd) - _Bill Stewart \<stewarts@ix.netcom.com\>_

