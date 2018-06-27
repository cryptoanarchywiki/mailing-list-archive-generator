---
layout: default
---

# 1996-09-29 - Re: Making Remailers Widespread [REMAILERS]

## Header Data

From: Bill Stewart \<stewarts<span>@</span>ix.netcom.com\><br>
To: remailer-operators@c2.org<br>
Message Hash: d6503e9cadf604e9b95df69cd463d3e3bbcc02cf3e432cdde6b0fddf8aded445<br>
Message ID: \<199609290623.XAA25604@dfw-ix3.ix.netcom.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-09-29 08:43:18 UTC<br>
Raw Date: Sun, 29 Sep 1996 16:43:18 +0800<br>

## Raw message

```
{% raw  %}From: Bill Stewart <stewarts@ix.netcom.com>
Date: Sun, 29 Sep 1996 16:43:18 +0800
To: remailer-operators@c2.org
Subject: Re: Making Remailers Widespread [REMAILERS]
Message-ID: <199609290623.XAA25604@dfw-ix3.ix.netcom.com>
MIME-Version: 1.0
Content-Type: text/plain


There have been several good replies - thanks!

>> Doing two-way remailers would be better, but that's still a hard problem,
>> and I don't want to widely deploy shoddy two-way-remailers.

>Unfortunately, one-way remailers have much fewer uses than two-way remailers,
>any many of these uses are abusive.

I agree, it's a problem; the return address seems to reduce abuse.
But one-way remailers can be used to simulate many of the uses of two-way,
especially with message-pool return methods (e.g. alt.anonymous.messages.)
Doing two-way remailers well is hard - most of the methods around are ok
for passive attacks, but may not resist subpoenas, rubber-hose, or crackers.
It's especially hard if you want the remailer to be a no-brainer to install
and operate, rather than one that requires expert support.

Snow's one-shot reply block method is interesting, whether you do a public-key
or secret-key approach (if you do public key, you obviously use the public
half for the part that stays at the remailer.)  It has the real advantage that
compromising the remailer doesn't give you the reply information for past or
current messages, so you can only compromise one message at a time,
which is a big win over the one-key-per-remailer reply blocks.
I think I like it.

On the other hand, there are a host of potential problems:
- Chaining is probably more difficult, at least return-chaining.
- Individual True Believer remailer operators would usually resist
cooperating with authorities to decrypt the reply block, but ad-hoc
remailer operators who are just running a remailer because they haven't
turned off the default feature that came with their Web Server
will probably reveal the key, especially for Politically Incorrect material
(definition depends on their individual politics, of course.)
- A web form interface, filled out from a web anonymizer, doesn't
give you a useful return address, so spammers can still abuse it.
- You have to decide how much persistence to use for the reply block.
One-shots are more secure, but aren't helpful for replies to web postings
or other multiple-recipient communication, but timeouts have their own problems.

>> - A centralized block list (e.g. http://www.remailer.net/block.txt)
>> which all of the form-based remailers could load and reference would
>> allow non-picky operators not to have to handle it themselves
>A single centralized point of failure is bad. Maybe 4 or 5 redundant ones.
>A blocking request sent to one will be replicated in the other automatically.

Good point.  A bit tough to implement in a no-brainer out-of-the-box remailer;
you gain a bit by having the block list point to an address that's really
a round-robin DNS spinner of some sort, but that still leaves you with
centralization.

>> [centralized blocking list; handshake with cookies ]
>>         - this is a bit messier for mailing lists, but we can ignore...
>
>We can't quite ignore... In the scheme you've just described, someone can
>enter a blocking request via a Web page and give a submission request for
>some mailing list, and the cookie will be e-mailed to the mailing list.

Yeah.  This makes it easy to block anonymous remailer input to (say)
the cypherpunks mailing list, since _any_ mailing list user can block.
Putting a never-block list at the blocking server is a possibility,
and would require some announced policy for implementing it.

>>         - special-case for "postmaster", who may want to block
>>                 all of foo.domain instead of just postmaster@foo.domain
>>         - special-special-case for postmasters of big sites, e.g. aol, netcom
>>                 who we may want to ignore?

>I don't think it's a good idea to suport blocking receivers in an entire
>domain, like *@aol.com. Just say it's not supported.

Blocking an entire domain like *@aol.com is mostly bad.
Blocking an entire domain like *@myconsultingfirm.com is fine.
Deciding the boundary between the two is, um, amusing :-)
I'd probably set it such that ISPs don't get blocked, but non-ISPs do,
though that might change if the administrator of aol.com asks 
five million users to submit individual blocking request.
I suppose this means there's a volume question here :-)
Having a don't-block list that individuals can subscribe to would help.

>> - A sender-blocking list is harder, and may still take human attention
>I don't think it's a good idea to support sender blocking at all.

There are some spammers you'd like to stop quickly when a Spam Event 
is happening.  There are broken email gateways that may need blocking.
There are known abusers you might want stopped.  And there are folks like
president@whitehouse.gov who can be presumed to be forgeries :-)
A sender-blocking list administered by the Remailer Cabal* would be
a reasonable default for no-brainer remailers, and obviously it
should be possible for remailer-admins to override or ignore if they want.


>Would the receiver blocking list be available to everyone to view? That
>sounds like a violation of privacy. Someone suggested on this list that
>(assuming that the entires are addresses that match exactly, not regular
>expressions), one can store hashes of addresses. 

That's worth doing, or at least thinking about seriously.
The most interesting regular expressions are *@domain (which you can
handle by keeping separate block lists for domains and full addresses
(or a merged list that the using remailer checks both)) and
*@*.domain and user@*.domain - e.g. alice@mailserver17.big-isp.com,
which would successfully deliver mail to alice@big-isp.com.
Perhaps the system needs to keep two hashes - hash(alice),hash(big-isp.com)
and check subsets of the domain name?  This is creeping featurism,
but it may be the right way to go to set a good precedent.

One unfortunate result of only using hashed names and not 
readable names is that it doesn't help the current remailer operators,
since their existing code doesn't work that way.  
Keeping the file of real names encrypted and only distributing it
to the Remailer Cabal seems leaky at best :-) - I'd expect to see it
remailed to some public place just on principle.

snow wrote:
> Off the top of my head, the biggest problem is that you can't send 
> email to a web site (page).
You can easily send it to a procmail program at a web site, though,
which can take care of doing the right thing with it.
Mark M.'s pointer to netcat is especially relevant for this.
> Netcat can be used pretty easily to fetch URLs 
> (e.g. echo "GET /foobar.html HTTP/1.0" | nc www.webserver.com 80). 

[*The existence of the Remailer Cabal, viewed by some as a 
shadowy subversive conspiracy, and by others as Dedicated Public Servants
has been repeatedly denied by anyone in a position to know. :-) ]

#			Thanks;  Bill
# Bill Stewart, +1-415-442-2215 stewarts@ix.netcom.com
# <A HREF="http://idiom.com/~wcs"> 	
# You can get PGP software outside the US at ftp.ox.ac.uk/pub/crypto





{% endraw %}
```

## Thread

+ Return to [September 1996](/archive/1996/09)
+ Return to [October 1996](/archive/1996/10)

+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/authors/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "[dlv<span>@</span>bwalk.dm.com (Dr.Dimitri Vulis KOTM)](/authors/dlv_at_bwalk_dm_com_dr_dimitri_vulis_kotm_)"
+ Return to "[snow <snow<span>@</span>smoke.suba.com>](/authors/snow_snow_at_smoke_suba_com_)"

+ 1996-09-29 (Sun, 29 Sep 1996 16:43:18 +0800) - Re: Making Remailers Widespread [REMAILERS] - _Bill Stewart \<stewarts@ix.netcom.com\>_
  + 1996-09-29 (Mon, 30 Sep 1996 02:18:35 +0800) - [Re: Making Remailers Widespread [REMAILERS]](/archive/1996/09/fc2e9c9f835a6730bb76166d2b61c45680f4179748a660c0f8eacefa54a799d8) - _dlv@bwalk.dm.com (Dr.Dimitri Vulis KOTM)_
  + 1996-10-01 (Tue, 1 Oct 1996 08:49:49 +0800) - [Re: Making Remailers Widespread [REMAILERS]](/archive/1996/10/5029dd22e2f2b4319b2070c5ad446ace780f8be861d8868072746e12f9137ad5) - _snow \<snow@smoke.suba.com\>_

