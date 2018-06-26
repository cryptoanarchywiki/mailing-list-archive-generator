---
layout: default
---

# 1997-11-16 - Re: trusting untrusted platforms

## Header Data

From: Ryan Lackey \<rdl<span>@</span>mit.edu\><br>
To: cypherpunks@cyberpass.net<br>
Message Hash: 9d0572f1bafa6a4a00dfefc6be0c7d902a63b7ac9c4cdb0227d2f773ca8bd5ba<br>
Message ID: \<199711161443.JAA01554@tana.mit.edu\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-11-16 14:48:12 UTC<br>
Raw Date: Sun, 16 Nov 1997 22:48:12 +0800<br>

## Raw message

```
{% raw  %}From: Ryan Lackey <rdl@mit.edu>
Date: Sun, 16 Nov 1997 22:48:12 +0800
To: cypherpunks@cyberpass.net
Subject: Re: trusting untrusted platforms
Message-ID: <199711161443.JAA01554@tana.mit.edu>
MIME-Version: 1.0
Content-Type: text/plain



> > Alexandre Maret <amaret@infomaniak.ch> says:

> > [how to do trusted computation on untrusted platforms]

I'm working on a paper, it's one of the technical hurdles on the way
to my Eternity DDS eternity service implementation.

> rdl, less frustrated with changing from vtwm/athena to KDE, says:

> I so far have been approaching it as "Type I (active)" and "Type II (passive)"
> attackers.  In the first case, people lie about the results, in the second,
> they give you the correct results, but snoop on the data. (For some reason
> the terminology is kind of lame, but it helps to have some)
> 
> There are a bunch of mathematical/cryptographic ways of hiding data from
> those doing computations on it, at least for a subset of computations.  I'm
> trying to put together a generalized computing model for this which would be
> turing complete if it can be, although it is not clear it can be.  Some
> operations practically will be a lot more expensive in this model than in
> the conventional environment, and perhaps to a computation which would require
> 10 units of conventional secret CPU time, you will need 9 units of secret
> CPU to encode/decode the data and 41 units of public CPU time.  You also need
> to guard against covert channels, such as the total amount of public CPU time
> you are requesting as a clue to what you're doing with it.  I am confident
> type II security can be realized with at least a minor amount of performance
> improvement over purely secret use, assuming public time is free.
> 
> Type I security is a lot more difficult to realize in true theoretical
> sense, but is easier in a practical sense.  A simple solution is to do the
> same computation on a bunch of different remote machines, and as long as
> they don't collude, you can just make sure they all answered the same, modulo
> rounding errors and stuff.  This isn't the kind of provable security you
> can conceivably get against type II attackers, but it doesn't have any innate
> performance hit.
> 
> It's possible there are systems which are byzantine fault tolerant to
> the former kind of attack -- instinctively, you can just split up the
> computation in small enough pieces that you don't care if it is compromised.
> 
> I'm interested in finding a provably secure computation-checksum technique.
> I think there are most likely reductions for a lot of problems to things
> which can be verified, and again, my goal is to have a Turing-complete
> model of computation with this property.
> 
> > [can cryptography be helpful?]
> 
> It's as much a theory of computation problem as anything else, once you
> have some functions through which you can carry some operations.  
> 
> Most of the stuff I've done so far focuses on the graph coloring problem.
> I'm probably going to finish a quick version which can only deal with
> a subset of problems, then work on a general model.

> > [paper availability issues]

> Yes, it will be publically available.  It will be available when it's closer
> to done; I will send something to cypherpunks about it, and I'll put it
> up on the web somewhere.  If it doesn't suck, and I can convince someone
> at LCS-CIS of this/to be a co-author/etc., I might try to get it published.

Anyone know anything very relevant to this?  I've mostly just started on
the research (my current exciting project has been Linux Fibre Channel and
making a bloody fast, yet maybe secure, yet small cipher for an on board
processor), and pointers would be useful.  It isn't as hard a problem as
I first thought, though.  This seems like the kind of thing everyone's favorite
judge-threatening tree-hugger-nose-mac-10-inserting gun-hoarding
old-man-on-the-mountain would have done N years ago :) [flames, fan.  
gasoline. rdx...] so I'd rather not reinvent the wheel more than once or twice.

Ryan (getting dangerously close to having a working Eternity DDS demo,
and wondering if FC98 will be on mbone, particularly the solar eclipse, since
even if he had the money to go, it's in the middle of next semester, and 
disappearing for a week would kind of be difficult, although not at all
impossible of someone wants to pay for me to go...ahh, but there's always
next year) 
-- 
Ryan Lackey
rdl@mit.edu
http://mit.edu/rdl/		






{% endraw %}
```

## Thread

+ Return to [November 1997](/archive/1997/11)

+ Return to "[Robert Hettinga <rah<span>@</span>shipwright.com>](/author/robert_hettinga_rah_at_shipwright_com_)"
+ Return to "[Ryan Lackey <rdl<span>@</span>mit.edu>](/author/ryan_lackey_rdl_at_mit_edu_)"

+ 1997-11-16 (Sun, 16 Nov 1997 22:48:12 +0800) - Re: trusting untrusted platforms - _Ryan Lackey \<rdl@mit.edu\>_
  + 1997-11-18 (Tue, 18 Nov 1997 08:42:39 +0800) - [Re: trusting untrusted platforms](/archive/1997/11/08e470d77f22ff3c7363e4d7522d78cd69f6f4b7b1fd9dd2a46de9293cbf2e20) - _Robert Hettinga \<rah@shipwright.com\>_

