---
layout: default
---

# 1996-02-02 - Re: Espionage-enabled Greed

## Header Data

From: "Erik E. Fair"  (Time Keeper) \<fair<span>@</span>clock.org\><br>
To: cypherpunks@toad.com<br>
Message Hash: c5a41f00ef355cebcc5a0abedbecd57ce8d3d0dd01b39e01519cf9ab3d44cf07<br>
Message ID: \<v02110102ad3807f0e5c1@[198.68.110.3]\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-02-02 20:35:21 UTC<br>
Raw Date: Sat, 3 Feb 1996 04:35:21 +0800<br>

## Raw message

```
{% raw  %}From: "Erik E. Fair"  (Time Keeper) <fair@clock.org>
Date: Sat, 3 Feb 1996 04:35:21 +0800
To: cypherpunks@toad.com
Subject: Re: Espionage-enabled Greed
Message-ID: <v02110102ad3807f0e5c1@[198.68.110.3]>
MIME-Version: 1.0
Content-Type: text/plain


This scenario has one problem: the providers have determined that large
public peering points like the CIX, NAPs, MAEs, and FIXs do not scale well,
and that for the continued health and growth of the Internet, there are
going to have to be more small, private interconnects between providers.

Put another way: if the equipment you're working with has certain limits
(let's say 100Mb/s FDDI or 45Mb/s T3/DS3 interfaces), it's better to have
more interconnects with fewer peers at each interconnect point when your
traffic potentially or actually will exceed those interface limits in
aggregate. This is being driven by the incredible growth of the Internet,
and by the fact that the customers can (and do) buy the same size pipes
into the providers that the providers themselves use for their backbones -
i.e. any such customer can potentially fill your backbone around the
section of your backbone where he connects to you. Ooops.

If you want to have fewer, large interconnects, which, incidentally, you
can monitor all the traffic passing through, you've gotta have monstrous
point-to-point bit pipes and/or LANs, and the Router/Switch From Hell to
make the traffic move. There are people trying to build such things - it's
called Asynchronous Transfer Mode (ATM), but it doesn't really work in
practice yet at high enough speeds - best you can get at the moment is OC3
(155Mb/s), which is only a trifle faster than FDDI, and the stuff is more
expensive than conventional LAN/WAN technology, so it's only being used in
small areas to prove the technology (with the hope that it really does
scale as promised, and gets cheaper). There are working examples of a fast
LAN switch in use at the public peering points: the DEC GIGAswitch (3.2Gb/s
aggregate - 16 100Mb/s FDDI ports).

Of course, you also have to build a pretty fast computer to suck down all
this traffic and analyze it, too. And we all have the ultimate laugh on
would-be eavesdroppers: IP security (read: end-to-end encryption of the
data payload of IP packets on a per peer basis), drafts for which are in
implementation phase as of the Stockholm IETF meeting (July 1995). This
leaves 'em with just traffic analysis to use on us.

Erik Fair






{% endraw %}
```

## Thread

+ Return to [February 1996](/archive/1996/02)

+ Return to "["Erik E. Fair"  (Time Keeper) <fair<span>@</span>clock.org>](/authors/erik_e_fair_time_keeper_fair_at_clock_org_)"

+ 1996-02-02 (Sat, 3 Feb 1996 04:35:21 +0800) - Re: Espionage-enabled Greed - _"Erik E. Fair"  (Time Keeper) \<fair@clock.org\>_

