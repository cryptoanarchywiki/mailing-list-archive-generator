---
layout: default
---

# 1996-07-30 - game theory

## Header Data

From: Wei Dai \<weidai<span>@</span>eskimo.com\><br>
To: Cypherpunks \<cypherpunks@toad.com\><br>
Message Hash: 38ecd640fefd9663ab1bf818f7bd99b2abaa2f2fa7d2f3b14be1fafb4e2845b4<br>
Message ID: \<Pine.SUN.3.95.960729183503.27103A-100000@eskimo.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-07-30 04:37:52 UTC<br>
Raw Date: Tue, 30 Jul 1996 12:37:52 +0800<br>

## Raw message

```
{% raw  %}From: Wei Dai <weidai@eskimo.com>
Date: Tue, 30 Jul 1996 12:37:52 +0800
To: Cypherpunks <cypherpunks@toad.com>
Subject: game theory
Message-ID: <Pine.SUN.3.95.960729183503.27103A-100000@eskimo.com>
MIME-Version: 1.0
Content-Type: text/plain


I agree with Tim that game theory is very interesting and a potentialy
useful tool in cryptography.  However, game theory currently has a major
limitation.  An even moderately complex game is likely to have a
very large set of equilibria (possible solutions where none of the players
will deviate from their strategy if they knew the strategy of all other
players).  It takes a lot of work to calculate the equilibria set, and
even if this is done, game theorists are hard pressed to explain or
predict which equilibrium is the actual outcome.

I have not read any of Schelling's work, but the notion of Schelling
points seems to be closely connected to that of equilibria in game theory.
If this is the case, then I don't see how it can be usefully applied to
the complex interactions of an entire society.  It is easy to say that
current social conventions are an equilibrium in some game, but how much
is this worth?  What we would like to know is what is the entire set of
possible equilibria, why we are in one of them (instead of the others),
and how changes in the game (such as introduction of strong crypto) change
that set.  I find it unlikely that game theory will soon advance to such a
state that it will give us the answers to these questions.

Wei Dai

P.S.  Now that I've reread Tim's original messages, I realize that maybe
Schelling points are not really the equilibria of game theory.  If this is
the case, Tim, can you please clarify its actual meaning?  (Perhaps by
quoting a definition from Schelling's book?)

ObCrypto: Here is a simple cryptographic application of game theory.  A
fair exchange protocol allows two parties to reveal valuable secrets to
each other one bit at a time.  Modeled as a game, it goes like this:

There are N (an even number) rounds.  On odd rounds Alice decides whether
to reveal a bit to Bob or to stop the game.  On even rounds Bob decides
whether to reveal a bit to Alice or to stop the game.  The goal is to get
as many bits as possible and secondarily to reveal as few bits as
possible.

Now using backwards inductions, we can show that the only subgame perfect
equilibrium of this game is that Alice stops the game in round 1.  The
analysis goes like this: on the last round (if the game goes that far) Bob
will have gotten all of the bits from Alice, so it makes no sense for him
to reveal his last bit to Alice.  On the next to last round, Alice knows
that even if she reveals her bit, she cannot get Bob's last bit, therefore
she would stop on that round.  Therefore Bob would stop on round N-2, and
on it goes.

Wei Dai





{% endraw %}
```

## Thread

+ Return to [July 1996](/archive/1996/07)

+ Return to "[Wei Dai <weidai<span>@</span>eskimo.com>](/authors/wei_dai_weidai_at_eskimo_com_)"

+ 1996-07-30 (Tue, 30 Jul 1996 12:37:52 +0800) - game theory - _Wei Dai \<weidai@eskimo.com\>_

