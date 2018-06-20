---
layout: default
---

# 1997-02-10 - What's next?

## Header Data

From: Thomas Koenig \<ig25@mvmap66.ciw.uni-karlsruhe.de\><br>
To: challenge@list.ee.ethz.ch (challenge)<br>
Message Hash: 70d02b258fe2bab03ecafca5f6d356a89bea3ee6f167edda4c2ec35d6ee5efa2<br>
Message ID: \<199702101024.LAA08950@mvmap66.ciw.uni-karlsruhe.de\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-02-10 11:26:43 UTC<br>
Raw Date: Mon, 10 Feb 1997 03:26:43 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: Thomas Koenig <ig25@mvmap66.ciw.uni-karlsruhe.de>
Date: Mon, 10 Feb 1997 03:26:43 -0800 (PST)
To: challenge@list.ee.ethz.ch (challenge)
Subject: What's next?
Message-ID: <199702101024.LAA08950@mvmap66.ciw.uni-karlsruhe.de>
MIME-Version: 1.0
Content-Type: text/plain


Now that we appear to be at a sustainable 300 MK/sec (which I could
hardly believe at first :-), is there any chance we could be attacking
the 56-bit DES key next?

DES is rumoured to be faster than RC5; also, there are likely to
be optimized assembler versions out there already.

We could also make better use of 64-bit architectures, since DES
uses 64-bit blocks.

However (and this is a very big however), that's still a keyspace of
7.2*10^16 keys to search.  Assuming 10^9 keys/second (three times our
current speed, which may be attainable with a good DES implementation)
that's still a bit over two years; too long by a factor of 10 or so.

Soo....

How fast are current DES implementations?  People could try des.c from
the ssh distribution as a starting point.

How much more computing power could we bring online?

Do people have optimized DES for Alpha, UltraSparc, HP 8000 and all
the other nifty 64-bit architectures?

Does it make sense to use MMX or equivalent for DES?
-- 
Thomas Koenig, Thomas.Koenig@ciw.uni-karlsruhe.de, ig25@dkauni2.bitnet.
The joy of engineering is to find a straight line on a double
logarithmic diagram.






{% endraw %}
```

## Thread

+ Return to [February 1997](/archive/1997/02)

+ 1997-02-10 (Mon, 10 Feb 1997 03:26:43 -0800 (PST)) - What's next? - _Thomas Koenig \<ig25@mvmap66.ciw.uni-karlsruhe.de\>_

