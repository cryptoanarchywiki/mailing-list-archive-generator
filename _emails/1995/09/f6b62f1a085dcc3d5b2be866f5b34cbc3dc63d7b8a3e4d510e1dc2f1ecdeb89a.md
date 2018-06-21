---
layout: default
---

# 1995-09-05 - Another Son of Clipper discussion paper

## Header Data

From: m5@dev.tivoli.com (Mike McNally)<br>
To: Jim Gillogly \<jim@rand.org\><br>
Message Hash: f6b62f1a085dcc3d5b2be866f5b34cbc3dc63d7b8a3e4d510e1dc2f1ecdeb89a<br>
Message ID: \<9509052136.AA11617@alpha\><br>
Reply To: \<199509052053.NAA01226@mycroft.rand.org\><br>
UTC Datetime: 1995-09-05 21:37:28 UTC<br>
Raw Date: Tue, 5 Sep 95 14:37:28 PDT<br>

## Raw message

```
{% raw  %}From: m5@dev.tivoli.com (Mike McNally)
Date: Tue, 5 Sep 95 14:37:28 PDT
To: Jim Gillogly <jim@rand.org>
Subject: Another Son of Clipper discussion paper
In-Reply-To: <199509052053.NAA01226@mycroft.rand.org>
Message-ID: <9509052136.AA11617@alpha>
MIME-Version: 1.0
Content-Type: text/plain



This is really interesting to me:

Jim Gillogly forwards:
 > Key Escrow Issues Meeting, September 6-7, 1995
 > Discussion Paper #3
 > 
 >                  Export Criteria Discussion Draft --
 >                 64-bit Software Key Escrow Encryption
 > . . .
 >                           --- Draft Export Criteria ---
 > for Software Key Escrow Encryption
 > 
 > Software key escrow encryption products meeting the following
 > criteria will be granted special export licensing...
 > 
 > 1.    The product will use an unclassified encryption algorithm
 >       (e.g., DES, RC4) with a key length not to exceed 64 bits.

Ok, sounds good... but what I don't understand is further on:

 > 5.    The product shall be resistant to any alteration that would
 >       disable or circumvent the key escrow mechanism, to include
 >       being designed so that the key escrow mechanism cannot be
 >       disabled by a static patch, (i.e., the replacement of a
 >       block of code by a modified block).

[ that I can understand ]

 > 6.    The product shall not decrypt messages or files encrypted by
 >       non-escrowed products, including products whose key escrow
 >       mechanisms have been altered or disabled.

This is where I start scratching my head.  I mean, how exactly will
the software be able to tell that what's being fed into it came from a
Good version versus an Evil version of the cryptosystem?  Isn't that
very issue the reason for Skipjack being (A) secret and (B) kept on a
supposedly auto-desctruct chip?

If the algorithm is public (and to stretch a point, if the executable
makes it onto somebody's hard disk, it's effectively public), I don't
really understand how the above can be made a realistic goal.  I'd
always thought that the idea behind software key escrow was that it'd
be stuck into most "name-brand" tools, so that Joe Lazy AOL User
wouldn't bother (or wouldn't know how) to circumvent it.  (Still seems
kinda ridiculous, but maybe that's just me.)  Anyway, this document
makes it seem like somebody seriously expects this is doable.  If it
is, then I *really* want to know how (because I'd like to exploit that
sort of technology myself...).

 > 7.    The key escrow mechanism allows access to a user's encrypted
 >       information regardless of whether that user is the sender or
 >       the intended recipient of the encrypted information.

Ooh.

 > 8.    The key escrow mechanism shall not require repeated
 >       involvement by the escrow agents for the recovery of
 >       multiple decryption keys during the period of authorized
 >       access.

Hmm...

 > 9.    In the event any such product is or may be available in the
 >       United States, each production copy of the software shall
 >       either have a unique key required for decrypting messages or
 >       files that is escrowed in accordance with #10, 

Well there go the manufacturing costs up through the roof...

 >       or have the
 >       capability for its escrow mechanism to be rekeyed and any
 >       new key to be escrowed in accordance with #10.

I guess that'd work with the somewhat weak mechanisms used with
"unlockable" CD-ROM stuff.

 > 10.   The product shall accept escrow of its key(s) only with
 >       escrow agents certified by the U.S. Government or by foreign
 >       governments with which the U.S. Government has formal
 >       agreements consistent with U.S. law enforcement and national
 >       security requirements.

Again, how can it tell?

Maybe I'm just being dense.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
| Nobody's going to listen to you if you just | Mike McNally (m5@tivoli.com) |
| stand there and flap your arms like a fish. | Tivoli Systems, Austin TX    |
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~



{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ 1995-09-05 (Tue, 5 Sep 95 13:54:02 PDT) - [Another Son of Clipper discussion paper](/archive/1995/09/32142df791f8c5b949547b1276a32eceb4687a87f28e668e19cc2fe6f878f875) - _Jim Gillogly \<jim@rand.org\>_
  + 1995-09-05 (Tue, 5 Sep 95 14:37:28 PDT) - Another Son of Clipper discussion paper - _m5@dev.tivoli.com (Mike McNally)_
  + 1995-09-06 (Wed, 6 Sep 95 01:57:46 PDT) - [Re: Another Son of Clipper discussion paper](/archive/1995/09/964efcbb8560a1bffc928bcd10981ea31237761bef0f71d16c6e8d11ae0f4d6f) - _Deranged Mutant \<rrothenb@ic.sunysb.edu\>_
  + 1995-09-07 (Wed, 6 Sep 95 23:30:51 PDT) - [Re: Another Son of Clipper discussion paper](/archive/1995/09/42d293ccf7a95c65bbce8aa95acfc0095ab4cc37cdf21c9cafe8ab3cfc774e7c) - _"Vladimir Z. Nuri" \<vznuri@netcom.com\>_

