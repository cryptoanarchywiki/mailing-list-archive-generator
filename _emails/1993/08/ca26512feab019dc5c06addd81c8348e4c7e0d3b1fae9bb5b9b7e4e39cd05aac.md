---
layout: default
---

# 1993-08-28 - Cisco vulnerabilities?

## Header Data

From: fergp<span>@</span>sytex.com (Paul Ferguson)<br>
To: cypherpunks@toad.com<br>
Message Hash: ca26512feab019dc5c06addd81c8348e4c7e0d3b1fae9bb5b9b7e4e39cd05aac<br>
Message ID: \<Jk8u9B3w165w@sytex.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-08-28 01:42:58 UTC<br>
Raw Date: Fri, 27 Aug 93 18:42:58 PDT<br>

## Raw message

```
{% raw  %}From: fergp@sytex.com (Paul Ferguson)
Date: Fri, 27 Aug 93 18:42:58 PDT
To: cypherpunks@toad.com
Subject: Cisco vulnerabilities?
Message-ID: <Jk8u9B3w165w@sytex.com>
MIME-Version: 1.0
Content-Type: text/plain


On Thu, 26 Aug 93 21:17:16 -0600,
 L. Detweiler <uunet!longs.lance.colostate.edu!ld231782> wrote -
 
> ===cut=here===
>
> Date: Wed, 25 Aug 1993 12:56:54 -0700 (PDT)
> From: Al Whaley <Al.Whaley@sunnyside.com>
> Subject: Cisco routers
>
> Rumors abound that Cisco routers have a back door; that is when
> a TCP port is disabled, it can still be accessed from Cisco's
> IP number.
>
> I have personally verified this with the sendmail port.
>
> Al Whaley        al@sunnyside.com       +1-415 322-5411(Tel), -6481 
(Fax)
> Sunnyside Computing, Inc., PO Box 60, Palo Alto, CA 94302
>
 
 Sure, they have a backdoor -- it's called unsecured ports and
 lackidaisical security.
 
 Cisco routers don't really have "TCP" ports, per se. They have
 ethernet ports, or token ring ports, v.35 serial ports, and
 dial-up rs-232 for fail-safe configuration when some idiot drops
 your feed at the local rboc and you need to "look into" your net.
 
 If the "entrance" passwords are enabled properly, then I feel quite
 sure that this threat is minimal. However, I have learned recently
 that some facets of SNMP encapsulation can exploit _management_ but
 can not, however exploit the configuration of the router. It can add
 to the traffic overhead.
 
 Also, there is an additional "enable" password for configuration
 modification, such as changing IP addresses of the ethernet or serial
 interfaces (ports) and saving the configuration to NVRAM.
 
 I had a guy adamantly try to convince me the other day that the
 (Cisco) routers were in jeopardy because of the ability to TFTP
 a new (albeit, damaging) operating system directly into NVRAM
 (a sleight of hand), rendering the box useless. It can be done,
 in fact, Cisco would have to ship me a whole new box overnight
 if it happened, but if I mind my P's and Q's (read: adhere to
 proper security), he's pissin' in the wind.
 
 ;-)
 
 Cheers,

Paul Ferguson               |  "Government, even in its best state,
Network Integrator          |   is but a necessary evil; in its worst
Centreville, Virginia USA   |   state, an intolerable one."
fergp@sytex.com             |      - Thomas Paine, Common Sense
 
Type bits/keyID   Date       User ID
pub  1024/1CC04D 1993/03/15  Paul Ferguson <fergp@sytex.com>
  Key fingerprint =  EE D2 93 7D 04 6D C6 05  AC 36 AD 9D 8E 4F 41 58




{% endraw %}
```

## Thread

+ Return to [August 1993](/archive/1993/08)

+ Return to "[fergp<span>@</span>sytex.com (Paul Ferguson)](/author/fergp_at_sytex_com_paul_ferguson_)"

+ 1993-08-28 (Fri, 27 Aug 93 18:42:58 PDT) - Cisco vulnerabilities? - _fergp@sytex.com (Paul Ferguson)_

