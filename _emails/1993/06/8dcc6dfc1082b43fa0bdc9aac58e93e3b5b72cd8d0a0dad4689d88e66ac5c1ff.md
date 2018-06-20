---
layout: default
---

# 1993-06-17 - Re: Weak steganography

## Header Data

From: kqb@whscad1.att.com<br>
To: cypherpunks@toad.com<br>
Message Hash: 8dcc6dfc1082b43fa0bdc9aac58e93e3b5b72cd8d0a0dad4689d88e66ac5c1ff<br>
Message ID: \<9306172216.AA11412@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-06-17 22:16:40 UTC<br>
Raw Date: Thu, 17 Jun 93 15:16:40 PDT<br>

## Raw message

```
{% raw  %}From: kqb@whscad1.att.com
Date: Thu, 17 Jun 93 15:16:40 PDT
To: cypherpunks@toad.com
Subject: Re: Weak steganography
Message-ID: <9306172216.AA11412@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


Hal Finney said:

> Another problem is that encrypted files look different from executable
> files.  Encrypted files have a uniform histogram (that is, all 256 different
> possible byte values are equally frequent), but exe files do not.  ...

I am building a "steganosaurus" and eventually will need to solve a
similar problem.  (A "steganosaurus" applies a primitive steganographic
technique to English text by using a thesaurus to generate enough word
variation to encode a hidden message.)  One of the weaknesses of this
"steganosaurus" is that the resulting output has statistical differences
from normal English text.  For example, word frequency will be skewed.

Worse, I have to assume that the eavesdropper knows my steganization
algorithm and can "desteganize" any innocuous-looking text I produce.
That "desteganized" text will show clearly the existence of a hidden,
encrypted message because, as Hal pointed out, it has a uniform histogram.

What I want is a program that will transform an encrypted file to a
(slightly larger) file that mimics the distribution achieved by
applying the "desteganization" algorithm to normal English text
that does *not* contain any hidden message.  The steganization
algorithm then gets applied to this stealthy, mimic file, not
directly to the encrypted hidden message.  By the way, since we
must assume that the eavesdropper knows all our algorithms but
not our secret keys, this algorithm will require a *second* secret
key in addition to the secret key used in the original encryption.
I'm not ready to tackle that yet.  Unless I hear otherwise, I'll
assume that if anyone knows how to achieve this, they're not telling...

                              Kevin Q. Brown
                              INTERNET    kqb@whscad1.att.com
                                 or       kevin_q_brown@att.com

PS: I found that a simple, semi-automatic algorithm can generate a
    public message only 5 to 10 times as long as the hidden message.
    Unfortunately, the public message from my simple algorithm is
    almost always a bizarre, disconnected sequence of rants, which,
    for most people, is not normal.  That is why I am building my
    "steganosaurus".  After that I will see if combining a natural
    language parser with transformational grammars can produce a
    less primitive, more efficient "trans-steganosaurus".




{% endraw %}
```

## Thread

+ Return to [June 1993](/archive/1993/06)

+ 1993-06-17 (Thu, 17 Jun 93 15:16:40 PDT) - Re: Weak steganography - _kqb@whscad1.att.com_

