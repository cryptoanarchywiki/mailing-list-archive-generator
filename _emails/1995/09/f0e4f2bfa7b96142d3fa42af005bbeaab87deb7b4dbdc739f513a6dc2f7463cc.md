---
layout: default
---

# 1995-09-04 - Re: SSL search attacks

## Header Data

From: Jiri Baum \<jirib<span>@</span>sweeney.cs.monash.edu.au\><br>
To: sjb@austin.ibm.com (Scott Brickner)<br>
Message Hash: f0e4f2bfa7b96142d3fa42af005bbeaab87deb7b4dbdc739f513a6dc2f7463cc<br>
Message ID: \<199509040132.LAA21977@sweeney.cs.monash.edu.au\><br>
Reply To: \<9508311728.AA16306@ozymandias.austin.ibm.com\><br>
UTC Datetime: 1995-09-04 01:33:40 UTC<br>
Raw Date: Sun, 3 Sep 95 18:33:40 PDT<br>

## Raw message

```
{% raw  %}From: Jiri Baum <jirib@sweeney.cs.monash.edu.au>
Date: Sun, 3 Sep 95 18:33:40 PDT
To: sjb@austin.ibm.com (Scott Brickner)
Subject: Re: SSL search attacks
In-Reply-To: <9508311728.AA16306@ozymandias.austin.ibm.com>
Message-ID: <199509040132.LAA21977@sweeney.cs.monash.edu.au>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

Hello cypherpunks@toad.com
  and Scott Brickner <sjb@austin.ibm.com>

Scott Brickner <sjb@austin.ibm.com> writes:
> Jiri Baum writes
...
> >Each client could pick a segment at random, check it and then broadcast
> >a NAK. Other clients would then know that the segment in question has
...
> This only reduces the cost if everyone is playing fair.  In practice,
...

No worse than fake NAKs to the central server (viz comment below).

> >One advantage is that it is not necessary to have a central infinitely
> >trusted server. (Nothing personal, but bogus server is an attack.)
> 
> An attack on what?  The overall model here is that someone presents
...

An attack on the attempt. If the key owner also volunteers a server,
then half the CPU cycles will report to that server (and be given
useless chunks of keyspace) thus halving the CPU power available to
the usual server ("half" in an infinitely naive world, of course).

The approach I suggested basically corresponds to everyone maintaining
hir own server; servers that trust each other will coordinate.
An attacker can of course NAK the key segment, but only those that trust
the attacker will take any notice.

> My point is that the "random" efforts are no different than everyone
> working on the problem independently, each picking a random place to
> start and going sequentially from there.

The difference is that in this scheme everyone does coordinate, only
it's peer-peer rather than client-server.

> >NAKs and IGRABs would be weighted by the trust accorded to the entity
> >that originated them.
> 
> This is similar to what I outlined yesterday afternoon.  Let unsolicited
...

I think that's where it came from. I really should provide citations,
shouldn't I...

...
> Invalid unsolicited NAKs
> don't destroy the current search, they only slow it down slightly ---
> but less than a fully random effort.

Similarly in the peer-peer approach, the effort is coordinated but
untrusted NAKs slow it down only slightly. The only "solicited" NAKs
will be your own.


Hope that makes sense...

Jiri
- --
If you want an answer, please mail to <jirib@cs.monash.edu.au>.
On sweeney, I may delete without reading!
PGP 463A14D5 (but it's at home so it'll take a day or two)
PGP EF0607F9 (but it's at uni so don't rely on it too much)

-----BEGIN PGP SIGNATURE-----
Version: 2.6.2i

iQCVAwUBMEpXLSxV6mvvBgf5AQFn2QP/eJ0BlATPHS2xoLoJuHdJYR7Y5gN5scmK
DHOby7rGJ3Rj6CZ6PrdkQVf9ckUdmUwhCzAiCi3wnPHPf0gi4rPjLyBpmyTgl8yA
q+VqYPkBAflwHqXIsqbxx94PiZayt8b578Qtqoa2jJzjSCKMa8IonWGeztP/xNxa
FCmJDocudq4=
=r/Hv
-----END PGP SIGNATURE-----



{% endraw %}
```

## Thread

+ Return to [August 1995](/archive/1995/08)
+ Return to [September 1995](/archive/1995/09)

+ Return to "[don<span>@</span>cs.byu.edu](/author/don_at_cs_byu_edu)"
+ Return to "[Jiri Baum <jirib<span>@</span>sweeney.cs.monash.edu.au>](/author/jiri_baum_jirib_at_sweeney_cs_monash_edu_au_)"
+ Return to "[Scott Brickner <sjb<span>@</span>austin.ibm.com>](/author/scott_brickner_sjb_at_austin_ibm_com_)"

+ 1995-08-29 (Tue, 29 Aug 95 14:01:35 PDT) - [SSL search attacks](/archive/1995/08/944e363c5d22443f1006954f38fbee6afc85cc537b6a4a30f89a7d60505271c9) - _don@cs.byu.edu_
  + 1995-08-30 (Tue, 29 Aug 95 18:01:35 PDT) - [Re: SSL search attacks](/archive/1995/08/4a675293882eed3d65318cbfc391e5fb0b2ac5b49dbe9585dbe7833122a9fd3d) - _Scott Brickner \<sjb@austin.ibm.com\>_
    + 1995-08-31 (Thu, 31 Aug 95 02:27:56 PDT) - [Re: SSL search attacks](/archive/1995/08/15af5f2cb16542ad1eb89f741d74856e03f856f1014205fa93e507f08e3e1b93) - _Jiri Baum \<jirib@sweeney.cs.monash.edu.au\>_
      + 1995-08-31 (Thu, 31 Aug 95 10:30:38 PDT) - [Re: SSL search attacks](/archive/1995/08/e9549482b2dd176b25e1852847cb3918a7c8d7087aaa24e74dee1ada80021e1b) - _Scott Brickner \<sjb@austin.ibm.com\>_
        + 1995-09-04 (Sun, 3 Sep 95 18:33:40 PDT) - Re: SSL search attacks - _Jiri Baum \<jirib@sweeney.cs.monash.edu.au\>_

