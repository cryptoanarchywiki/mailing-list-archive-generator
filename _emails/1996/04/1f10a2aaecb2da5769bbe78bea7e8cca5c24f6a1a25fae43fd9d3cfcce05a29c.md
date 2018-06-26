---
layout: default
---

# 1996-04-10 - RISKS: Compuserve "secure" login

## Header Data

From: stevenw<span>@</span>best.com (Steven Weller)<br>
To: cypherpunks@toad.com<br>
Message Hash: 1f10a2aaecb2da5769bbe78bea7e8cca5c24f6a1a25fae43fd9d3cfcce05a29c<br>
Message ID: \<v01540b01ad90cf8c8249@[206.86.1.35]\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-04-10 11:34:22 UTC<br>
Raw Date: Wed, 10 Apr 1996 19:34:22 +0800<br>

## Raw message

```
{% raw  %}From: stevenw@best.com (Steven Weller)
Date: Wed, 10 Apr 1996 19:34:22 +0800
To: cypherpunks@toad.com
Subject: RISKS: Compuserve "secure" login
Message-ID: <v01540b01ad90cf8c8249@[206.86.1.35]>
MIME-Version: 1.0
Content-Type: text/plain


------------------------------

Date: Thu, 04 Apr 1996 19:34:12 +0200
From: Heinz-Bernd Eggenstein <eggenste@noether.informatik.uni-dortmund.de>
Subject: CompuServe's "secure login protocol": two steps forward, one back

Summary: a new CompuServe Information Service (CIS) logon protocol was
designed to prevent passive and active attacks (where the attacker
impersonates a CompuServe node) but a flawed implementation in the
WinCIM 2.0(.1) client software still allows active attacks.

Version 2.0 of the "WinCIM" access software introduced a new logon protocol.
Previous versions of the software had transmitted the user's UID AND his/her
password in plaintext during logon. The risks are obvious, especially when
connecting via the Internet to CompuServe (e.g. to save long distance
telephone charges).

The new, "secure logon protocol" is a challenge-response type protocol where
the "challenge" is to compute a keyed hash-function, the key is derived from
the shared secret, the user's password:

1) The client (WinCIM) generates a pseudorandom string of bits, its "nonce"
   (RB)
2) The client transmits the user's UID (e.g. 12345,6789) and the additional
   parameter "/secure:1" to request a secure login.
3) The host transmits its pseudo random nonce (RA) (The old protocol would
   instead prompt for the password)
4) client sends RB to the host
5) client computes  UR:=MD5(S|Z|RA|RB|S) and sends it to the host
   (where S (128 bits) is a function of the password, "|" stands for
   concatenation, Z is a 128bits block of 0s and MD5 is the well
   known message digest function.)
6) The host performs the same calculation with it's copy of the user's
   password. If the results match, the host sends HR:=MD5(S|Z|RB|RA|S)
   (Note the symmetry in the calculation of HR and UR)
7) The client software verifies HR with it's copy of the password to
   make sure the host is really a CIS node (!)

(See the script-files cserve.scr and seclog.scr in the subdirectory SCRIPTS
of a WINCIM 2.0(.1) installation, WinCim is available via anon. ftp
at ftp.compuserve.com).

Weaknesses:

a) The scriptfile cserve.scr (versions 3.8 & 3.8.1) has the following bug:
   even after requesting a secure logon, the client software will fall back
   into the old protocol when receiving a "Password" prompt (Client: "I want
   a secure logon" Host:"OK, but anyway, give me your password" Client "Well
   ok then, here it is ..."). It will send the password in plaintext! This
   makes the protection against active attacks (see step 7) obsolete.

b) A timeout condition or even an invalid HR response form the host will
   (seclog.scr & cserve.scr version 3.8.1) restart the protocol (it won't
   disconnect!), using *the same* client-nonce RB again, instead of
   generating a new one. If a spoofing host can predict RB as in this
   situation, it can pick the same nonce, leading to HR=UR=MD5(S|Z|RB|RB|S),
   so the host can just send back UR as HR.

Note that unlike a), b) does not compromise the user's password.

There may be other ways to predict the client software's nonce e.g. *if* the
PRNG used by WinCIM is predictable (this calls for further investigation).

Note that *offline* dictionary attacks to guess the password are possible
after a passive, eavesdropping attack (so you still have to pick a "good"
password). It's debatable whether CIS's password recommendation
(<word><non-alphanum. char.><word>, both words unrelated, e.g.
apple@battery) is adequate in this context).

I notified CIS about these weaknesses and I was informed that they are
"fixed" now, no details were given about the fix (source: Britta Herbst,
German customer support (11111.754@compuserve.com)).

Risks? The new protocol is obviously an improvement over the old,
plaintext-password-only version. It's debatable whether protection against
active attacks is at all necessary for access to an online service. However,
CIS itself designed it's protocol to prevent spoofing attacks. Anyway, I
think this a good example how to half-ruin a good protocol by embedding it
into carelessly written code.

Credits: Thanks to Gary Brown (70003.1215@compuserve.com) for sending me
information on the implementation of the new protocol).

Heinz-Bernd Eggenstein [usual disclaimers]

------------------------------

-------------------------------------------------------------------------
Steven Weller                      |  Weller's three steps to Greatness:
                                   |     1. See what others cannot
                                   |     2. Think what others cannot
stevenw@best.com                   |     3. Express what others cannot






{% endraw %}
```

## Thread

+ Return to [April 1996](/archive/1996/04)

+ Return to "[stevenw<span>@</span>best.com (Steven Weller)](/author/stevenw_at_best_com_steven_weller_)"

+ 1996-04-10 (Wed, 10 Apr 1996 19:34:22 +0800) - RISKS: Compuserve "secure" login - _stevenw@best.com (Steven Weller)_

