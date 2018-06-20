---
layout: default
---

# 1994-01-27 - remailer multiple paths?

## Header Data

From: "Mark W. Eichin" \<eichin@paycheck.cygnus.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: 48e5e8eecd96e89b88a4bbff6e13fc5912c0dba8d1e26cbfeaeb1ba0c597c7fe<br>
Message ID: \<9401271557.AA08940@paycheck.cygnus.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-01-27 17:02:12 UTC<br>
Raw Date: Thu, 27 Jan 94 09:02:12 PST<br>

## Raw message

```
{% raw  %}From: "Mark W. Eichin" <eichin@paycheck.cygnus.com>
Date: Thu, 27 Jan 94 09:02:12 PST
To: cypherpunks@toad.com
Subject: remailer multiple paths?
Message-ID: <9401271557.AA08940@paycheck.cygnus.com>
MIME-Version: 1.0
Content-Type: text/plain



Is there any value to the idea of breaking up a message and sending
the parts of it by different "remailer paths" to the ultimate
recipient? Shouldn't this reduce the risk of remailer compromise as
much or more than simply nesting remailers?

You'd need a good way of breaking up the message; if you were
encrypting already, it'd probably do well enough to put byte x into
message (x mod n) where you're sending n messages. (You could even
slice it at the bit level, but that's a little harder to do in a
trivial script...) 

Or would you? is breaking up the message at all good enough, or is it
necessary that "nothing of value" can be produced from the pieces?

Haven't thought this through, but perhaps others here have. (The
concept could even be used with an anonymous pool, sort of a "collect
the whole set!" type of reading mechanism...)

It could be argued that the various binary.pictures groups are already
run this way :-)

				_Mark_ <eichin@paycheck.cygnus.com>
				... just me at home ...





{% endraw %}
```

## Thread

+ Return to [January 1994](/archive/1994/01)

+ 1994-01-27 (Thu, 27 Jan 94 09:02:12 PST) - remailer multiple paths? - _"Mark W. Eichin" \<eichin@paycheck.cygnus.com\>_
  + 1994-01-27 (Thu, 27 Jan 94 12:37:42 PST) - [Re: remailer multiple paths?](/archive/1994/01/41acc51b0676c714f7032d59f67ed9107933bf201504806fd3c5b4c0549c7dae) - _Eli Brandt \<ebrandt@jarthur.Claremont.EDU\>_

