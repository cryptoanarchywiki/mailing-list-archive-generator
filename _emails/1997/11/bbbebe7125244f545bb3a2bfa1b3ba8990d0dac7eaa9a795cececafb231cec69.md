---
layout: default
---

# 1997-11-03 - One Time Pads (Real Ones!)

## Header Data

From: Mix \<mixmaster<span>@</span>remail.obscura.com\><br>
To: cypherpunks@cyberpass.net<br>
Message Hash: bbbebe7125244f545bb3a2bfa1b3ba8990d0dac7eaa9a795cececafb231cec69<br>
Message ID: \<199711031002.CAA26848@sirius.infonex.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-11-03 10:26:28 UTC<br>
Raw Date: Mon, 3 Nov 1997 18:26:28 +0800<br>

## Raw message

```
{% raw  %}From: Mix <mixmaster@remail.obscura.com>
Date: Mon, 3 Nov 1997 18:26:28 +0800
To: cypherpunks@cyberpass.net
Subject: One Time Pads (Real Ones!)
Message-ID: <199711031002.CAA26848@sirius.infonex.com>
MIME-Version: 1.0
Content-Type: text/plain



-----BEGIN PGP SIGNED MESSAGE-----

One time pads are under rated, in my view.  Not only are they secure
forever, but the executive branch of the U.S. government says they are
exportable.

I've been thinking about how practical they are.

One diskette holds about 150 messages.  The people we trust tend to be
people we communicate with a lot.  An exchange of one box of diskettes
should last a long time in most cases.

The first 128 bits of the pad can be used as a key to identify it.
This the recipient can figure out how to decode it by hunting through
his or her key collection for the one that matches.

When keys are exchanged, additional information can be exchanged and
associated with each key.  Length, for example.  This means no length
fields are needed because it can be recovered from the key itself.
There are probably more examples.

One time pads are self authenticating.

For increased security, the use of a double one time pad is a good
idea.  Both correspondents generate key sets.  The message is
encrypted using one key from each key set.  Again, no identifying
information is needed, because the recipient can look for pairs of
keys that work.

If these key sets are exchanged through separate secure channels, they
will be especially hard to compromise.

Also, each user can be confident that the message is secure with
regard to key material if they have generated the keys themselves.

Keys should be destroyed immediately after use.  This means that the
only time the rubber hose attack is effective is during message
transit.

Key destruction is a hard problem, though, because it is difficult to
be confident that the key has been completely erased from a disk.  Use
of diskettes improves the situation.  Other media might be better,
such as static memory.

There is no good reason not to wrap one time pads in other encryption
protocols.  It is hard, maybe impossible for some algorithms, to crack
a message when the contents have the appearance of noise.  This means
that it is hard to tell who is using one time pads and when they are
doing it.  Naturally, the user will send many messages which consist
of noise, indistinguishable from a one time pad.  This gives the user
plausible deniability, especially if the practice is common.

If the wrapper encryption protocol has not been compromised at the
time of use, it has the pleasing result that it buys time.  Should the
message be recorded and filed on tape at Ft. Meade, and the encryption
protocol broken ten years later, the user will have a very difficult
time producing the key material.

Key generation is an inadequately solved problem right now.  There are
chips which generate streams of random bits, but it is impossible to
tell if they have been compromised.  A home brew hardware based random
number generator with a serial interface is probably the best way to
go.  The output of this device could be XORed with other source of
randomness to increase confidence.

One time pads seem practical to me.

Comments?

Monty Cantsin
Editor in Chief
Smile Magazine
http://www.neoism.org/squares/smile_index.html
http://www.neoism.org/squares/cantsin_10.htm

-----BEGIN PGP SIGNATURE-----
Version: 2.6.2

iQEVAwUBNF1/WZaWtjSmRH/5AQER3Af+M+T31s+VOdrCE61a0kbp0fe3Eyosoub2
YkAWZs48knTFgtAS0sv5IRrKparKaKdgAQISscBSuW5YXGi9WJCA2/3+2/+iwvrK
1tIoEDF+fYaq6/a2yiyI4PVZ8qPMpyLayZ3K89P8N8zzuQSMS6pB7yOf4waOufcF
6nAmcVG8/O4BddID15XiKbdc7QSpHKK2R3LlwrS4ZQBHyhYvC5Quo41SHNiWIGjO
N6zMkBKuDXEpjmnX9O1LRelT7hEMX0ss6b4ZTmFw39NXwDwgFahP+C2/Zw+Kt0Je
+/PNDJXWWQDWovVrCW2yKmpKeTPgxTJ1R4aEpt2CBwdQlMqVwpVrAg==
=O5oZ
-----END PGP SIGNATURE-----






{% endraw %}
```

## Thread

+ Return to [November 1997](/archive/1997/11)

+ Return to "[Mix <mixmaster<span>@</span>remail.obscura.com>](/authors/mix_mixmaster_at_remail_obscura_com_)"
+ Return to "["Peter D. Junger" <junger<span>@</span>upaya.multiverse.com>](/authors/peter_d_junger_junger_at_upaya_multiverse_com_)"
+ Return to "[Tim May <tcmay<span>@</span>got.net>](/authors/tim_may_tcmay_at_got_net_)"

+ 1997-11-03 (Mon, 3 Nov 1997 18:26:28 +0800) - One Time Pads (Real Ones!) - _Mix \<mixmaster@remail.obscura.com\>_
  + 1997-11-03 (Tue, 4 Nov 1997 00:51:54 +0800) - [Re: One Time Pads (Real Ones!)](/archive/1997/11/27c6a9f083175d30a86287c8d2dafa18e615d23f0f2945271141561ef440a1f2) - _"Peter D. Junger" \<junger@upaya.multiverse.com\>_
  + 1997-11-03 (Tue, 4 Nov 1997 06:12:36 +0800) - [Export a random number, go to jail](/archive/1997/11/ee670572d13c2c7aa7a11ae91f032d04be10524a2fc37432148ea531895fecc3) - _Tim May \<tcmay@got.net\>_

