---
layout: default
---

# 1997-10-22 - Re: shared keys, proxy encryption (was Re: PGP 5.5 CMR/GAK: a possible solution)

## Header Data

From: Jon Callas \<jon@pgp.com\><br>
To: Adam Back \<mark@unicorn.com<br>
Message Hash: c6b2bdbf188270bccfbf5c18dc2beccac6c97dd7b0ee2bc854ea9ee8b4e73641<br>
Message ID: \<3.0.3.32.19971022120251.00bf7b30@mail.pgp.com\><br>
Reply To: \<877514566.20581.193.133.230.33@unicorn.com\><br>
UTC Datetime: 1997-10-22 19:17:10 UTC<br>
Raw Date: Thu, 23 Oct 1997 03:17:10 +0800<br>

## Raw message

```
{% raw  %}From: Jon Callas <jon@pgp.com>
Date: Thu, 23 Oct 1997 03:17:10 +0800
To: Adam Back <mark@unicorn.com
Subject: Re: shared keys, proxy encryption (was Re: PGP 5.5 CMR/GAK: a possible solution)
In-Reply-To: <877514566.20581.193.133.230.33@unicorn.com>
Message-ID: <3.0.3.32.19971022120251.00bf7b30@mail.pgp.com>
MIME-Version: 1.0
Content-Type: text/plain



At 01:46 PM 10/22/97 +0100, Adam Back wrote:
   
   Mark Grant <mark@unicorn.com> writes:
   > The current system sends out a user's personal key, with a tag to say
that
   > if I don't encrypt to the company as well, my mail will bounce. But think
   > about this: how often do I want to send email to a particular person in a
   > company, and ensure that only they see it? And how often do I want to
send
   > mail to a particular group inside a company? All I want is to ensure that
   > I get a response from the company, I usually don't care who I talk to
in the
   > process.
   
   The CMR feature in pgp5.5 isn't so far intented to cope with this
   scenario I think.  That's because pgp5.5 I understand can only
   generate keys with one CMR request field.

Well, Adam, you are yet again describing it wrong. You can put in N of
them. You are right that the 5.5 UI isn't general. Something had to slip.
Also, there's another thing you're not describing correctly. This is not a
feature of the key -- it's a feature of the user name, and included in a
user name's self signature. It can be changed at any time, and you can even
have an ambivalent key that has a username with the CMR packet
(salesdweeb@foobar.com) and a without it (jblow@foobar.com).
   
   Problem for both approaches is re-keying: what happens when Fred
   leaves the sales team to work for a competitor.  Revoke the shared key
   and start over?  Or with the CMR method, revoke just the CMR request
   for Fred, and allow key servers to remove CMR requests when presented
   with a suitable CMR request revocation cert?  (How often will senders
   check key servers for revocation certs?)  Or have short expiries on
   encryption-only keys (one per day?), so that they key update happens
   soon enough anyway.  (pgp5.x allows for short lived encryption keys
   directly because of the separation of signature and encryption keys,
   the WoT applies to the signature key).

This is why any sort of shared or escrowed keys suck. But in most cases
it's good enough, because when Fred leaves sales, he loses access to the
sales computers. In most of these cases, when someone decrypts something
with the sales key, it ends up going into the order system in plaintext
anyway.

However, one of the features of the new PGP key format is that you can
change encryption keys easily. If you
   
   Really it seems to me that actually having half a dozen sales droids
   sharing a key, or being able to decrypt a message because they are all
   CMR enforced multiple crypto recipients is a security nightmare either
   way :-)
   
   Reckon it would be arguably more secure to have the SMTP policy
   enforcer decrypt it for them, even.

Really? You think the SMTP agent should be decrypting? Wow. I don't. I
think that's *really* intrusive, and worse than what we did. Interestingly
enough, there are a number of people (like Bruce Schneier) who have no
problem with the additional encryption part, but think that the SMTP agent
is the work of the devil. Expect pushback.
   
   Another method of authenticating TLS is to base the authentication on
   the user's PGP WoT.  Include authentication information to the
   delivery agent which is capable of TLS, which is also exchanged inside
   the encryption envelope.  (Eg. transfer an authentication symmetric
   key k1 inside the encryption envelope; send the local TLS capable SMTP
   hub / SMTP policy enforcer the key k1.  The TLS forward secret key
   negotiation can then be authenticated using this key.  The remote TLS
   system can tack the authentication information on to the delivered
   message, in a header, or otherwise, and the recipient can check the
   authentication).

Note that the user's WoT is stored in the user's keyring. There's an
operational problem here. This means that the MTA has to have access to all
users' pubrings. This is not a good thing, to my mind.
   
   > So PGP's "everything private unless you choose to make it public" system
   > seems backwards. Surely what we really need to meet these customer
demands
   > is an "everything public (within the company) unless you choose to
make it
   > private" system? That is, all mail to my department inside the company
   > should be encrypted to a department key, shared by all members, *unless*
   > it is confidential, in which case it should *only* be encrypted to me. 
   
   I think what PGP are arguing for is ability to recover stored messages
   even if they are intended for one recipient only.  As I think has been
   established this can be acheived by storage recovery, without exposing
   communications traffic to the associated risks.  It is possible that
   there is an unstated perceived user requirement, that the messaging
   standard be able to allow third party access to the communications
   traffic directly.

Nope, that's not what we're arguing for. What we're arguing for is an
alternative to key escrow -- the kind where your employer keeps your secret
key just in case they need it.

	Jon





-----
Jon Callas                                  jon@pgp.com
Chief Scientist                             555 Twin Dolphin Drive
Pretty Good Privacy, Inc.                   Suite 570
(415) 596-1960                              Redwood Shores, CA 94065
Fingerprints: D1EC 3C51 FCB1 67F8 4345 4A04 7DF9 C2E6 F129 27A9 (DSS)
              665B 797F 37D1 C240 53AC 6D87 3A60 4628           (RSA)





{% endraw %}
```

## Thread

+ Return to [October 1997](/archive/1997/10)

+ 1997-10-22 (Wed, 22 Oct 1997 18:10:30 +0800) - [PGP 5.5 CMR/GAK: a possible solution](/archive/1997/10/facc384450f56b9f115ec7d685384dbffe1df9b3c5b264f62ad375e3564ed0e8) - _mark@unicorn.com_
  + 1997-10-22 (Wed, 22 Oct 1997 19:57:44 +0800) - [Re: PGP 5.5 CMR/GAK: a possible solution](/archive/1997/10/65957c4a48ba38555cb02a867bbe959c74fdb9d037af6a3acdc514ca6ce6882d) - _amp@pobox.com_
  + 1997-10-22 (Wed, 22 Oct 1997 21:05:08 +0800) - [shared keys, proxy encryption (was Re: PGP 5.5 CMR/GAK: a possible solution)](/archive/1997/10/5270def84ea89fd3ef229f579bcf198f1272f0cac61b3d036bf3fec4ebbee344) - _Adam Back \<aba@dcs.ex.ac.uk\>_
  + 1997-10-22 (Thu, 23 Oct 1997 02:58:27 +0800) - [Re: PGP 5.5 CMR/GAK: a possible solution](/archive/1997/10/d82c9940c0384252d62bfcd498c30b9785151a1a509ec475071819e33672106e) - _Jon Callas \<jon@pgp.com\>_
    + 1997-10-22 (Thu, 23 Oct 1997 04:42:37 +0800) - [Re: PGP 5.5 CMR/GAK: a possible solution](/archive/1997/10/5650f0adabd87c84d9aece927b3c6cdb80d391b71708ee83ee1acf0363798bf0) - _Adam Back \<aba@dcs.ex.ac.uk\>_
    + 1997-10-23 (Thu, 23 Oct 1997 08:07:27 +0800) - [Re: PGP 5.5 CMR/GAK: a possible solution](/archive/1997/10/cc09cff2f2a3204196385db80840337a537adc61afcdc14f288e16e17b5db526) - _jmayorga@netscape.com (John Mayorga)_
  + 1997-10-22 (Thu, 23 Oct 1997 03:17:10 +0800) - Re: shared keys, proxy encryption (was Re: PGP 5.5 CMR/GAK: a possible solution) - _Jon Callas \<jon@pgp.com\>_
    + 1997-10-22 (Thu, 23 Oct 1997 04:45:37 +0800) - [Re: shared keys, proxy encryption (was Re: PGP 5.5 CMR/GAK: a possible solution)](/archive/1997/10/e6c13b76b70d4284c5f23737c49ddaacc55c698b413ba6ded09756480243ffe2) - _Adam Back \<aba@dcs.ex.ac.uk\>_
      + 1997-10-23 (Thu, 23 Oct 1997 21:42:02 +0800) - [Re: shared keys, proxy encryption (was Re: PGP 5.5 CMR/GAK: a](/archive/1997/10/6c2684ffec84ff729684b7046c99a5795b4cc1d1b93f3e8fd134f95d48d1acd1) - _lutz@taranis.iks-jena.de (Lutz Donnerhacke)_
  + 1997-10-22 (Thu, 23 Oct 1997 04:25:05 +0800) - [Re: PGP 5.5 CMR/GAK: a possible solution](/archive/1997/10/407a1d3515babdbcae470082881f78ad3f9a12b1846206b0f0c137d0e6ad613a) - _Tim May \<tcmay@got.net\>_
  + 1997-10-23 (Thu, 23 Oct 1997 21:41:58 +0800) - [Re: shared keys, proxy encryption (was Re: PGP 5.5 CMR/GAK: a](/archive/1997/10/cfd235ad4279c62e6d50d44323760d1439b22b9a8330eac181e773de55c823cd) - _lutz@taranis.iks-jena.de (Lutz Donnerhacke)_

