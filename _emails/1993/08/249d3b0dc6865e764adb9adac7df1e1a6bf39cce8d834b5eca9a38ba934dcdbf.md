---
layout: default
---

# 1993-08-27 - What, Me Worry?

## Header Data

From: karn<span>@</span>qualcomm.com (Phil Karn)<br>
To: peb@PROCASE.COM<br>
Message Hash: 249d3b0dc6865e764adb9adac7df1e1a6bf39cce8d834b5eca9a38ba934dcdbf<br>
Message ID: \<9308272011.AA06979@servo\><br>
Reply To: \<9308271811.AA06477@banff.procase.com\><br>
UTC Datetime: 1993-08-27 20:13:24 UTC<br>
Raw Date: Fri, 27 Aug 93 13:13:24 PDT<br>

## Raw message

```
{% raw  %}From: karn@qualcomm.com (Phil Karn)
Date: Fri, 27 Aug 93 13:13:24 PDT
To: peb@PROCASE.COM
Subject: What, Me Worry?
In-Reply-To: <9308271811.AA06477@banff.procase.com>
Message-ID: <9308272011.AA06979@servo>
MIME-Version: 1.0
Content-Type: text/plain


I follow the GPS universe fairly closely.  The term for the
intentional degrading of accuracy for "unauthorized" (civilian) users
is "Selective Availability" (SA).

The story gets even better. Although the DoD hasn't described how SA
works, it's now apparent that they add cryptographically generated
"phase noise" to the timebase on each satellite, probably with a
direct digital synthesizer. In other words, the satellite looks like
it has a noiser atomic clock than it really does. "Authorized" users
with the right keys can regenerate the same dither stream and subtract
it out of their observations.

During the Gulf War, the DoD quietly turned SA *off* because they
could only meet their immediate need for vast quantities of receivers
by tapping the commercial ("unauthorized") market.  Of course, this
did not go unnoted by the civilan GPS market; there were probably some
red faces in the Pentagon.  I do know there were a lot of broad grins
in the civilian world. It's almost as if they had decided to use PGP
on PC clones due to a lack of NSA-approved military crypto gear.

Unfortunately, after the war, DoD turned SA back on again. However,
the civies had a neat trick up their sleeves: "differential GPS". This
involves placing a GPS receiver in a fixed spot and having it
broadcast the difference between its known location and its current
position as determined by GPS. Because most of the errors in GPS are
strongly correlated between nearby receivers, this subtracts out
almost all the errors in the mobile user's position. Not just SA, but
ionospheric dispersion, orbital element inaccuracies, etc.  The result
is an accuracy of 1-3 meters, with or without SA.

The really fun part is this. Guess who's leading the effort to deploy
differential GPS beacons? The US Coast Guard! That's right, while one
side of the military intentionally sabotages the signal, another
military service (albeit under the Department of Transportation rather
than the DoD) works to un-sabotage it! Your tax dollars at work.

Actually, the Coast Guard says it would be doing differential GPS even
if SA were turned off.  With SA on, accuracy is typically on the order
of 100m; without it, accuracy improves only to about 25m, and this is
insufficient for many harbor approaches.

And here's yet another delightful irony in the GPS saga. The DoD
maintains a network of ground tracking stations that determine the
orbit of each GPS satellite. Every few hours they uplink these orbital
elements to the satellites so they can be broadcast to the users.
There was talk for a time of encrypting the low order bits of the
orbital elements as part of SA, but this apparently hasn't happened.
Nevertheless, GPS is so useful to the international scientific
community that they've set up their own network of tracking stations
to produce and disseminate their own GPS orbital elements. And while
the DoD-generated elements are good only to about 10-15m, the
civilians, having many more stations and better techniques, generate
sets good to less than 1m!

Phil








{% endraw %}
```

## Thread

+ Return to [August 1993](/archive/1993/08)

+ Return to "[karn<span>@</span>qualcomm.com (Phil Karn)](/authors/karn_at_qualcomm_com_phil_karn_)"
+ Return to "[peb<span>@</span>PROCASE.COM (Paul Baclace)](/authors/peb_at_procase_com_paul_baclace_)"

+ 1993-08-27 (Fri, 27 Aug 93 11:13:21 PDT) - [Re: What, Me Worry?](/archive/1993/08/8bb3dd35ec66bd2e027e9d260c349d8546d7daa698b345af31886464de16e4c0) - _peb@PROCASE.COM (Paul Baclace)_
  + 1993-08-27 (Fri, 27 Aug 93 13:13:24 PDT) - What, Me Worry? - _karn@qualcomm.com (Phil Karn)_

