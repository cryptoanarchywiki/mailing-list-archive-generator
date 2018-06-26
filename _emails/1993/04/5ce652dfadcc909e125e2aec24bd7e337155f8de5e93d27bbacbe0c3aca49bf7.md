---
layout: default
---

# 1993-04-28 - MYK-78

## Header Data

From: Eric Hughes \<hughes<span>@</span>soda.berkeley.edu\><br>
To: cypherpunks@toad.com<br>
Message Hash: 5ce652dfadcc909e125e2aec24bd7e337155f8de5e93d27bbacbe0c3aca49bf7<br>
Message ID: \<9304281705.AA23767@soda.berkeley.edu\><br>
Reply To: \<199304280536.AA09155@well.sf.ca.us\><br>
UTC Datetime: 1993-04-28 17:09:14 UTC<br>
Raw Date: Wed, 28 Apr 93 10:09:14 PDT<br>

## Raw message

```
{% raw  %}From: Eric Hughes <hughes@soda.berkeley.edu>
Date: Wed, 28 Apr 93 10:09:14 PDT
To: cypherpunks@toad.com
Subject: MYK-78
In-Reply-To: <199304280536.AA09155@well.sf.ca.us>
Message-ID: <9304281705.AA23767@soda.berkeley.edu>
MIME-Version: 1.0
Content-Type: text/plain


Arthur sez:
>I've been stalking Mykotronx with phone and smail 

And I've been peering over his shoulder for much of that time.  I'd
like to comment on some of the unapproved ways to use this chip.

The way that the chip enforces the wiretap protocol is by not working
as a pair unless the LEEF's are transferred from one chip to another.
Since these LEEF's are presumed to go out in the clear, tapping is
reasonably assured.

>LEEF = Law Enforcement Exploitation Field.  

I really am astounded at the names these people use.  It does give
rise to a great new slogan, though:

	"Stop Government Exploitation Fields!"

Now suppose that there was a law requiring use of this chip.  One
could still create an untappable system just by not sending the LEEF's
in the clear.  So, for example, you do a D-H key exchange with a 600
bit modulus.  Then the originating chip transmits the CV, LEEF's, etc.
(as I count 282 bits), XORing with the D-H key, i.e. using a one-time
pad.  Now the LEEF's have been transferred, but not revealed to any
eavesdropper.  With a 600 bit modulus in the key exchange you could
transmit one set of keying material each way.

There's a great hack here to be had.  These AT&T secure phones with
the wiretap chip inside have internal modems and run some coordination
protocol to synchronize.  Almost certainly such an initial protocol
must have retry paths in its state machine; otherwise the reliability
would suffer.  So we could make a compatible phone that initially
tried to determine if another such phone was on the other end; if so,
proceed with the blinded LEEF transmission.  If not, drop back and try
the wiretap protocol.

In fact, those of you who have seen Shimomura's and Lottor's work with
hacked cellular phones know that it might be possible to put this
hacked protocol right in the AT&T phone itself!  If the phone has a
ROM of some type which contains the microcontroller code, it could be
reverse engineered and reprogrammed.  

If I were mandated to use the chip in a commercial product, I'd put
three buttons on the phone:
	CLEAR (icon=open doors)
	SECURE (icon=closed doors)
	TELL THE GOVERNMENT (icon=benevolent face) 
Pressing the third button would use the AT&T protocol, pressing the
second would encrypt the LEEF's.

"AT&T: Helping the government to reach in and touch you."

There might be another technique.  There is a Write CV command that is
accepted in normal operation.  (Some CV must be put in during
initialization after reset to reach the idle state, i.e. the normal
operating state.)  This command requires the check word, but that's
easily generated in the normal manner.  It is possible that changing
the CV requires generating another set of LEEF's; that's not clear to
me, but Arthur thinks you can.  If, however, one can just change the
CV at will, one could send the LEEF's in the clear and then
immediately change the CV (session key).  Now the LEEF has been sent
but the conversation makes no sense.  My money is that this is
interlocked with IV generation, though.

Eric




{% endraw %}
```

## Thread

+ Return to [April 1993](/archive/1993/04)

+ Return to "[Arthur Abraham <a2<span>@</span>well.sf.ca.us>](/author/arthur_abraham_a2_at_well_sf_ca_us_)"
+ Return to "[Eric Hughes <hughes<span>@</span>soda.berkeley.edu>](/author/eric_hughes_hughes_at_soda_berkeley_edu_)"

+ 1993-04-28 (Tue, 27 Apr 93 22:36:15 PDT) - [MYK-78](/archive/1993/04/774f1f1c7f221e817a5828fa3278e59f8682d202387b0ed799cf4a11e4c3f442) - _Arthur Abraham \<a2@well.sf.ca.us\>_
  + 1993-04-28 (Wed, 28 Apr 93 10:09:14 PDT) - MYK-78 - _Eric Hughes \<hughes@soda.berkeley.edu\>_

