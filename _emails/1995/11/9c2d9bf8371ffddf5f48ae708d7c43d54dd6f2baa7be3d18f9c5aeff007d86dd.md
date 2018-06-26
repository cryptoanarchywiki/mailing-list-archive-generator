---
layout: default
---

# 1995-11-04 - Re: Sources of randomness

## Header Data

From: tcmay<span>@</span>got.net (Timothy C. May)<br>
To: cypherpunks@toad.com<br>
Message Hash: 9c2d9bf8371ffddf5f48ae708d7c43d54dd6f2baa7be3d18f9c5aeff007d86dd<br>
Message ID: \<acc0dca515021004eb09@[205.199.118.202]\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-11-04 17:41:51 UTC<br>
Raw Date: Sun, 5 Nov 1995 01:41:51 +0800<br>

## Raw message

```
{% raw  %}From: tcmay@got.net (Timothy C. May)
Date: Sun, 5 Nov 1995 01:41:51 +0800
To: cypherpunks@toad.com
Subject: Re: Sources of randomness
Message-ID: <acc0dca515021004eb09@[205.199.118.202]>
MIME-Version: 1.0
Content-Type: text/plain


At 8:04 AM 11/4/95, Peter Monta wrote:

>Perhaps there ought to be a couple of standard random-bit-source
>implementations, say at the CMOS-standard-cell and board-subsystem
>levels, that are widely vetted and trusted (and used!).  But it's
>mostly a solved problem, seems to me.

This is something John Gilmore called for when he wrote:

At 9:50 PM 9/20/95, John Gilmore wrote:
>Software-generated random numbers are likely to be of poor quality.
>There just isn't that much true randomness visible to computers.
>Several ways to build good hardware random number generators are
>known.  But before hardware random number generators can be
>incorporated into common desktop computers, someone will have to put
>them into a small fraction of a chip.
>
>Currently, random number generators are chips or larger circuits.
>Nobody will pay to put these on a motherboard.  But if a random number
>generating circuit occupied 1/1000th of a CPU chip or "multi-function
>I/O" chip, cost would not be a reason to leave it out.
>
>You probably can't build a hardware random number generator out of
>existing "gate array" gates or "standard cell" cells, because all the
>existing gates and cells are designed to behave completely
>predictably!  It will take designing a new circuit structure.
>
>Do we know any solid state physics / circuit design experts who think
>this might be a fun thing to do?  I bet you could get a paper out of
>it.  And probably improve the world a few years later, when companies
>used your paper to close another hole in their computer security.
>
>        John

There were several other posts in this thread, so interested folks might
want to check the archives for this time period.

Continuing on with Peter Monta's post:

>A radioactive source might be okay at the board level (though probably
>costlier than its electronic counterpart), but it'd be a pain to
>integrate, and it might disturb the rest of the chip.  (I'd like to
>have a get_random_bit instruction as part of a microprocessor, for
>example.)  Also if you want a high rate of random bits, you need many
>decay events, whereas for electronic sources the corresponding
>bandwidth is free---Johnson and shot noise are flat to 1 THz or so.

I agree, for several reasons. First, I agree that electronic noise sources
are easy to build, easy to get licenses for use (basically, no licenses,
unless the ITAR boys decide random number generators are munitions--maybe
the "This t-shirt is a munition" could have "export-controlled dice"?

Second, the ease of integration as a standard library module.

However, getting the chip companies to do this will not be easy. They
generally don't see the need (hey, even _we_ don't, given the diverse
opinions on what is needed).

This is why many of us favor an external dongle that plugs in somewhere.
Then it could be sold cheaply and not have to get "buy-ins" from industry
and committees.

One idea is something that superficially looks like a modem, as everyone
has modem software and ports (though I suppose many people use internal
modems and so can't easily access it.) One would attach the "RNG-modem," a
little dongle, and grab noise into a buffer for processing (hashing,
filtering, etc.), or as ASCII garbage.

(Before anyone jokingly asks about "1-800-RANDOMS," I've thought of it. Not
practical, for obvious reasons.)

A purer approach would be just a noise source dumped into dev/random, or
whatever one wishes to call it.

--Tim May

Views here are not the views of my Internet Service Provider or Government.
---------:---------:---------:---------:---------:---------:---------:----
Timothy C. May              | Crypto Anarchy: encryption, digital money,
tcmay@got.net  408-728-0152 | anonymous networks, digital pseudonyms, zero
Corralitos, CA              | knowledge, reputations, information markets,
Higher Power: 2^756839      | black markets, collapse of governments.
"National borders are just speed bumps on the information superhighway."






{% endraw %}
```

## Thread

+ Return to [November 1995](/archive/1995/11)

+ Return to "[tcmay<span>@</span>got.net (Timothy C. May)](/author/tcmay_at_got_net_timothy_c_may_)"

+ 1995-11-04 (Sun, 5 Nov 1995 01:41:51 +0800) - Re: Sources of randomness - _tcmay@got.net (Timothy C. May)_

