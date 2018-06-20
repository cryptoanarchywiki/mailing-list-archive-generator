---
layout: default
---

# 1995-09-04 - Re: maximizing cryptographic return

## Header Data

From: SINCLAIR  DOUGLAS N \<sinclai@ecf.toronto.edu\><br>
To: vznuri@netcom.com (Vladimir Z. Nuri)<br>
Message Hash: 9108bd3feb87d52c0510e9628f3b7bcd8ebc17ed8ee3db7f734f7afd2defe1ac<br>
Message ID: \<95Sep3.231607edt.994@cannon.ecf.toronto.edu\><br>
Reply To: \<199509040149.SAA01359@netcom10.netcom.com\><br>
UTC Datetime: 1995-09-04 03:16:35 UTC<br>
Raw Date: Sun, 3 Sep 95 20:16:35 PDT<br>

## Raw message

```
{% raw  %}From: SINCLAIR  DOUGLAS N <sinclai@ecf.toronto.edu>
Date: Sun, 3 Sep 95 20:16:35 PDT
To: vznuri@netcom.com (Vladimir Z. Nuri)
Subject: Re: maximizing cryptographic return
In-Reply-To: <199509040149.SAA01359@netcom10.netcom.com>
Message-ID: <95Sep3.231607edt.994@cannon.ecf.toronto.edu>
MIME-Version: 1.0
Content-Type: text/plain


> I was wondering how secure the following algorithm would be for phone
> calls: suppose that at the beginning of each session, the random
> key is traded using RSA or some other very secure approach. the
> key is a *random bit width*, say 100-6000 bits. now, my question is,
> I wonder if some very cheap algorithms, in terms of computation time,
> could be used for the "on the fly" encryption of the voice using those
> bit. would XOR with the pad be totally out of line? 
> 
> the situation is such that trivial algorithms such as XOR with  *unlimited
> cyphertext* can be broken quite trivially. but it seems to me this
> dogma that "XOR is WEAK" is based on the premise that you have a huge
> amount of cyphertext to play with. take away this premise, that you
> have a session key that is guaranteed to really give you very little
> cyphertext, do these supposedly "weak" algorithms then become pretty
> secure?

No, XOR is weak if used even twice.  If you XOR the two pieces of
cyphertext with each other, you get the two plaintexts XORed.  I'd
be willing to bet that the human ear can understand two audio signals
XORed.  Certainly with practice people can understand audio that has
been encrypted with frequency inversion.  Pre-encryption compression
would solve this, but XOR is still very weak.




{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ 1995-09-04 (Sun, 3 Sep 95 18:52:47 PDT) - [maximizing cryptographic return](/archive/1995/09/32fbe29715482d369e0b7ab85f48141f0d01eac41f260813ea7272193aee3bbf) - _"Vladimir Z. Nuri" \<vznuri@netcom.com\>_
  + 1995-09-04 (Sun, 3 Sep 95 20:16:35 PDT) - Re: maximizing cryptographic return - _SINCLAIR  DOUGLAS N \<sinclai@ecf.toronto.edu\>_

