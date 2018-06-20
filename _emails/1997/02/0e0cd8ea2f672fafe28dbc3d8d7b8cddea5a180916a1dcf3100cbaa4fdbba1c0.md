---
layout: default
---

# 1997-02-07 - Re: mail-to-news fun

## Header Data

From: Lance Cottrell \<loki@infonex.com\><br>
To: Bill Stewart \<svmcguir@syr.edu\><br>
Message Hash: 0e0cd8ea2f672fafe28dbc3d8d7b8cddea5a180916a1dcf3100cbaa4fdbba1c0<br>
Message ID: \<199702070441.UAA09115@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-02-07 04:41:11 UTC<br>
Raw Date: Thu, 6 Feb 1997 20:41:11 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: Lance Cottrell <loki@infonex.com>
Date: Thu, 6 Feb 1997 20:41:11 -0800 (PST)
To: Bill Stewart <svmcguir@syr.edu>
Subject: Re: mail-to-news fun
Message-ID: <199702070441.UAA09115@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


It would be a trivial hack for Mixmaster. It allways knows if a message if
going to another remailer, or if this is the last hop, so it can add the
disclaimer only on the last hop.

	-Lance

At 4:06 PM -0800 2/6/97, Bill Stewart wrote:
>At 01:01 PM 2/6/97 -0500, Scott V. McGuire wrote:
>>On Wed, 5 Feb 1997 stewarts@ix.netcom.com wrote:
>>> People don't read mail headers or disclaimers at the bottom,
>>> and putting disclaimers like that into message text for
>>> email exposes the message to traffic analysis.)
>
>>How does putting it in the message expose it to traffic analysis but not
>>putting it in a header?
>
>Suppose you're sending a message on a remailer chain of
>you -> Alice->Bob->Charlie->Dave->Eve->Fred--> target
>and Bob puts lots of disclaimers in his remailer's outgoing messages.
>Anything Bob puts in a header will get stripped out by Charlie,
>so it's no problem.  However, if Bob tacks a disclaimer
>as the bottom text in the outgoing message, when Eve sends
>mail to Fred she'll also see the disclaimer that
>	The message was sent by an anonymous user
>	through the remailer at Bob's Remailer Shack.
>	Bob doesn't know who sent it, and doesn't keep records,
>	so he can't squash the user, but he can block mail to you
>	if you don't want any more anonymous email.
>	Don't believe everything you read!
>so she'll know to check the FBI Illegal Wiretap files for Bob.
>
>Some comments and backtracking
>0) Of course, if you want to avoid traffic analysis,
>sending unencrypted email is pretty stupid, and only the
>next hop is going to see a disclaimer that you append
>after the encrypted part of the message.
>
>1) Prepending the disclaimer to the message body is
>pretty unfriendly to the :: syntax, and not all that
>great for PGP encrypted messages either.  Pretend I
>really just suggested appending it at the end,
>since that's what I would have said if I'd been thinking :-)
>
>On the other hand, I suppose that you can see whether the
>next hop is a Type I remailer by looking for the :: or ##.
>
>2) Cutmarks would be a nice fix, but they require too much
>attention to detail to get right, in case the next hop
>is a remailer.
>
>So maybe you _should_ always put in the disclaimer,
>at the end, with a reminder to always encrypt your
>remailer-chain mail if you want to avoid traffic analysis :-)
>
>
>
>
>
>#			Thanks;  Bill
># Bill Stewart, +1-415-442-2215 stewarts@ix.netcom.com
># You can get PGP outside the US at ftp.ox.ac.uk/pub/crypto/pgp
>#     (If this is a mailing list, please Cc: me on replies.  Thanks.)


----------------------------------------------------------
Lance Cottrell   loki@obscura.com
PGP 2.6 key available by finger or server.
http://www.obscura.com/~loki/

"Love is a snowmobile racing across the tundra.  Suddenly
it flips over, pinning you underneath.  At night the ice
weasels come."
                        --Nietzsche
----------------------------------------------------------







{% endraw %}
```

## Thread

+ Return to [February 1997](/archive/1997/02)

+ 1997-02-07 (Thu, 6 Feb 1997 20:41:11 -0800 (PST)) - Re: mail-to-news fun - _Lance Cottrell \<loki@infonex.com\>_

