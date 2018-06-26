---
layout: default
---

# 1996-07-20 - Re: Opiated file systems

## Header Data

From: "Chris Adams" \<adamsc<span>@</span>io-online.com\><br>
To: "cypherpunks" \<dfloyd@IO.COM\><br>
Message Hash: 0dc3ece2e6ff6bbefe5cef34897f16dc1e9b458eb088811cdf7c93d7ca5f8ba2<br>
Message ID: \<199607200454.VAA10536@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-07-20 11:29:04 UTC<br>
Raw Date: Sat, 20 Jul 1996 19:29:04 +0800<br>

## Raw message

```
{% raw  %}From: "Chris Adams" <adamsc@io-online.com>
Date: Sat, 20 Jul 1996 19:29:04 +0800
To: "cypherpunks" <dfloyd@IO.COM>
Subject: Re: Opiated file systems
Message-ID: <199607200454.VAA10536@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


On 18 Jul 96 18:49:04 -0800, dfloyd@IO.COM wrote:

>The problem I ran into firsthand with archive sites is that they tend to
>turn into porn or pirated software servers.  One could then have the
>software delete after a download.  Anyway, one is always open to a denial
>of service attack where someone just throws chunks of /dev/random at you.

>If someone has any ideas on how to slow down attacks like this, please
>E-mail me.  It would be nice to have an offsite storage place, but without
>the necessity of giving a bunch of personal info (as with Mcaffee's
>WebStor).

A) Only accept files with valid PGP signatures from accepted keys - this
is one area where PGP's commandline interface is a plus - just write a
batch script. Demand that a separate file be sent first, signed by a
certain key. This file would contain valid filenames for the rest of the
session. If a non-listed file is sent, kill the session.  This could all
be automated with a simple program. You could probably even use SSLs and
similar to do it on a website if you could swill the PGP bit - maybe a
plugin?

B) bounce trash back.

// Chris Adams <adamsc@io-online.com> - Webpages for sale! Se habla JavaScript!
// Automatically receive my resume or PGPKEY by sending email with a subject
// of 'send PGPKEY' or 'send resume'. Capitalization counts so be careful!
 

                                                                                                                                                                                                                                             








{% endraw %}
```

## Thread

+ Return to [July 1996](/archive/1996/07)

+ Return to "["Chris Adams" <adamsc<span>@</span>io-online.com>](/author/chris_adams_adamsc_at_ioonline_com_)"

+ 1996-07-20 (Sat, 20 Jul 1996 19:29:04 +0800) - Re: Opiated file systems - _"Chris Adams" \<adamsc@io-online.com\>_

