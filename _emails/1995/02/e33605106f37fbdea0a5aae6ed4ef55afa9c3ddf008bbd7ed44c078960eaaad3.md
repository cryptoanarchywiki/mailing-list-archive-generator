---
layout: default
---

# 1995-02-02 - MX'ing and jpunix.com

## Header Data

From: "John A. Perry" \<perry@jpunix.com\><br>
To: alt.privacy.anon-server@myriad.pc.cc.cmu.edu<br>
Message Hash: e33605106f37fbdea0a5aae6ed4ef55afa9c3ddf008bbd7ed44c078960eaaad3<br>
Message ID: \<199502022127.PAA14199@jpunix.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-02-02 21:29:14 UTC<br>
Raw Date: Thu, 2 Feb 95 13:29:14 PST<br>

## Raw message

```
{% raw  %}From: "John A. Perry" <perry@jpunix.com>
Date: Thu, 2 Feb 95 13:29:14 PST
To: alt.privacy.anon-server@myriad.pc.cc.cmu.edu
Subject: MX'ing and jpunix.com
Message-ID: <199502022127.PAA14199@jpunix.com>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----


	JPUNIX.COM (soon to be alias.net) offers a MX service for
individuals that want to run an anonymous remailer but don't want the
domain they are operating from to be immediately apparent. By making
application to perry@jpunix.com, a remailer operator will be granted a DNS
MX record pointing to the domain address of the requestor's choice and 
will appear to reside in the jpunix.com (alias.net) domain. 

	Additional masking can be provided by having the MX record point
to myriad.pc.cc.cmu.edu. What good does this do? I have an agreement with
myriad.pc.cc.cmu.edu (Matt Ghio) where myriad will take the MX-pointed
record and additionally alias it through the smail daemon on myriad. This
function adds the unique benefit where determining the actual location of
the remailer in question will be foiled when using nslookup.  Since an
additional alias is performed the result of an nslookup will always point
to myriad. The actual location of the remailer remains hidden inside the
alias on myriad. Lastly, Matt has the EXPN function of his sendmail daemon
disabled so the identity of the remailer can't be determined by alias
expansion. 

	Future modifications to this scheme include adding an addition
step whereby the MX-alias process will cause a version of Raph Levien's
premail to post-process the message to add one or more random remailer
paths the the overall path that the message travels. This step in still in
the planning stages and has not been implemented yet. 

	If you have and questions, or want to set up an MX record, send
email to: 

perry@jpunix.com or ghio@myriad.pc.cc.cmu.edu

John Perry < perry@jpunix.com>


-----BEGIN PGP SIGNATURE-----
Version: 2.6.2

iQCVAwUBLzFN6lOTpEThrthvAQHfAAQAkzoGHz7iaJKHMzB5GEQr8OvEwhDY0F9s
lCZUJhTw3KV2hVWDoUtZNPwiSf4vcsDhGx0CDQrDUon2vXC0mOHj4zBbDhhuUD5l
/NCPOmtWKFSnWiny2JbD0esNIuxIaWfa/tVTkDoDq/zPtsG0awmHTpGMSeIkkxvy
II1mDwnZ9n0=
=2jQD
-----END PGP SIGNATURE-----




{% endraw %}
```

## Thread

+ Return to [February 1995](/archive/1995/02)

+ 1995-02-02 (Thu, 2 Feb 95 13:29:14 PST) - MX'ing and jpunix.com - _"John A. Perry" \<perry@jpunix.com\>_
  + 1995-02-03 (Fri, 3 Feb 95 15:14:54 PST) - [Re: MX'ing and jpunix.com](/archive/1995/02/365ba2228267fcc1cbbe02772d7854b59b2aa3ca23f13ae2d7027aca9e1fc00a) - _eric@remailer.net (Eric Hughes)_

