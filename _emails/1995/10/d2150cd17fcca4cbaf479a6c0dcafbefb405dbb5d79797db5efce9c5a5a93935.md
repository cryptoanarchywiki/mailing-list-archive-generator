---
layout: default
---

# 1995-10-09 - Re: Rethinking the utility of netnews "cancel" control messages

## Header Data

From: Michael H. Warfield \<mhw<span>@</span>wittsend.com\><br>
To: stu@nemesis.wimsey.com<br>
Message Hash: d2150cd17fcca4cbaf479a6c0dcafbefb405dbb5d79797db5efce9c5a5a93935<br>
Message ID: \<m0t2Jg8-0000rmC@wittsend.com\><br>
Reply To: \<m0t2Ffg-0000VgC@nemesis\><br>
UTC Datetime: 1995-10-09 15:00:15 UTC<br>
Raw Date: Mon, 9 Oct 95 08:00:15 PDT<br>

## Raw message

```
{% raw  %}From: Michael H. Warfield <mhw@wittsend.com>
Date: Mon, 9 Oct 95 08:00:15 PDT
To: stu@nemesis.wimsey.com
Subject: Re: Rethinking the utility of netnews "cancel" control messages
In-Reply-To: <m0t2Ffg-0000VgC@nemesis>
Message-ID: <m0t2Jg8-0000rmC@wittsend.com>
MIME-Version: 1.0
Content-Type: text/plain


Stuart Smith enscribed thusly:
> 
> -----BEGIN PGP SIGNED MESSAGE-----
> 
> In article <v02110105ac99c03922dd@[204.179.132.4]> you write:
> >The downsides of having the mechanism (especially unauthenticated) we see
> >now: official and unofficial squelching of articles that someone doesn't
> >like for whatever arbitrary or situational reason.
> 
> You miss an important point in the mechinism - individual sites *choose*
> whether or not to pay any attention to cancels.  Theoretically, they could
> be configured to only listen to cancels from certain places etc etc.  By all
> means these should be authenticated, but it is vital to remember that this
> is still (for now..) an anarchy.  I don't have to honour anyones cancels,
> and if I do, and you don't like it - you don't have to get a news feed from
> me.

	(No doubt, you are going to get hammered heavily on this from multiple
sides, but here is my shot anyways.)

	Actually you miss a very critical point.  This choice is, in fact,
a "Hobsens Choice", a choice that is no choice.  If any site between you
and the article source choses to honor that cancel, you never get the
original article to begin with.  All you get is the cancel message and your
choice to honor it or not is totally meaningless.  To be worth anything
all of the intermediate nodes would have to chose to ignore cancel messages
and then the leaf nodes would have the privledge of honoring or ignoring
them.  But it will be a VERY cold day in a VERY warm place before that ever
happens, even if it did make sense (It doesn't).

	Yes yes, I know - article loss is contigent upon the cancel arriving
there before you pick up the article from them, this effect would just serve
to add a level of chaos and indetermanancy to the mechanism.  Obviously 
(because of time elements involved in realization and forging of cancels)
it is much more likely that you will receive originals for article where a
forged cancel is received.  That depends on the latency involving all of
the news feeds between you and the article source and the latency involving
the forger and his ability to recognize a message he wants to cancel and
to get that cancel out.  The human factor adds a lot here.  Perhaps we
should add a "time-limit" to cancel messages?  This too would be highly
indeterminant as propagation times stretched out.

	End result is that most sites currently do honor cancels, so many
of the originals never reach a lot of the leaf nodes while all of us
continue to be subjected to a FLOOD of cancel control messages.  In terms
of message count and article numbers (not total bytes of storage) my control
group is the largest newsgroup group on my system!

	Regards,
	Mike
-- 
 Michael H. Warfield    |  (770) 985-6132   |  mhw@WittsEnd.com
  (The Mad Wizard)      |  (770) 925-8248   |  http://www.wittsend.com/mhw/
  NIC whois:  MHW9      |  An optimist believes we live in the best of all
 PGP Key: 0xDF1DD471    |  possible worlds.  A pessimist is sure of it!



{% endraw %}
```

## Thread

+ Return to [October 1995](/archive/1995/10)

+ Return to "[bogstad<span>@</span>news.cs.jhu.edu (Bill Bogstad)](/authors/bogstad_at_news_cs_jhu_edu_bill_bogstad_)"
+ Return to "[Bryce <wilcoxb<span>@</span>nagina.cs.colorado.edu>](/authors/bryce_wilcoxb_at_nagina_cs_colorado_edu_)"
+ Return to "["Erik E. Fair"  (Time Keeper) <fair<span>@</span>clock.org>](/authors/erik_e_fair_time_keeper_fair_at_clock_org_)"
+ Return to "[Michael H. Warfield <mhw<span>@</span>wittsend.com>](/authors/michael_h_warfield_mhw_at_wittsend_com_)"
+ Return to "[stu<span>@</span>nemesis (Stuart Smith)](/authors/stu_at_nemesis_stuart_smith_)"

+ 1995-10-05 (Thu, 5 Oct 95 10:19:05 PDT) - [Re: Rethinking the utility of netnews "cancel" control messages](/archive/1995/10/b7fdd4e3d2456f5d93c05be67efde0654e0ba78c4cf304cc58322077eef91b8c) - _"Erik E. Fair"  (Time Keeper) \<fair@clock.org\>_
  + 1995-10-05 (Thu, 5 Oct 95 12:42:50 PDT) - [Re: Rethinking the utility of netnews "cancel" control messages](/archive/1995/10/1c88940aef0d082cf991766cc67966a28dae361ac27836d823ed9bc8db431ef8) - _Bryce \<wilcoxb@nagina.cs.colorado.edu\>_
  + 1995-10-08 (Sun, 8 Oct 95 09:00:25 PDT) - [Re: Rethinking the utility of netnews "cancel" control messages](/archive/1995/10/b221ffd7da9b52d65096b5f610b14e4481e8548030565c4fc77068832184a032) - _bogstad@news.cs.jhu.edu (Bill Bogstad)_
  + 1995-10-09 (Mon, 9 Oct 95 04:22:24 PDT) - [Re: Rethinking the utility of netnews "cancel" control messages](/archive/1995/10/32600a0595ebb6f43999c12ecfc5086602c228dacc732660c18e1efb15a9685f) - _stu@nemesis (Stuart Smith)_
    + 1995-10-09 (Mon, 9 Oct 95 08:00:15 PDT) - Re: Rethinking the utility of netnews "cancel" control messages - _Michael H. Warfield \<mhw@wittsend.com\>_

