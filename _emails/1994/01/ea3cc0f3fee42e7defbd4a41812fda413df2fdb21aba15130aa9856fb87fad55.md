---
layout: default
---

# 1994-01-24 - Remailer Policies

## Header Data

From: wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)<br>
To: cypherpunks@toad.com<br>
Message Hash: ea3cc0f3fee42e7defbd4a41812fda413df2fdb21aba15130aa9856fb87fad55<br>
Message ID: \<9401240615.AA19817@anchor.ho.att.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-01-24 06:16:35 UTC<br>
Raw Date: Sun, 23 Jan 94 22:16:35 PST<br>

## Raw message

```
{% raw  %}From: wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)
Date: Sun, 23 Jan 94 22:16:35 PST
To: cypherpunks@toad.com
Subject: Remailer Policies
Message-ID: <9401240615.AA19817@anchor.ho.att.com>
MIME-Version: 1.0
Content-Type: text/plain


A certain Tentacle of Medusa writes about problems with anonymous
remailers being abused, and apparently speaks with some experience
about mailbombing and other obnoxious behaviour.  He suggests a few
policies that he'd like somebody to enforce on remailer operators,
as near as I can tell?

> 1. Remailers should *not* be able to send anything to any list on the
> Lists of Lists or any other known mailing list, by default. If the
> moderator approves it, the remailers are allowed.

Unless you control all the mail-users in the world, you can't stop this.
On the other hand, it would be good if the standard remailer tools
make it easy for remailer-operators to prevent the remailer from
sending mail to specified destinations, and perhaps to restrict
mail originating *from* certain users either in general or to
specific destinations.  The latter are more difficult, since
networks of remailers do tend to make it difficult to tell
where mail really came from, but sometimes remailer-operators 
need to do this in self-defense.

It would also be worthwhile and courteous for remailer-operators to
decide policies for blocking remailing.  For example,
Julf's anon.penet.fi remailer doesn't post news anonymously
to newsgroups that have voted that they don't want it,
and he's had to deal with a number of abusive users who he's blocked.

> 2. Mailbombing through the remailers should be dampened with
> limitations on the size of messages and the frequency.

This is difficult to define or implement.  I can often recognize
mailbombing when I see it, if it's unencrypted, but a remailer
operator has trouble determining whether something is a long train
of abuses, or merely the transactions from the First Digital Bank
Anonymous Credit Card or the responses from the ftp-by-mail server
at NASA that somebody really wanted.  On the other hand,
letting a recipient specify throttles would be useful,
and charging for remailing (whether by message, by size, or both)
can also cut down on abuse.

> 3. The ability for *anyone* to state that they do not want to receive
> anonymous mail should be *automated*-- and the remailers should act as
> a *whole network* in propagating these `requests for denial' between them.
It's not difficult, if you're using a modern mail system,
to filter out messages based on anything you can easily automate.
There are some mailing list handlers, like the ones the Extropians bought
for their list, that are friendly and flexible about it,
so you can decide who to exclude, and a next generation of
anonymous remailers should probably include similar capabilities.
On the other hand, it's about like junk mail - there are groups of
junk mail senders who will drop you from their list by a single request,
and other junk mail senders who buy those requests to target you :-)

I'd personally be disturbed if the software easily supported
this sort of voluntary blacklisting without good authentication,
since otherwise one of your Medusa buddies will go around unsubscribing
people from anonymous remailer lists who don't want to unsubscribe;
digicash banks and customers and political organizers are particularly
vulnerable to this kind of abuse.

> 4. You should keep and pass around lists of people that have caused one
> remailer operator problems, so that others have the option of denying service.
I thought *you* were the one who was just complaining about
remailer operators who divulge the identity of their users,
though maybe I misinterpreted you.  While people who abuse
remailers as publicly as you do are easy to put on these lists,
most abusers are probably doing so for the fun of abusing people
rather than to make a point about how easy these systems are to abuse,
so they're more difficult to stop without violating privacy.
This also opens up the possibility of forged abuse, 
with an attempt to get someone widely blacklisted,
and censorship by remailer operators claiming a user is abusive.

Then, of course, there are people who call for others to be Shunned,
while making nuisances of themselves....

		Bill
# Bill Stewart  NCR Corp, 6870 Koll Center Parkway, Pleasanton CA, 94566
# Voice/Beeper 510-224-7043, Phone 510-484-6204
# email bill.stewart@pleasantonca.ncr.com billstewart@attmail.com
# ViaCrypt PGP Key IDs 384/C2AFCD 1024/9D6465




{% endraw %}
```

## Thread

+ Return to [January 1994](/archive/1994/01)

+ 1994-01-24 (Sun, 23 Jan 94 22:16:35 PST) - Remailer Policies - _wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)_

