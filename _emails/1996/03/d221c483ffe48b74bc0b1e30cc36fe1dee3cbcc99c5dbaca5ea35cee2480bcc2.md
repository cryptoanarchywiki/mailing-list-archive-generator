---
layout: default
---

# 1996-03-14 - Re: entropy masking (was Re: Multiple spinners as sources of entropy?)

## Header Data

From: JonWienke<span>@</span>aol.com<br>
To: cypherpunks@toad.com<br>
Message Hash: d221c483ffe48b74bc0b1e30cc36fe1dee3cbcc99c5dbaca5ea35cee2480bcc2<br>
Message ID: \<960313234757_350663563@emout09.mail.aol.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-03-14 18:36:52 UTC<br>
Raw Date: Thu, 14 Mar 1996 13:36:52 -0500<br>

## Raw message

```
{% raw  %}From: JonWienke@aol.com
Date: Thu, 14 Mar 1996 13:36:52 -0500
To: cypherpunks@toad.com
Subject: Re: entropy masking (was Re: Multiple spinners as sources of entropy?)
Message-ID: <960313234757_350663563@emout09.mail.aol.com>
MIME-Version: 1.0
Content-Type: text/plain


In a message dated 96-03-13 18:35:51 EST, Matt Blaze writes:

>I would go even further than this.  I wouldn't trust ANY
>environmentally-based random source (cycle spinner, keyboard
>timer, disk noise, whatever) against adversaries on the
>same system.

In DOS, the keyboard, mouse, and disk drives run on interrupts, not timers.
 If you use a timer as a spinner, such as the Windows GetCurrentTime()
function, (I MSec. resolution) and check its value each time a key is pressed
and released, It would appear that the results should be quite random,
because the keystroke is not processed in conjunction with the timer, but
rather whenever the interrupt occurs.  My tests in this area indicate that
any 8 bit value can be achieved with this method, with a fairly uniform
distribution.  My tests are not thorough (I haven't sat down and typed for 2
hours to test the distribution of the output), but results look reasonably
good so far.

Jonathan Wienke




{% endraw %}
```

## Thread

+ Return to [March 1996](/archive/1996/03)

+ Return to "[blane<span>@</span>aa.net (Brian C. Lane)](/authors/blane_at_aa_net_brian_c_lane_)"
+ Return to "[JonWienke<span>@</span>aol.com](/authors/jonwienke_at_aol_com)"

+ 1996-03-14 (Thu, 14 Mar 1996 13:36:52 -0500) - Re: entropy masking (was Re: Multiple spinners as sources of entropy?) - _JonWienke@aol.com_
  + 1996-03-19 (Wed, 20 Mar 1996 01:30:01 +0800) - [Re: entropy masking (was Re: Multiple spinners as sources of entropy?)](/archive/1996/03/f6f660c778d6c0dfcca21e067dec0a0043f7e61d80ff66472b8b1c95e6419adc) - _blane@aa.net (Brian C. Lane)_

