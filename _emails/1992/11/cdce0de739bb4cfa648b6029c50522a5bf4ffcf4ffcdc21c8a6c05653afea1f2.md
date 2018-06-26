---
layout: default
---

# 1992-11-30 - Re: Secure Key exchange

## Header Data

From: pfarrell<span>@</span>cs.gmu.edu (Pat Farrell)<br>
To: tytso@ATHENA.MIT.EDU<br>
Message Hash: cdce0de739bb4cfa648b6029c50522a5bf4ffcf4ffcdc21c8a6c05653afea1f2<br>
Message ID: \<9211301910.AA11750@cs.gmu.edu\><br>
Reply To: _N/A_<br>
UTC Datetime: 1992-11-30 19:11:12 UTC<br>
Raw Date: Mon, 30 Nov 92 11:11:12 PST<br>

## Raw message

```
{% raw  %}From: pfarrell@cs.gmu.edu (Pat Farrell)
Date: Mon, 30 Nov 92 11:11:12 PST
To: tytso@ATHENA.MIT.EDU
Subject: Re: Secure Key exchange
Message-ID: <9211301910.AA11750@cs.gmu.edu>
MIME-Version: 1.0
Content-Type: text/plain


	tytso@ATHENA.MIT.EDU (Theodore Ts'o) wrote:
	  quoting: pfarrell@cs.gmu.edu (Pat Farrell)
	   I sign keys only when I am certian that the key belongs to 
           the human who claims to have the name on the key. There 
           are not a lot of keys signed by me floating arround, maybe 
           six total.....
  tt> 
  tt> Ah, but how do we know that it's really you making this statement, and
  tt> not some evil NSA spoofer?  What people need to do is to make their
  tt> key-signinging policies available _signed_ with their private key; that
  tt> way at least we would know that the entity signing the keys and the
  tt> entity claiming that this is its policy are the same.  
Exellent point. I'll put a signed statement of my policy in my
.plan. It won't add many characters, and anyone can find it by
fingering me. (and I've never claimed I don't work for
NSA/CIA/...)

  tt>         This helps, but
  tt> we would then still need to trust that the entity is telling the truth
  tt> insofar as its key-signing policy is concerned.
I can't solve this one so easily. I have two ideas that can
help:
	1. change PGP in future versions (starting with 2.1?)
so it doesn't ask for confirmation every time a key is added
to the ring. Make the user do an active action, rather than a
half-asleep y<cr> to sign a key.

	2. store a comment in my secret ring that is captured
each time I sign a key. Thus I could store the
"reason/justification" for the signature to jog my memory. I
know whose key's I've signed now, but as the number gets bigger, then
I'll need a memory aid. I suggest the secret ring, as I share
my public ring, and don't think that why I chose to sign a key
should be generally available. If this were supported, you
could then send me a msg asking "why did you sign John Doe's
key?" You would have to compare my answer to my published
policy and make your own judgement as to whether I follow it.

I could keep track of this manually, and should. But PGP
already requires me to have a lot of files arround.

Pat

Pat Farrell,      Grad Student                       pfarrell@cs.gmu.edu
Department of Computer Science, George Mason University, Fairfax, VA
PGP key available via finger or request           #include standard.disclaimer
Write PKP. Offer money for a personal use license for RSA.




{% endraw %}
```

## Thread

+ Return to [November 1992](/archive/1992/11)

+ Return to "[pfarrell<span>@</span>cs.gmu.edu (Pat Farrell)](/author/pfarrell_at_cs_gmu_edu_pat_farrell_)"

+ 1992-11-30 (Mon, 30 Nov 92 11:11:12 PST) - Re: Secure Key exchange - _pfarrell@cs.gmu.edu (Pat Farrell)_

