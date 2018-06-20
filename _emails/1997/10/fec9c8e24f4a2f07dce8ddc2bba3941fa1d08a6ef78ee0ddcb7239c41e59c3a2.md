---
layout: default
---

# 1997-10-16 - Re: Security flaws introduced by "other readers" in CMR

## Header Data

From: Anonymous \<nobody@REPLAY.COM\><br>
To: cypherpunks@cyberpass.net<br>
Message Hash: fec9c8e24f4a2f07dce8ddc2bba3941fa1d08a6ef78ee0ddcb7239c41e59c3a2<br>
Message ID: \<199710161715.TAA21716@basement.replay.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-10-16 17:39:41 UTC<br>
Raw Date: Fri, 17 Oct 1997 01:39:41 +0800<br>

## Raw message

```
{% raw  %}From: Anonymous <nobody@REPLAY.COM>
Date: Fri, 17 Oct 1997 01:39:41 +0800
To: cypherpunks@cyberpass.net
Subject: Re: Security flaws introduced by "other readers" in CMR
Message-ID: <199710161715.TAA21716@basement.replay.com>
MIME-Version: 1.0
Content-Type: text/plain



Let's look a little closer at the kinds of access and notice available in
the PGP system compared to alternatives.

As several people have pointed out, no encryption system can provide
protection against what is done with the message after it is decrypted.
The receiver could share it with whoever he wants to, or whoever he is
forced to.

Consider the following scenarios:

 - An encrypted message is sent to someone at his workplace using current
   systems like PGP 2.6.

 - An encrypted message is sent to someone at his workplace, who is using the
   message access features of PGP 5.5.  The corporation key is marked as
   "optional", and the message is not encrypted to that extra key.

 - An encrypted message is sent as before, but this time the message is
   encrypted to the corporate key.

 - An encrypted message is sent to someone at his workplace, who is using
   a different form of corporate access which relies on key escrow
   or automatic acquisition of cleartext.

We agree that none of these systems can provide complete protection
against third party access.  In any of them, the receiver could be forced
to turn over the encrypted message.  But there is still a difference.

In the first two scenarios, the expectation of privacy is the same.
You are encrypting to a personal key at a business address, but you
expect that you would know about it if the data were being provided to
a third party.  There is no widespread installed base of software which
provides secret access after the message is decrypted.

In fact, the second scenario arguably provides slightly more privacy
than the first, which is what we have now.  The reason is that in the
second scenario, the company provides an optional mechanism for business
mail to be recoverable, but also provides an explicit, sender-controlled
escape clause.  The company is granting an explicit expectation of privacy
by allowing the corporate key recipient to be removed.  With usage of
older versions of PGP, there was really no way for the company to even
inform the sender about whether it was going to be reading the mail.

In the third scenario, where you encrypt to the corporate key, there is
no expectation of privacy.  All parties, the sender, the receiver, and
the company, know that the data is being made available to the business.
There is not much privacy here; what you have is business security.  This
mode would be used for business documents and business communications.

In the fourth scenario, which some people are offering as a superior
approach, the expectation of privacy is much less clear.  Unlike in the
current PGP approach, where the design of the corporate access system
is oriented around notifying the sender and receiver, a key escrow or
plaintext recovery system inherently provides no such notice.

This is different from the status quo.  We are talking about a commercial
product which provides automatic corporate access to communications.
Widespread installation and use of this alternate version of PGP
inherently changes the assumptions and expectations that you will have
when you encrypt to someone at work.  Given the company's desire for
message access, this approach implies that you must conservatively assume
that most encryption to a business address will be read.

The PGP system is designed to avoid this.  It provides another method
for corporate access, a visible and explicit method.  It is intended as
an alternative to key escrow and other systems which recovery data after
the recipient gets it.  PGP's third party recipient feature is designed
to prevent the creation of an installed base of escrowed keys and after
the fact third party access software.

Even if the encryption system provides a way for the user to mark his
keys as being escrowed or otherwise providing third party access,
the system is not self-correcting in the way the PGP system is.
It would be much easier for a business owner to pervert a secretive
access system than one like PGP.  The company could install the access
features but not tell its employees that their keys were being escrowed,
or that their mail client was secretly storing a copy of all plaintexts.
This kind of change would be easy to make with the after-the-fact access
systems some people are proposing.  Yes, theoretically this can be done
with any encryption system (as all agree) but the point is to avoid the
widespread distribution of software which invites this kind of abuse.
The PGP system is designed to satisfy business needs without leading us
into this dangerous situation.

A world in which third party encryption by the sender is the normal and
widespread method for corporate access is one with increased privacy and
more visibility of access.  The alternatives which have been proposed are
prone to abuse and provide less visibility.  They lead us towards a world
in which there is no expectation of privacy even for encrypted messages,
by providing an installed base of snooping software.  The PGP approach
is explicitly designed to keep us out of that world, by removing the need
for that kind of software.





{% endraw %}
```

## Thread

+ Return to [October 1997](/archive/1997/10)

+ 1997-10-16 (Fri, 17 Oct 1997 01:39:41 +0800) - Re: Security flaws introduced by "other readers" in CMR - _Anonymous \<nobody@REPLAY.COM\>_
  + 1997-10-16 (Fri, 17 Oct 1997 02:53:40 +0800) - [Re: Security flaws introduced by "other readers" in CMR](/archive/1997/10/7182430d30ab413ba14df36c8a6f981b99ab1bdab7accf5f06a4af81dab7095c) - _Tim May \<tcmay@got.net\>_

