---
layout: default
---

# 1997-10-27 - Re: cryptographic anecdotes -- GPS and

## Header Data

From: Martin Pool \<mbp<span>@</span>pharos.com.au\><br>
To: Julian Assange \<proff@iq.org\><br>
Message Hash: 9c1fac12bdbe0f1cfbec046ac3adb33a1bf0fa5e538e345ccb377ba5abdc6e22<br>
Message ID: \<Pine.LNX.3.95.971027160901.7921B-100000@buffalo.pharos.com.au\><br>
Reply To: \<19971027010829.851.qmail@iq.org\><br>
UTC Datetime: 1997-10-27 08:00:48 UTC<br>
Raw Date: Mon, 27 Oct 1997 16:00:48 +0800<br>

## Raw message

```
{% raw  %}From: Martin Pool <mbp@pharos.com.au>
Date: Mon, 27 Oct 1997 16:00:48 +0800
To: Julian Assange <proff@iq.org>
Subject: Re: cryptographic anecdotes -- GPS and
In-Reply-To: <19971027010829.851.qmail@iq.org>
Message-ID: <Pine.LNX.3.95.971027160901.7921B-100000@buffalo.pharos.com.au>
MIME-Version: 1.0
Content-Type: text/plain



On 27 Oct 1997, Julian Assange wrote:

> I'm involved in producing a segment on cryptograpic issues for Radio
> National (ABC) to be aired latter this week. I have no problems with
> the technical issues but could use some (reliable) "colour" i.e small
> quirky or unusual anecdotes that will draw in and hold the larger
> order of listeners who don't otherwise have any cryptography/
> cryptographic-policy background.

Do you know the timeslot yet?

"Java Network Services" (I forget the exact title) from Prentice Hall has
a case study about interfacing Java to GPS hardware.  The introduction to
the chapter provides some very interesting information about GPS which,
like crypto, is a "dual use technology".  It's not exactly the same, of
course -- GPS is about people getting information that the state would
like to keep secret, not vice versa -- but it's still interesting.
("Location escrow" is a nice phrase.)

If the book is correct, then the system was originally designed to
introduce errors into the part of the time signal decypherable by civilian
users that would produce positional uncertainty of about 100m.  The
complete signal, available (in theory) only to US or US-sponsored forces,
allowed positions to be calculated to within an accuracy of about 1m.

However, hackers being what they are ;-), somebody realized that since the
same errors were observed by all receivers, one could compensate for them
to some extent.  

Specifically, one has a base station somewhere whose location you know
very accurately by other means.  This station continuously subtracts it's
known position from the position calculated by it's civilian GPS hardware,
and broadcasts the difference over the pager network or some other public
medium.  (The math is not quite that simple, I imagine, but conceptually
that's what you do.)  Combining this information with the satellite signals
allows civilian GPS hardware to improve it's accuracy by an order of
magnitude to about 10m of uncertainty, which could make all the difference
in, say, a search-and-rescue situation.  This technique is called,
obviously enough, "differential GPS". 

Even more interesting is that the DOT is apparently negotiating with the
DOD to make full GPS publicly available, presumably because it would sell
more cars.  (Just what the world needs...)  Quite possibly there will be
export restrictions, of course.  The similarities to commerce vs TLA
concerns in encryption are obvious.  I don't know the outcome of the
negotiations, but I got the impression it was more likely than not. 

The book was not immensely technical, so some (or all) details may be
wrong.

Assuming you're talking about Australian RN, then comparisons to the
recent gun buy-back scheme might be interesting, on the topic of
balance-of-power between the people and the state.  (Hmm, wish I could
post "Blue Murder", a documovie about NSW police corruption in the 80s to
the list.) 

--
Martin Pool





{% endraw %}
```

## Thread

+ Return to [October 1997](/archive/1997/10)

+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/author/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "[bureau42 Anonymous Remailer <nobody<span>@</span>bureau42.ml.org>](/author/bureau42_anonymous_remailer_nobody_at_bureau42_ml_org_)"
+ Return to "[Julian Assange <proff<span>@</span>iq.org>](/author/julian_assange_proff_at_iq_org_)"
+ Return to "[Martin Pool <mbp<span>@</span>pharos.com.au>](/author/martin_pool_mbp_at_pharos_com_au_)"
+ Return to "[nobody<span>@</span>REPLAY.COM (Anonymous)](/author/nobody_at_replay_com_anonymous_)"

+ 1997-10-27 (Mon, 27 Oct 1997 09:19:33 +0800) - [cryptographic anecdotes](/archive/1997/10/fba61a105d97f4e6bc3d0eee5f255113156113b77080a14062618c796aef4fe7) - _Julian Assange \<proff@iq.org\>_
  + 1997-10-27 (Mon, 27 Oct 1997 15:01:27 +0800) - [Re: cryptographic anecdotes](/archive/1997/10/2140542e4330d262153d026a57c9b522fae66868137f12d68e688960121d7661) - _nobody@REPLAY.COM (Anonymous)_
    + 1997-10-27 (Tue, 28 Oct 1997 00:20:31 +0800) - [No Subject](/archive/1997/10/271fd20858ad1ff40483e4535899b2a7ec449d56e4559e61ab721bdbb4bce935) - _bureau42 Anonymous Remailer \<nobody@bureau42.ml.org\>_
  + 1997-10-27 (Mon, 27 Oct 1997 16:00:48 +0800) - Re: cryptographic anecdotes -- GPS and - _Martin Pool \<mbp@pharos.com.au\>_
  + 1997-10-29 (Wed, 29 Oct 1997 15:10:00 +0800) - [Re: cryptographic anecdotes](/archive/1997/10/3e09a0b82e0031752f3d59e85598f07b3bb86f77886d1d22caef447322ce91be) - _Bill Stewart \<stewarts@ix.netcom.com\>_

