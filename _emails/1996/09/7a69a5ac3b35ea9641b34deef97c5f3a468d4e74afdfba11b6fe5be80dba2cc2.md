---
layout: default
---

# 1996-09-07 - non-interactive forward secrecy

## Header Data

From: Adam Back \<aba<span>@</span>dcs.ex.ac.uk\><br>
To: coderpunks@toad.com<br>
Message Hash: 7a69a5ac3b35ea9641b34deef97c5f3a468d4e74afdfba11b6fe5be80dba2cc2<br>
Message ID: \<199609062108.WAA00230@server.test.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-09-07 16:54:05 UTC<br>
Raw Date: Sun, 8 Sep 1996 00:54:05 +0800<br>

## Raw message

```
{% raw  %}From: Adam Back <aba@dcs.ex.ac.uk>
Date: Sun, 8 Sep 1996 00:54:05 +0800
To: coderpunks@toad.com
Subject: non-interactive forward secrecy
Message-ID: <199609062108.WAA00230@server.test.net>
MIME-Version: 1.0
Content-Type: text/plain



[This discussion is driven by the desirability of having forward
secrecy in mixmaster for the mix packets delivered by email where the
interactive nature of normal DH is incovenient]

Anyone have any ideas for a non-interactive forward secrecy protocol?

Aside from actually doing the DH key exchange via email (painful), I
have one suggestion for a protocol, perhaps people can improve on
this:

Assuming common prime p, and generator g:

Two remailers A and B.  A wants to send messages to B without having to
wait for replies from B.

B generates ys (y0,y1,...,yn), 

	where y(i+1) = hash(y(i))

then computes Ys (Y0,Y1,...,Yn)

	where Y(i) = g ^ y(i) mod p

B sends A Ys, and discards ys.

Now A can send B n consecutive packets with forward secrecy before
receiving any more packets from B.

(B keeps y0, and overwrites it with y1 = hash(y0), etc, so that all B
ever has to hand is the current y(i), and y(i-1) is hard to compute
from y(i) because of the hash functions properties.)

This isn't truly non-interactive, it just reduces the number of
interactions, to an interactive exchange in 1 out of n cases.

(you could randomly chose ys rather than having related ys, and delete
y(i) after use, but this has higher storage requirements (n rather
than 1 on the recipient)).


Heres the obvious construction for a truly non-interactive forward
secrecy protocol based on DH.  (That is it only requires 1
interactive exchange).

Aside from the obvious of having a huge n, and the above protocol,
which would have large space requirements, what we're after is a way
to do this with negligable space requirements.

Say that we have the two parties Alice and Bob.  Bob doesn't loose
much by having his secret (x) related as above.

1.	x(i+1) = f1( x(i) )
2.	X(i+1) = f2( X(i) )
3.      f1 is non reversible

f1 should have hash-like properties (it should be non-reversible).

Do functions f1 and f2 satisfying 1, 2 and 3 exist?  Is there another
way to achieve this?

(My closest attempt so far, based on the hardness of discrete square roots:

	f1(x) = x^2 (mod p)
	f2(X) = X^2 (mod p)

doesn't work because g^(x^2 mod p) mod p != g^(x^2) mod p)

Adam
--
#!/bin/perl -sp0777i<X+d*lMLa^*lN%0]dsXx++lMlN/dsM0<j]dsj
$/=unpack('H*',$_);$_=`echo 16dio\U$k"SK$/SM$n\EsN0p[lN*1
lK[d2%Sa2/d0$^Ixp"|dc`;s/\W//g;$_=pack('H*',/((..)*)$/)




{% endraw %}
```

## Thread

+ Return to [September 1996](/archive/1996/09)

+ Return to "[Adam Back <aba<span>@</span>dcs.ex.ac.uk>](/author/adam_back_aba_at_dcs_ex_ac_uk_)"

+ 1996-09-07 (Sun, 8 Sep 1996 00:54:05 +0800) - non-interactive forward secrecy - _Adam Back \<aba@dcs.ex.ac.uk\>_

