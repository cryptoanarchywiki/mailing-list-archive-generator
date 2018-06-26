---
layout: default
---

# 1993-10-22 - Sharing a secret

## Header Data

From: hfinney<span>@</span>shell.portal.com (Hal Finney)<br>
To: cypherpunks@toad.com<br>
Message Hash: b98fe5afef72a6c65ca1b097df41f3df0e9ed4ddf2fbb20a1c1f427c2cac8be8<br>
Message ID: \<9310221637.AA01633@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-10-22 16:38:17 UTC<br>
Raw Date: Fri, 22 Oct 93 09:38:17 PDT<br>

## Raw message

```
{% raw  %}From: hfinney@shell.portal.com (Hal Finney)
Date: Fri, 22 Oct 93 09:38:17 PDT
To: cypherpunks@toad.com
Subject: Sharing a secret
Message-ID: <9310221637.AA01633@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


I will give a simple example of Shamir secret sharing.  Suppose you have
some data D which you want to split up into n pieces such that any 2
of them are sufficient to reconstruct D.  Shamir solves the problem for
any k of them being sufficient, but the case k=2 is especially simple.

Pick a random number m which will be the slope of a line.  Take the
equation y = mx + D, and substitute x = 1, x = 2, ... x = n.  Pass out
the y's for each value of x as the secret shares.

For example, if D=12, pick random m = 4, and pass out (1,16), (2,20),
(3,24), (4,28), and so on.

Now, suppose an enemy gets hold of one of these - say (2,20).  What does
this tell him about the value of D?  Nothing!  D could be anything,
depending on the value of m.

But suppose we have two of these values - say (1,16) and (2,20).  From
these it is easy to calculate m=4, and from that it is easy to see that
D=12.  Two points determine a line.

In the actual Shamir scheme, integers mod a prime p are used, where p>D.
The math is basically the same.  For k=3, a parabola is used instead of
a line, so that 3 points are needed; for k=4, a third-degree polynomial
is used, and for general k, a (k-1)-degree polynomial is used.  In each
case, knowing k-1 points tells you nothing, because there will be a
(k-1)-degree polynomial that would pass through any possible value of
D.

Hal




{% endraw %}
```

## Thread

+ Return to [October 1993](/archive/1993/10)

+ Return to "[hfinney<span>@</span>shell.portal.com (Hal Finney)](/author/hfinney_at_shell_portal_com_hal_finney_)"
+ Return to "[Matthew J Ghio <mg5n+<span>@</span>andrew.cmu.edu>](/author/matthew_j_ghio_mg5n_at_andrew_cmu_edu_)"

+ 1993-10-22 (Fri, 22 Oct 93 09:38:17 PDT) - Sharing a secret - _hfinney@shell.portal.com (Hal Finney)_
  + 1993-10-22 (Fri, 22 Oct 93 13:33:18 PDT) - [Re: Sharing a secret](/archive/1993/10/8d808728fac34b5ee5e5fbc8898755027113aa7311bffdd3a33d7f59ca346aa3) - _Matthew J Ghio \<mg5n+@andrew.cmu.edu\>_

