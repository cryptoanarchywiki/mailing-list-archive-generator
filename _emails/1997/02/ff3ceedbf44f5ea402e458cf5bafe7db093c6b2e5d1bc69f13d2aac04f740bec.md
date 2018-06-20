---
layout: default
---

# 1997-02-18 - Re: Anyone have the complete info on CP list alternatives?

## Header Data

From: "E. Allen Smith" \<EALLENSMITH@ocelot.Rutgers.EDU\><br>
To: cypherpunks@toad.com<br>
Message Hash: ff3ceedbf44f5ea402e458cf5bafe7db093c6b2e5d1bc69f13d2aac04f740bec<br>
Message ID: \<01IFJFI7LF848Y4YVV@mbcl.rutgers.edu\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-02-18 03:57:08 UTC<br>
Raw Date: Mon, 17 Feb 1997 19:57:08 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: "E. Allen Smith" <EALLENSMITH@ocelot.Rutgers.EDU>
Date: Mon, 17 Feb 1997 19:57:08 -0800 (PST)
To: cypherpunks@toad.com
Subject: Re: Anyone have the complete info on CP list alternatives?
Message-ID: <01IFJFI7LF848Y4YVV@mbcl.rutgers.edu>
MIME-Version: 1.0
Content-Type: text/plain


From: ichudov@algebra.com (Igor Chudov @ home)

>Bryan Reece wrote:
>> 
>> It receives some Big Usenet groups, but only for local users.
>> alt.cypherpunks is open, but there will be long delays, on the
>> order of a day, for articles there (unless someone better connected to
>> Usenet wants to feed me alt.cypherpunks.*---any volunteers?).

	Well, Lance Cottrell would appear to be a good person to ask
on this matter, but...

>I just set up a recipe for using mail2news gateways like this:

>:0 c
>| formail -I "Newsgroups: alt.cypherpunks,misc.misc" | 		\
>	sendmail mail2news@anon.lcs.mit.edu mail2news@utopia.hacktic.nl

>Any objections?

given that mail2news@anon.lcs.mit.edu gets one of its USENET feeds via
cyberpass.net, it would appear to be unnecessary if this recipe is in
use. However, I do have one problem with this recipe: lack of
loop prevention if a news2mail gateway is going in the other direction.
I don't know, but the mail2news gateway folks may not be too happy with
this idea either, given massively increased load; this is particularly
true since IIRC misc.misc is _not_ the proper place to crosspost stuff
from & to; it's only for stuff that _really_ doesn't fall under any
other category. (I've crossposted this message to the remailer-operators
mailing list to make sure it gets to the operators of the gateways in
question.)

In regards to your later query about whether people want their postings
going to Usenet, might I suggest that this be individual to the given
distributed mailing list? In other words, since the recipe is logically
going to have to not forward to a gateway messages from other mailing
lists (since it's not a good idea to have multiple copies of the same
message arriving at the gateway if it can be helped; better to filter
it out beforehand), some of the mailing lists can forward and the
others cannot. (One could even determine this behavior on application
of the proper X-header, although I never trust various mailing systems
to forward such intact.) The same could also be done with gatewaying
_from_ Usenet - if the news2mail gateway feeds to whatever individual
lists sign up to it and they _don't_ forward such messages to others,
people can decide whether or not to receive Usenet postings on
alt.cypherpunks.* by which list they subscribe to.
	-Allen

P.S. A thank you to Reece for setting up a gateway; I had looked
at the program and did _not_ much like the idea of having to
maintain it on my limited knowledge of C/C++ and mailing
software.




{% endraw %}
```

## Thread

+ Return to [February 1997](/archive/1997/02)

+ 1997-02-18 (Mon, 17 Feb 1997 19:57:08 -0800 (PST)) - Re: Anyone have the complete info on CP list alternatives? - _"E. Allen Smith" \<EALLENSMITH@ocelot.Rutgers.EDU\>_
  + 1997-02-18 (Mon, 17 Feb 1997 20:24:04 -0800 (PST)) - [Re: Anyone have the complete info on CP list alternatives?](/archive/1997/02/cbb3d833d1692e81f5500ebe7a9dfe1b7014044f09e38cb413f3883fe9448cc2) - _Bryan Reece \<reece@taz.nceye.net\>_

