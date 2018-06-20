---
layout: default
---

# 1996-09-23 - provably hard PK cryptosystems

## Header Data

From: Adam Back \<aba@dcs.ex.ac.uk\><br>
To: cypherpunks@toad.com<br>
Message Hash: fb0b06f4002611df3cd7e2edf7dc5ca05b48bef3bae8bbcfedf7f29e7ac15ff5<br>
Message ID: \<199609222158.WAA00325@server.test.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-09-23 04:26:35 UTC<br>
Raw Date: Mon, 23 Sep 1996 12:26:35 +0800<br>

## Raw message

```
{% raw  %}From: Adam Back <aba@dcs.ex.ac.uk>
Date: Mon, 23 Sep 1996 12:26:35 +0800
To: cypherpunks@toad.com
Subject: provably hard PK cryptosystems
Message-ID: <199609222158.WAA00325@server.test.net>
MIME-Version: 1.0
Content-Type: text/plain



extracting from part of another thread...

Dimitri Vulis <dlv@bwalk.dm.com> writes:
> Adam Back writes:
> > [...] I think I remember that you posted some time ago a way to have
> > two plausible decryptions for one ciphertext, to enable things like
> > duress keys, in terms of RSA.  The problem with this, however is
> > that RSA is currently very slow to use in its pure form for
> > messages.
>
> I don't recall this one... My feeling about RSA is that one of these
> days there will be a breakthrough allowing much faster factorization
> (either through a better algorithm on a conventional computer, or by
> a practical quantum computer) and then all the codes based on
> factorization will become essentially plaintext. It's time to start
> looking for other hard problem to base PKC on.

I'm not sure about quantum computers, some people who know much more
about particle physics than I do seemed initially sceptical, and
didn't think it was doable.  However I have read some optimistic
sounding news clippings (on the list) which sounded as if things are
progressing well, with techniques being found using redundancy to get
around what were earlier problems of reliability.  Is this accurate
reporting (thinking of garbled stories by over enthusiastic
journalists)?  I'd be interested to hear opinions from anyone who does
know about particle physics about the likihood of practical quantum
computers being practical in the next 20 years or so.

RSA has always had problems with two pitfalls in any proof of its
hardness: no proof that RSA is as hard as factoring, and no proof that
factoring is hard.  Rabin and variants of it at least have the proof
of being as hard as factoring.

You mentioned your opinion that a vastly better factoring algorithm
may yet be found.  What about the possibility of finding proof of a
useful lower bound for the complexity of factoring, do you have any
thoughts on the likelihood of this being achieved?  That would be a
very significant result, and in the absence of a quantum attack would
be as good as it gets. It would allow you to make realistic
calculations about physical limits of attacking it, in a similar manner
to the entropy calculations possible for brute force of symmetric
ciphers.  (Heat death of the sun before a solution even if every
particle was part of hardware key cracking computer type arguments).

One other area that did sound promising was some kind of mapping
problem in n dimensional tiling that Tim was discussing at a physical
meet while I was over in the US.  A news clipping posted to
cypherpunks a short time ago was talking about a researcher who had
constructed a crypto system related to the problem of finding paths in
a tiling problem (sounded like the same problem).  The interesting
part was that the researcher was reported as having a proof of
hardness.  Similarly is this being reported accurately?

> E.g., does anyone know of any progress made on public-key
> cryptosystems based on the word problem in semigroups, described in
> Neal Wagner and Marianne Magyarik, _A public key cryptosystem based
> on the word problem_, Advances in Cryptology: Proceedings of Crypto
> '84, G. R. Blakley and D. Chaum, eds., Lecture Notes in Computer
> Sciences #196, Springer Verlag, 1985, and also mentioned in Wayne
> Patterson, _Mathematical Cryptology for Computer Scientists and
> Mathematicians_, Rowman and Littlefield, 1987?

Not familiar with the problem.  Is it something you could explain
briefly, or are there any on-line papers on the subject?

> >From what I neard, NSA tried very hard to implement it and failed,
> and the Soviets actually built a cryptosystem similar to what they
> described. I tried to duplicate what the Soviets supposedly did, but
> without success.

Adam
--
#!/bin/perl -sp0777i<X+d*lMLa^*lN%0]dsXx++lMlN/dsM0<j]dsj
$/=unpack('H*',$_);$_=`echo 16dio\U$k"SK$/SM$n\EsN0p[lN*1
lK[d2%Sa2/d0$^Ixp"|dc`;s/\W//g;$_=pack('H*',/((..)*)$/)




{% endraw %}
```

## Thread

+ Return to [September 1996](/archive/1996/09)

+ 1996-09-23 (Mon, 23 Sep 1996 12:26:35 +0800) - provably hard PK cryptosystems - _Adam Back \<aba@dcs.ex.ac.uk\>_

