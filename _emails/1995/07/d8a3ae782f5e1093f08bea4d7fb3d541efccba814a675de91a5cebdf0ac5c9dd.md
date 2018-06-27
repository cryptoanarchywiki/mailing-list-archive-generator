---
layout: default
---

# 1995-07-26 - Re: Netscape the Big Win

## Header Data

From: paul<span>@</span>poboy.b17c.ingr.com (Paul Robichaux)<br>
To: hfinney@shell.portal.com (Hal)<br>
Message Hash: d8a3ae782f5e1093f08bea4d7fb3d541efccba814a675de91a5cebdf0ac5c9dd<br>
Message ID: \<199507261447.AA17788@poboy.b17c.ingr.com\><br>
Reply To: \<199507211727.KAA06527@jobe.shell.portal.com\><br>
UTC Datetime: 1995-07-26 14:53:18 UTC<br>
Raw Date: Wed, 26 Jul 95 07:53:18 PDT<br>

## Raw message

```
{% raw  %}From: paul@poboy.b17c.ingr.com (Paul Robichaux)
Date: Wed, 26 Jul 95 07:53:18 PDT
To: hfinney@shell.portal.com (Hal)
Subject: Re: Netscape the Big Win
In-Reply-To: <199507211727.KAA06527@jobe.shell.portal.com>
Message-ID: <199507261447.AA17788@poboy.b17c.ingr.com>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

Hal said:
> This sounds very good if it already is almost working.  The TCP
> connection which is opened would have to be to a server on the local
> machine, so it would be important that the software support that.  Also,
> the local SOCKS relay would of course not want its winsock calls to be
> intercepted and translated in this way, so there would need to be some
> alternative way to access "vanilla" winsock.  Can you give any
> more information on the NEC work?

This should be fairly straightforward: take the existing winsock.dll
or winsock32.dll and rename it. Install the NEC DLL with the old
winsock's name, then have the NEC DLL do a LoadLibrary() to attach the
original version.

> I have written a simple dummy relay for winsock and it requires a pretty
> different programming style than for Unix.  Netscape has a habit of
> firing off a bunch of requests at once, so it has to be extremely
> asynchronous.  For Windows this means you get a windows message every
> time a packet arrives and use non-blocking I/O.  In Unix this is usually
> handled by forking a new process to handle each independent connection.
> Non-blocking I/O can be used in Unix but I don't think there is a
> non-blocking connect as there is in Windows.  Maybe Windows 95 will allow
> a more Unix-style communication model, though.  Should the proxy require
> Windows 95, or will Windows 3 still be in widespread use for another
> year or two?

Asynchronous requests are the best way to implement I/O under Windows
(3.1, '95, and NT.) Any app that's threaded (Free Agent and Netscape
come to mind) will benefit, as will any user who's using a
multiprocessor machine.

If you're willing to assume the existence of Win95 or WinNT, you can
always spawn a new thread for each connection.

- -Paul

- -- 
Paul Robichaux, KD4JZG       | Do you support free speech? Even when
perobich@ingr.com            | you don't like what's being said?
		 Be a cryptography user. Ask me how.


-----BEGIN PGP SIGNATURE-----
Version: 2.6.2

iQCVAwUBMBZVcafb4pLe9tolAQHrHwQAhBAtIAZnaL2gh1BhZeE6WWQ1UQK7ffB2
XRZReUNzAVpCyvllKPDiN5TgUSuit8XeB4BzHOStXkNMJGlLE0vqTr5j5y2S0Fzo
nisi5Ve5+8XWJ8wFrshldfFcLyFuOK3LeL9cAKXQQrQ2GdxluusqBzqYHFM8koPP
zWI2YiF0VHM=
=yzFt
-----END PGP SIGNATURE-----




{% endraw %}
```

## Thread

+ Return to [July 1995](/archive/1995/07)

+ Return to "[Enzo Michelangeli <enzo<span>@</span>ima.com>](/authors/enzo_michelangeli_enzo_at_ima_com_)"
+ Return to "[Enzo Michelangeli <enzo<span>@</span>ima.net>](/authors/enzo_michelangeli_enzo_at_ima_net_)"
+ Return to "[Hal <hfinney<span>@</span>shell.portal.com>](/authors/hal_hfinney_at_shell_portal_com_)"
+ Return to "[paul<span>@</span>poboy.b17c.ingr.com (Paul Robichaux)](/authors/paul_at_poboy_b17c_ingr_com_paul_robichaux_)"

+ 1995-07-21 (Fri, 21 Jul 95 10:28:50 PDT) - [Re: Netscape the Big Win](/archive/1995/07/1a07a9e7a6bd48514e6b364c1dbc1f9cab1aad9e82a78059adf6664fa1fefe9d) - _Hal \<hfinney@shell.portal.com\>_
  + 1995-07-22 (Sat, 22 Jul 95 04:47:59 PDT) - [Re: Netscape the Big Win](/archive/1995/07/c4a1cc0902134dafdd7b202b92049b5b9d71624ec8b1c2efcc2522bf1f72f728) - _Enzo Michelangeli \<enzo@ima.net\>_
  + 1995-07-26 (Wed, 26 Jul 95 07:53:18 PDT) - Re: Netscape the Big Win - _paul@poboy.b17c.ingr.com (Paul Robichaux)_
    + 1995-07-27 (Wed, 26 Jul 95 22:17:48 PDT) - [Re: Netscape the Big Win](/archive/1995/07/ed870b6e438988bfbb2504d937a79123cc1481c8df8f2e22a92c3bebf67e1794) - _Enzo Michelangeli \<enzo@ima.com\>_

