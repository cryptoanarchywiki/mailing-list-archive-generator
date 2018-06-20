---
layout: default
---

# 1994-12-17 - Re: properties of FV

## Header Data

From: Nathaniel Borenstein \<nsb@nsb.fv.com\><br>
To: eric@remailer.net<br>
Message Hash: ac42abb39d7844f74ec8f6ef447bcff03eabbe21af27490c03abdafe32d27df5<br>
Message ID: \<Qiwp1730Eyt5E5hexK@nsb.fv.com\><br>
Reply To: \<21153.787690580.1@nsb.fv.com\><br>
UTC Datetime: 1994-12-17 20:57:17 UTC<br>
Raw Date: Sat, 17 Dec 94 12:57:17 PST<br>

## Raw message

```
{% raw  %}From: Nathaniel Borenstein <nsb@nsb.fv.com>
Date: Sat, 17 Dec 94 12:57:17 PST
To: eric@remailer.net
Subject: Re: properties of FV
In-Reply-To: <21153.787690580.1@nsb.fv.com>
Message-ID: <Qiwp1730Eyt5E5hexK@nsb.fv.com>
MIME-Version: 1.0
Content-Type: text/plain


Excerpts from fv: 17-Dec-94 Re: properties of FV eric@remailer.net (2015)

> The argument I see here is like this: "Not very many people have it,
> so we can't use it."  Under this rule, FV shouldn't worry about
> support for smart front ends, because most people don't have them
> already.  FV shouldn't try to deploy mechant software, because most
> people don't have it already.  Now I know that you're not claiming any
> of these ridiculous things, that is, outside of cryptography.

Interesting analogy.  But there's a number of other tradeoffs here.  The
work involved for us in the case of a smart front end is relatively
minimal -- whipping together a safe-tcl-based front end for
metamail-enabled mail tools didn't take me very long at all, actually,
and it makes for very sexy demos, which as you know is important to
marketing types.  (Ever tried giving a sexy demo of cryptography?  It's
sort of like demoing a new kernel.  Ooh, how exciting.)  So while I am
certainly NOT claiming that sexy demos are more important than
cryptographic freedom, it is simply true that there was a far larger
perceived "bang for the buck" in building the sexy front end.  And as
for deploying merchant software, well, that IS clearly more essential
than cryptography -- you simply can't have a commerce mechanism without
sellers!

The work involved in adding optional cryptography is much more than you
might think, particularly because of our internal security architecture.
 Basically, without going into a lot of details, the FV crypto-engine
would have to live on the non-Internet machines that are not in our
direct control, and this would enormously complicate the limited
(batch!) communication we facilitate between the Internet and
non-Internet machines.  Trust me, it isn't trivial by a long shot.  That
doesn't mean we won't do it, but it does affect our priorities.  (It's
interesting that in our case, security gets in the WAY of crypto, given
the non-cryptographic security mechanisms we've already sete up!)

> What I am suggesting is that FV _allow_, not require, the use of
> encryption.  Your main concern with cryptography, it seemed, was theft
> of secret keys.  As you agree, that concern can be disposed of.  Now
> the reason not to use crypto rests on paucity of existing sites which
> use it.  If FV were to _require_ crypto, there would be grounds for
> concern.  Yet neither of us think that a crypto requirement is
> appropriate for the current FV mechanism.

I think we're completely in sync here with regard to everything except
the timing:  we're a small company and we have to choose our priorities
carefully.  The crypto option is one we're very interested in adding
eventually, but at this point it would be a major strain on our
resources.  Moreover, frankly, if we did it, that would only serve to
mix our message in many peoples' perception.  It's hard enough
explaining to reporters that "we've discovered that crypto isn't needed
for commerce."  Their chance of understanding our message would NOT be
enhanced if we then added "but we're providing crypto as an option
anyway."  At this early stage, we have to keep our publicity message as
simple as possible.  (In fact, I think it's already too complicated, so
making it even more complicated is a very hard sell.)

> So why, then, will not FV lead for crypto rather than follow?

Well, mostly because we're leading for commerce, and we can't lead for
everything.  Trying to do too many things at once often causes you not
to succed at any of them.  We do, however, put our money where our mouth
is when we say that we believe in the importance of universal access to
cryptography -- that's why, even as a startup, we are a significant
sponsor of Phil Zimmerman's ongoing work.  (We paid for the development
of a PGP-encrypted telnet, which will be publicly available soon if it
isn't already, and we send monthly checks in support of work related to
the development of PGP 3.0.)

I think I could argue that this makes us more of a "leader for crypto"
than most other companies in the world.  We just don't want our belief
in the importance of privacy, which is real, to become on obstacle to
the success of our business plan, which does not require cryptography,
and which in fact REQUIRES making people realize that crypto is not a
prerequisite for commerce.

> It might be for saving face.  Having argued against crypto so
> publicly, changing positions so rapidly might be seen to look bad.

Heck, no.  I will *enjoy* the day when we add cryptographic support, and
as I hope I've made clear above, I won't regard this as "changing
positions" at all.  To be perfectly clear, our position is that crypto
would be a valuable future enhancement to our system because it will
enhance our users' privacy, not because it will enhance the system's
security.  We think the system is quite sufficiently secure today,
without crypto.  I am sorry if we have alienated some crypto-enthusiasts
with our "crypto is not needed" argument, but this fact is critical to
our business strategy.  It is NOT the same as saying "crypto is bad". 
So if we've been unclear, let me try once more to be crystal clear:

1.  Cryptography is a Good Thing.

2.  Universal access to cryptography is critical to the future of human
freedom.

3.  First Virtual has discovered that cryptography is not NECESSARY for
Internet commerce, and is trying to use that discovery to stimulate real
commerce on the net and to grow our business.

4.  Nearly every technology has positive and negative effects.  If our
discovery sets back the progress of freedom of cryptography, that was
never our intent, and we recognize it as a NEGATIVE effect.  Just
because crypto isn't necessary for commerce doesn't mean it isn't
vitally important to the future of humanity.

5.  As a social responsible corporate citizen of the net, recognizing
the special responsibilities that stem from our invention of crypto-free
commerce, First Virtual is proud to sponsor ongoing PGP development, and
is open to other opportunities (within our still-limited resources) to
help promote the cause of free and universal access to cryptography.

> So, I'm confused.  What _is_ still the problem?

Mostly that there's not enough hours in the day.  (To give you an idea
of how I spend MY time:  In the 36 hour period that ended Saturday
morning, during which I was briefly out of town, I received 760 email
messages.  No kidding.  We're a tad busy these days....)

The bottom line:  First Virtual is not the enemy of cryptography. 
However, our invention is certainly cause for concern for those among us
who thought that commerce would be the "killer app" for making
cryptography universally available.   We believe that on balance our
invention is a very good thing, especially given its democratizing
properties (anyone in the world can be a merchant, unlike standard
credit cards).  We want to work WITH the advocates of crypto to make
sure that cryptography remains avialable for privacy, even though we
have demonstrated that it isn't necessarily a prerequisite for commerce.
 -- Nathaniel




{% endraw %}
```

## Thread

+ Return to [December 1994](/archive/1994/12)

+ 1994-12-17 (Sat, 17 Dec 94 12:57:17 PST) - Re: properties of FV - _Nathaniel Borenstein \<nsb@nsb.fv.com\>_
  + 1994-12-21 (Wed, 21 Dec 94 10:21:01 PST) - [Re: properties of FV](/archive/1994/12/25ad893fe881069700aaf88905153a5d111a5adf341dc6ec1a859d3a77d4ee4f) - _eric@remailer.net (Eric Hughes)_

