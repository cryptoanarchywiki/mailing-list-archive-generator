---
layout: default
---

# 1996-04-13 - Re: Protocols at the Point of a Gun

## Header Data

From: Rich Graves \<llurch<span>@</span>networking.stanford.edu\><br>
To: "Richard K. Moore" \<rkmoore@iol.ie\><br>
Message Hash: e86c2aafacbb488a1e9fe2961afcbe7b14d14c1e2a0bf19bcf3cab108196d5a1<br>
Message ID: \<Pine.ULT.3.92.960412234329.2525A-100000@Networking.Stanford.EDU\><br>
Reply To: \<v02110134ad945a3a8bff@[194.125.43.36]\><br>
UTC Datetime: 1996-04-13 12:12:00 UTC<br>
Raw Date: Sat, 13 Apr 1996 20:12:00 +0800<br>

## Raw message

```
{% raw  %}From: Rich Graves <llurch@networking.stanford.edu>
Date: Sat, 13 Apr 1996 20:12:00 +0800
To: "Richard K. Moore" <rkmoore@iol.ie>
Subject: Re: Protocols at the Point of a Gun
In-Reply-To: <v02110134ad945a3a8bff@[194.125.43.36]>
Message-ID: <Pine.ULT.3.92.960412234329.2525A-100000@Networking.Stanford.EDU>
MIME-Version: 1.0
Content-Type: text/plain


On Fri, 12 Apr 1996, Richard K. Moore wrote:

> 4/11/96, Bill Stewart wrote:
> >There are serious technical problems with the suggestion that labelling
> >packets as "Adult" or "Child" using IP options and filtering at ISPs
> >for censorship.
>
>         IMHO, the technical problems can somehow be solved, whether we like
> it or not, although it will probably be botched intentionally or otherwise.
> It's tougher than most protocol upgrades, but easier than was designing
> X.400 (just to give some GROSS bounds to the problem).

Hello? We're talking packets, not sessions. Trying to do this at the
network layer (or lower) is so monstrously wrong that it's not worth
talking about. It's impossible by design. In a properly designed system,
the application should have no way to tell the protocol stack to flip
special bits. What about encapsulation? Fragmentation? LAN emulation?

Although... if you're talking ATM PVCs rather than packets, I could
imagine adding minor/adult negotiation to the setup phase. But despite the
hype, I don't expect to see many people using raw ATM (not LAN
emulation/encapsulation) for a decade, if at all.

>         My (simplistically presented) suggestion in such a scheme would be
> that we don't want a "flag" on packets: we want two "fields":
>         - content-classification field in packets:
>                 _roughly_ analogous to a dewey-decimal number -- says a
>                 lot (?) about the content, not merely which end of the
>                 library it goes in
>
>         - user-classification field appended to user-id's:
>                 a micro-bio of the user -- says something
>                 about age, languages known, interests

We're talking packets here, not sessions.

>         Before you flame -- I'm not thinking about the potential abuses,
> I'm thinking about the useful applications: more useful filtering based on
> such fields can be installed as agents on:
>         - user machine
>         - "dial-in" network node
>         - retrieval engines
>         - database engines

For this you use different TCP ports and out-of-band cryptographic
authentication, not extra fields in the packets.

-rich





{% endraw %}
```

## Thread

+ Return to [April 1996](/archive/1996/04)

+ Return to "[Rich Graves <llurch<span>@</span>networking.stanford.edu>](/authors/rich_graves_llurch_at_networking_stanford_edu_)"
+ Return to "[rkmoore<span>@</span>iol.ie (Richard K. Moore)](/authors/rkmoore_at_iol_ie_richard_k_moore_)"

+ 1996-04-13 (Sat, 13 Apr 1996 16:03:33 +0800) - [Re: Protocols at the Point of a Gun](/archive/1996/04/c292ccd58f5706e222285979a0f185c5b63925edc23e4a2df84c0166776cb680) - _rkmoore@iol.ie (Richard K. Moore)_
  + 1996-04-13 (Sat, 13 Apr 1996 20:12:00 +0800) - Re: Protocols at the Point of a Gun - _Rich Graves \<llurch@networking.stanford.edu\>_

