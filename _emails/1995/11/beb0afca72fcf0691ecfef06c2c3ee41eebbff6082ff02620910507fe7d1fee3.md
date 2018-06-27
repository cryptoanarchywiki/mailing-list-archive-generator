---
layout: default
---

# 1995-11-02 - Sources of randomness

## Header Data

From: Carl Ellison \<cme<span>@</span>TIS.COM\><br>
To: tcmay@got.net<br>
Message Hash: beb0afca72fcf0691ecfef06c2c3ee41eebbff6082ff02620910507fe7d1fee3<br>
Message ID: \<9511022143.AA26596@tis.com\><br>
Reply To: \<199511021940.LAA00300@comsec.com\><br>
UTC Datetime: 1995-11-02 23:13:18 UTC<br>
Raw Date: Fri, 3 Nov 1995 07:13:18 +0800<br>

## Raw message

```
{% raw  %}From: Carl Ellison <cme@TIS.COM>
Date: Fri, 3 Nov 1995 07:13:18 +0800
To: tcmay@got.net
Subject: Sources of randomness
In-Reply-To: <199511021940.LAA00300@comsec.com>
Message-ID: <9511022143.AA26596@tis.com>
MIME-Version: 1.0
Content-Type: text/plain


>Date: Thu, 2 Nov 1995 00:39:29 -0800
>From: tcmay@got.net (Timothy C. May)

>Digitized video input, especially from something like a noisy channel (t.v.
>channel, for example), is quite likely to produce a lot more entropy bits
>per second than nearly any of us ever need. (One's PGP key could be seeded
>in a fraction of a millisecond, for example.)

My cable feed into my Mac, for example, has surprisingly little noise --
and it's only local noise (stuff only at my house, not available to the
eavesdropper) which counts as entropy.

>  One of the basic ideas we
>have had, as Cypherpunks, is to encourage widespread methods. Any methods
>that need special hardware tend to not get widely used.
>
>Audio, video, disk timing, and all sorts of other sources of physical
>randomness are useful to have, but most people either won't have the right
>configuration or won't configure their systems so as to use their
>configuration.

Most Macs and PCs have audio inputs.  Most of those are mono,
unfortunately.  [The numeric difference between two stereo mics is
especially hard for an eavesdropper-wannabe to predict/compute, assuming
the room isn't silent.]  However, if the eavesdropper doesn't have a mic in
your room, there's still some entropy available on the mono channel.

Meanwhile, my old Sparcstation 1 had an A-D which, when no mic was
connected, gave about 1 bit/second of entropy.  (The newer Sparc here gives
solid 0's with no mic.)

Recorded audio is useless as entropy, of course.


Almost all computers have a mouse and a normal signature, hand-written with
a mouse, has great gobs of noise.  (I'm still working on the little PC
program to measure this -- but preliminary results show a minimum of 1 bit
of noise per mouse sample -- or 200 bits per signature.  Final results may
get higher entropy rates, but I'll wait for the real results before
claiming that.)


+--------------------------------------------------------------------------+
|Carl M. Ellison      cme@tis.com    http://www.clark.net/pub/cme	   |
|Trusted Information Systems, Inc.   http://www.tis.com/                   |
|3060 Washington Road          PGP 2.6.2:  61E2DE7FCB9D7984E9C8048BA63221A2|
|Glenwood MD  21738         Tel:(301)854-6889      FAX:(301)854-5363       |
+--------------------------------------------------------------------------+






{% endraw %}
```

## Thread

+ Return to [November 1995](/archive/1995/11)

+ Return to "[Carl Ellison <cme<span>@</span>TIS.COM>](/authors/carl_ellison_cme_at_tis_com_)"
+ Return to "["Perry E. Metzger" <perry<span>@</span>piermont.com>](/authors/perry_e_metzger_perry_at_piermont_com_)"

+ _Unknown thread root_
  + 1995-11-02 (Fri, 3 Nov 1995 07:13:18 +0800) - Sources of randomness - _Carl Ellison \<cme@TIS.COM\>_
    + 1995-11-03 (Fri, 3 Nov 1995 10:00:07 +0800) - [Re: Sources of randomness](/archive/1995/11/d3345dcaf84808e388e1d17423d0b221e0b251be739944294854410254be7e3d) - _"Perry E. Metzger" \<perry@piermont.com\>_

