---
layout: default
---

# 1994-03-01 - Insecurity of public key crypto #2 (reply to May)

## Header Data

From: wet!naga (Peter Davidson)<br>
To: cypherpunks@toad.com<br>
Message Hash: 2d05014efea7fbc5c44639cdabefa920070f0fa0bb35ddfbbcccb9055c18d8f9<br>
Message ID: \<m0pbaXM-000C52C@wet.uucp\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-03-01 20:11:49 UTC<br>
Raw Date: Tue, 1 Mar 94 12:11:49 PST<br>

## Raw message

```
{% raw  %}From: wet!naga (Peter Davidson)
Date: Tue, 1 Mar 94 12:11:49 PST
To: cypherpunks@toad.com
Subject: Insecurity of public key crypto #2 (reply to May)
Message-ID: <m0pbaXM-000C52C@wet.uucp>
MIME-Version: 1.0
Content-Type: text/plain



 
[The BBS I use seems to have brain damage.  Apologies if this
has already been posted.]
 
>From: tcmay@netcom.netcom.com (Timothy C. May)
>Subject: Re: Mac encryption
>Date: Wed, 23 Feb 1994 09:56:40 -0800 (PST)
>
>Ron Davis writes:
>
>(quoting me [T.C.M.])
>
>>>MacPGP, available by anonymous ftp from the soda.berkeley.edu site, is
>>>the only one I know of using public key methods, and hence the only
>>>one of real interest to Cypherpunks.
>
>The problem with symmetrical ciphers is one of *scaling*.
>
>Since a key must be exchanged with each other person, the total number
>of keys growns rapidly as the community of participants increases. At
>any stage, the key may be lost, stolen, observed, shared with the
>Feds, etc. A community of 700 participants, as here on Cypherpunks,
>would mean each person would have to generate, exchange (securely!),
>and store 700 specific keys for use just with others.
 
Anybody with 700 co-conspirators is asking for trouble, since at least
one of them is sure to be a federal agent.  Encryption is for concealing
"sensitive" information.  If it's not sensitive, why bother?  If it is
sensitive then you'd better be damn sure you can trust the person you're
sending it to.
 
>This is the famed "key distribution problem."
>
>With public key methods, this problem is largely solved. Each person
>can generate his or her own key, publish the public key part of it,
>and be done with it.
 
It's not that simple.  Terry Ritter has pointed out on sci.crypt that
the problem with PGP is the validation of public keys used.  In other
words, the security hole in the use of PGP is not in the encryption
methods used, or in the use of PGP itself, but in the possibility of
being duped by someone (or some nefarious federal agency) spreading
bogus public keys. It's not enough to have a public key which you
believe is the public key of a person you wish to communicate securely
with - you also have to be sure that the private key which corresponds
to this public key is known only to that person, in other words, that
the public key really did come from the person you believe it came
from.  If you get the (presumed) public key of some person X from some
directory of public keys, or from some third party, how can you be
sure it didn't originate with someone who wants to monitor all the
encrypted messages being sent to X?  Terry Ritter has explained how a
third party can place themselves in the middle of encrypted communications
between two people using PGP and monitor everything they say to each other
- and this without having to crack RSA or IDEA.
 
This method of eavesdropping applies only to public key encryption
systems, not to secret key systems, so I suggest that the latter are
still of interest (even to cypherpunks), not only for encrypting data
that stays on your hard disk but also for encrypted communications.
 

rom owner-cypherpunks  Tue Mar  1 12:11:49 1994
Return-Path: <owner-cypherpunks>
Received: by toad.com id AA28180; Tue, 1 Mar 94 12:11:49 PST
Received: from wet.UUCP by toad.com id AA28156; Tue, 1 Mar 94 12:11:44 PST
Received: by wet.uucp (/\=-/\ Smail3.1.18.1 #18.2)
	id <m0pbaUt-000CAaC@wet.uucp>; Tue, 1 Mar 94 11:52 PST
Message-Id: <m0pbaUt-000CAaC@wet.uucp>
Date: Tue, 1 Mar 94 11:52 PST
From: wet!naga (Peter Davidson)
To: cypherpunks@toad.com
Subject: Insecurity of public key crypto #1 (reply to Mandl)
Sender: owner-cypherpunks@toad.com
Precedence: bulk


 
[My BBS is having fits lately.  Apologies if this has already been posted.]
 
>Date: Wed, 23 Feb 94 12:13:57 EST
>From: dmandl@lehman.com (David Mandl)
>Subject: Re: Mac encryption
>
>The invention (discovery?) of public-key crypto changed the world, and
>makes practical everyday use of crypto infinitely easier.
 
Infinitely?  You mean there is absolutely *no* difficulty involved
in using PGP?  I quit using it up quite a while back.  Couldn't be
bothered with the hassle.
 
>It also makes
>the kinds of specific things cypherpunks are interested in much more
>practical (or POSSIBLE).
 
Digital signatures, yes.  I haven't had a need for 'em so far (I'm not
setting up a digital bank).
 
>If you correspond with hundreds of people on a
>regular basis, including people you don't know and people you may send
>something to once and never deal with again, it is impractical to say the
>least to have to generate and exchange keys.
 
Only "sensitive" information is worth encrypting and if you want to
stay out of trouble you don't go giving sensitive information to
someone you don't know.  A certain mutual knowledge and trust between
two people has to be establish before any exchange of sensitive information.
 
>Why was public key crypto invented at all?  Why are people interested in
>using it?  Practically, it's really fundamentally different from symmetric
>crypto, which is of very limited use in the situation we're all in now
>(anonymous communication, the net, quick hit-and-run dissemination of
>information, digital signatures, etc., etc.).
 
Crypto is for concealing information from those you don't want to see it.
Public key crypto is thus not fundamentally different from symmetric key
crypto.  The difference is in communication of the encryption key, which
is not a fundamental difference.  Both kinds of crypto have problems when
it comes to key distribution.  In the case of secret key the problem is
in keeping the key secret.  In the case of public key the problem is in
validating the public key.
 
>PGP also has the "web of trust" structure built in.
 
"Trust"?  Sure.  Just trust the person you got X's public key from
(who got it from someone who got it from who knows?).  So is X's
public key really X's public key?  Sure, just trust that it's so,
then send X a message and trust that it won't be intercepted by
whoever put out the bogus public key for X.
 




{% endraw %}
```

## Thread

+ Return to [March 1994](/archive/1994/03)

+ Return to "[rcain<span>@</span>netcom.com (Robert Cain)](/authors/rcain_at_netcom_com_robert_cain_)"
+ Return to "[wet!naga (Peter Davidson)](/authors/wetnaga_peter_davidson_)"

+ 1994-03-01 (Tue, 1 Mar 94 12:11:49 PST) - Insecurity of public key crypto #2 (reply to May) - _wet!naga (Peter Davidson)_
  + 1994-03-02 (Tue, 1 Mar 94 17:32:27 PST) - [Re: Insecurity of public key crypto #2 (reply to May)](/archive/1994/03/77a854ef8490930c989c2cb6d375d4ae273ee78acf3aa836be67b8b8ed8834a6) - _rcain@netcom.com (Robert Cain)_

