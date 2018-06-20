---
layout: default
---

# 1994-03-06 - better way to generate a permutation?

## Header Data

From: Jef Poskanzer \<jef@ee.lbl.gov\><br>
To: cypherpunks@toad.com<br>
Message Hash: 82dbddb5dbaeb58f3c5a4d681c23ab2dd4758d0b44b2adabce671a5fa2f89d84<br>
Message ID: \<9403060145.AA21067@hot.ee.lbl.gov\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-03-06 01:46:04 UTC<br>
Raw Date: Sat, 5 Mar 94 17:46:04 PST<br>

## Raw message

```
{% raw  %}From: Jef Poskanzer <jef@ee.lbl.gov>
Date: Sat, 5 Mar 94 17:46:04 PST
To: cypherpunks@toad.com
Subject: better way to generate a permutation?
Message-ID: <9403060145.AA21067@hot.ee.lbl.gov>
MIME-Version: 1.0
Content-Type: text/plain


I'm putting the polish on pnmstega/pnmdestega.  Currently they spend
the largest part of their time generating the permuted list of bit positions
to use for storing the data bits.  Not surprising, I knew the first
version would be slow - it actually mallocs an array, fills it with
numbers, and shuffles them.  Now I'm looking for suggestions on better
methods.  I looked in Knuth, Sedgewick, and Schneier, and didn't
find anything.  Send email if you've got an idea.  Something with a
bit vector might work.
---
Jef




{% endraw %}
```

## Thread

+ Return to [March 1994](/archive/1994/03)

+ 1994-03-06 (Sat, 5 Mar 94 17:46:04 PST) - better way to generate a permutation? - _Jef Poskanzer \<jef@ee.lbl.gov\>_

