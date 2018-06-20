---
layout: default
---

# 1994-08-18 - Re: Remailer ideas (Was: Re: Latency vs. Reordering)

## Header Data

From: wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)<br>
To: cypherpunks@toad.com<br>
Message Hash: 6bcb882b3c118b6d0437c407fa447a8f3bcedaccdab4ae8bb7fbf9b4d812dd27<br>
Message ID: \<9408180100.AA02892@anchor.ho.att.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-08-18 01:02:20 UTC<br>
Raw Date: Wed, 17 Aug 94 18:02:20 PDT<br>

## Raw message

```
{% raw  %}From: wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)
Date: Wed, 17 Aug 94 18:02:20 PDT
To: cypherpunks@toad.com
Subject: Re: Remailer ideas (Was: Re: Latency vs. Reordering)
Message-ID: <9408180100.AA02892@anchor.ho.att.com>
MIME-Version: 1.0
Content-Type: text/plain


> > What I think is a better idea was proposed here last year, and I think
> > someone was doing it for a while.  It is for someone to volunteer to
> > be the keeper of the remailer aliveness information.  He runs scripts
> > every day to ping the remailers, keeps lists of which remailers are
> > currently active, and so on.
>  
> This does seem like a better idea, except for one thing:
> Everybody has got to trust the Keeper of the Aliveness Info. 
> I'm not sure how much of a problem this is, nor am I sure that
> the newsgroup method neccesitates any less trust. 

A major problem with having a single-point aliveness-info source is that
watching traffic to that source gives you some idea who's about to send
anonymous messages - multiple sources mean there are N sources to wiretap
to get the same information, which may be nearly as bad.
On the other hand, a broadcast method like a usenet group has the advantage
that you can read the newsgroup without being very obvious, except locally.
A mailing list is somewhere in between.

Similar problems occur with anonymous single remailers in the absence of 
good reordering; many new remailer users, or users of unreliable remailers
precede their real anonymous messages with a ping of some sort,
such as a message through the remailer chain pointing back to themselves.

If you're using a news reader without NNTP, or with NNTP only for the
local non-tapped LAN, you may be ok.  Another alternative are mailing lists
(NOT human-readable ones like cypherpunks) which reforward the remailer 
newsgroup information, preferably encrypted.

Newsgroups are obviously easy to inject bogus information into, but
that's the way it goes; any non-trusted system is, well, non-trusted....

			Bill
			




{% endraw %}
```

## Thread

+ Return to [August 1994](/archive/1994/08)

+ 1994-08-18 (Wed, 17 Aug 94 18:02:20 PDT) - Re: Remailer ideas (Was: Re: Latency vs. Reordering) - _wcs@anchor.ho.att.com (bill.stewart@pleasantonca.ncr.com +1-510-484-6204)_

