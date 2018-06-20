---
layout: default
---

# 1993-10-27 - Re: help writing code

## Header Data

From: "Pat Farrell" \<pfarrell@netcom.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: eff126dcf3bd7e74d1693ec5af4796ddbce8cedd0ae616d76d8232caafed62e8<br>
Message ID: \<45331.pfarrell@netcom.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-10-27 16:37:54 UTC<br>
Raw Date: Wed, 27 Oct 93 09:37:54 PDT<br>

## Raw message

```
{% raw  %}From: "Pat Farrell" <pfarrell@netcom.com>
Date: Wed, 27 Oct 93 09:37:54 PDT
To: cypherpunks@toad.com
Subject: Re: help writing code
Message-ID: <45331.pfarrell@netcom.com>
MIME-Version: 1.0
Content-Type: text/plain


In message Wed, 27 Oct 1993 10:10:04 -0600 (MDT),
  mpjohnso@nyx.cs.du.edu (Michael Johnson)  writes:

> The only way to communicate reliably over the serial port in Windows is
> to upgrade the UART in your serial port to a 16550AFN or equivalent. The
> standard UART (16450 in AT class machines) has no buffer and suffers from
> frequent dropouts due to data overwrite on receive. If you can't do that,
> then an error correcting protocol such as SLIP or PPP is required.

A 16550 is clearly a big help, but Microsoft admits that their
comm.drv fails often when you are using speeds greater than 4800. I have
16550's in my PC. A step in the right direction is TurboComm, a replacement
driver, but that is expensive. A hardware solution is to use an intellegent
serial card, like Hayes ESP or Telcor's T/Port. An O/S solution is to use a
real operating system, :-)  I want a no cost, MS-Windows solution.

But I think folks read too much into my use of "robust"
NUpop works fine as a DOS program without end-to-end.
I simply want that functionality in a Windows program. No more, no less.

I'm aiming low end, the mass market with a 386sx and a 2400 modem. Folks
like me with a network of PCs in their house and even cypherpunks are not
my market. The English majors, history and art majors are the folks I
envision when I see a "user"

Pat

Pat Farrell      Grad Student                 pfarrell@netcom.com
Department of Computer Science    George Mason University, Fairfax, VA
Public key availble via finger          #include <standard.disclaimer>




{% endraw %}
```

## Thread

+ Return to [October 1993](/archive/1993/10)

+ 1993-10-27 (Wed, 27 Oct 93 09:37:54 PDT) - Re: help writing code - _"Pat Farrell" \<pfarrell@netcom.com\>_

