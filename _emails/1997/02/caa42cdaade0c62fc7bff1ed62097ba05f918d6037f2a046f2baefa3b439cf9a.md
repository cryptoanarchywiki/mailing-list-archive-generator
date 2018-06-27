---
layout: default
---

# 1997-02-18 - Re: Anyone have the complete info on CP list alternatives?

## Header Data

From: Bryan Reece \<reece<span>@</span>taz.nceye.net\><br>
To: EALLENSMITH@ocelot.Rutgers.EDU<br>
Message Hash: caa42cdaade0c62fc7bff1ed62097ba05f918d6037f2a046f2baefa3b439cf9a<br>
Message ID: \<199702180512.VAA23671@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-02-18 05:12:01 UTC<br>
Raw Date: Mon, 17 Feb 1997 21:12:01 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: Bryan Reece <reece@taz.nceye.net>
Date: Mon, 17 Feb 1997 21:12:01 -0800 (PST)
To: EALLENSMITH@ocelot.Rutgers.EDU
Subject: Re: Anyone have the complete info on CP list alternatives?
Message-ID: <199702180512.VAA23671@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


   Date: Mon, 17 Feb 1997 22:55 EDT
   From: "E. Allen Smith" <EALLENSMITH@ocelot.Rutgers.EDU>



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

All the mailing-list hosts are supposed to check for duplicates before
forwarding anything, so this shouldn't do anything worse than have a
few extra copies of each post get discarded, loading the network and
the hosts a bit more.  But posting the list to a widely-distributed
newsgroup seems wrong for noise (both to the list itself and to
posters) and delay reasons.

    (I've crossposted this message to the remailer-operators
   mailing list to make sure it gets to the operators of the gateways in
   question.)



   In regards to your later query about whether people want their postings
   going to Usenet, might I suggest that this be individual to the given
   distributed mailing list? In other words, since the recipe is logically
   going to have to not forward to a gateway messages from other mailing
   lists (since it's not a good idea to have multiple copies of the same
   message arriving at the gateway if it can be helped; better to filter
   it out beforehand),

It doesn't seem an especially bad idea, since it 

   some of the mailing lists can forward and the
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

The code currently running is a perl script that turns typical email
messages into something INN is happy with.  It is probably possible to
get your message rejected by INN if you put obsolete or otherwise
unusual and illegal headers in.  This may be a bug.






{% endraw %}
```

## Thread

+ Return to [February 1997](/archive/1997/02)

+ Return to "[Bryan Reece <reece<span>@</span>taz.nceye.net>](/authors/bryan_reece_reece_at_taz_nceye_net_)"

+ 1997-02-18 (Mon, 17 Feb 1997 21:12:01 -0800 (PST)) - Re: Anyone have the complete info on CP list alternatives? - _Bryan Reece \<reece@taz.nceye.net\>_

