---
layout: default
---

# 1997-07-30 - Re: Cryptography Question (I hope it's not off-topic on this list)

## Header Data

From: Paul Bradley \<paul<span>@</span>fatmans.demon.co.uk\><br>
To: cypherpunks@Algebra.COM<br>
Message Hash: cc4dcd35b0ccacb6cd6f3936a5bbc89fa6a39ae827aed32f2634eda406ec42d0<br>
Message ID: \<Pine.LNX.3.91.970728211016.884C-100000@fatmans.demon.co.uk\><br>
Reply To: \<199707281537.RAA09388@basement.replay.com\><br>
UTC Datetime: 1997-07-30 18:01:15 UTC<br>
Raw Date: Thu, 31 Jul 1997 02:01:15 +0800<br>

## Raw message

```
{% raw  %}From: Paul Bradley <paul@fatmans.demon.co.uk>
Date: Thu, 31 Jul 1997 02:01:15 +0800
To: cypherpunks@Algebra.COM
Subject: Re: Cryptography Question (I hope it's not off-topic on this list)
In-Reply-To: <199707281537.RAA09388@basement.replay.com>
Message-ID: <Pine.LNX.3.91.970728211016.884C-100000@fatmans.demon.co.uk>
MIME-Version: 1.0
Content-Type: text/plain





>   e.g. - If only 56-bit encryption becomes legal, is there a method
> of *chaining* several passes of 48-bit encryption which would make it
> just as hard to break as 96/192/384-bit (etc.) encryption?

This is a similar idea to implementing, say DES, with independent 
subkeys. Layering encryption in this manner makes the plaintext more 
difficult to determine providing that:

a. The involved cryptosystem is not a group, or does not posess strong 
group like properties (eg. There are no large subgroups).

b. Independent keys are used for each encryption

For a good example of a particular case of your idea see 3DES

>   If this is indeed impossible, then perhaps the government might pass
> a law that makes it illegal to encrypt an encrypted file, but experience
> seems to suggest that any law passed always leaves a loophole or back
> door for inventive people to circumvent it.

This law would be difficult to pass, because it is essentially saying 
some sets of data may be encrypted and some not, and there are lots of 
ways out to give plausible deniability "It isn`t an encrypted file 
officer, it`s random bits being encrypted as cover traffic", if the 
cryptosystem is strong the cyphertext shouldn`t be distinguishable from 
random values.

As for circumventing it, any law such as this should just be ignored.

        Datacomms Technologies data security
       Paul Bradley, Paul@fatmans.demon.co.uk
  Paul@crypto.uk.eu.org, Paul@cryptography.uk.eu.org    
       Http://www.cryptography.home.ml.org/
      Email for PGP public key, ID: FC76DA85
     "Don`t forget to mount a scratch monkey"






{% endraw %}
```

## Thread

+ Return to [July 1997](/archive/1997/07)

+ Return to "[iang<span>@</span>cs.berkeley.edu (Ian Goldberg)](/author/iang_at_cs_berkeley_edu_ian_goldberg_)"
+ Return to "[nobody<span>@</span>REPLAY.COM (Anonymous)](/author/nobody_at_replay_com_anonymous_)"
+ Return to "[Paul Bradley <paul<span>@</span>fatmans.demon.co.uk>](/author/paul_bradley_paul_at_fatmans_demon_co_uk_)"

+ 1997-07-28 (Mon, 28 Jul 1997 23:51:36 +0800) - [Cryptography Question (I hope it's not off-topic on this list)](/archive/1997/07/a2ecfe39f88227814a37116bae82bd09eeba3de0efc418eb378e3051bf4b5e01) - _nobody@REPLAY.COM (Anonymous)_
  + 1997-07-30 (Thu, 31 Jul 1997 02:01:15 +0800) - Re: Cryptography Question (I hope it's not off-topic on this list) - _Paul Bradley \<paul@fatmans.demon.co.uk\>_
  + 1997-07-30 (Thu, 31 Jul 1997 04:30:22 +0800) - [Re: Cryptography Question (I hope it's not off-topic on this list)](/archive/1997/07/c811fb4b93a7b7806839a65c8bc727c0a21c327d405d5c4682ee84aa900f8556) - _iang@cs.berkeley.edu (Ian Goldberg)_

