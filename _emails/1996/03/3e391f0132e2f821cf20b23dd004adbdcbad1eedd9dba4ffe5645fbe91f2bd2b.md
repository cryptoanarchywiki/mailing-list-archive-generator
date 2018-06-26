---
layout: default
---

# 1996-03-08 - Re: Looking for code to run an encrypted mailing list

## Header Data

From: abostick<span>@</span>netcom.com (Alan Bostick)<br>
To: stewarts@ix.netcom.com<br>
Message Hash: 3e391f0132e2f821cf20b23dd004adbdcbad1eedd9dba4ffe5645fbe91f2bd2b<br>
Message ID: \<baHQx8m9LwlQ085yn@netcom.com\><br>
Reply To: \<199603060542.VAA28896@ix9.ix.netcom.com\><br>
UTC Datetime: 1996-03-08 22:00:38 UTC<br>
Raw Date: Sat, 9 Mar 1996 06:00:38 +0800<br>

## Raw message

```
{% raw  %}From: abostick@netcom.com (Alan Bostick)
Date: Sat, 9 Mar 1996 06:00:38 +0800
To: stewarts@ix.netcom.com
Subject: Re: Looking for code to run an encrypted mailing list
In-Reply-To: <199603060542.VAA28896@ix9.ix.netcom.com>
Message-ID: <baHQx8m9LwlQ085yn@netcom.com>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

In article <199603060542.VAA28896@ix9.ix.netcom.com>,
Bill Stewart <stewarts@ix.netcom.com> wrote:

> On the other hand, it really only costs you one IDEA encryption if you
> want to use the multiple-recipients options to PGP.  With the current PGP,
> this means you don't have to hack your own crypto code; the toolkits in PGP 3.0
> will make that easier, though.

True, and reasonable.

Suppose, though, that the Cypherpunks list was encrypted in this way.
There are about a thousand listmembers.  Using one IDEA key and the
multiple-recipients option would mean that the encrypted message would
consist of a thousand RSA-encrypted session keys followed by the
IDEA-encrypted cyphertext.  If everyone used a 1024-bit-or-longer key
pair, then each message would be a megabyte long!

( (m**P) mod n is going to be log2(n) bits long, right?)

BTW, it was pointed out to me in private email that while vanilla RSA
commutes, the PKCS-compliant RSA in PGP which pads the session key with
random data does not, so that my nifty trick to never expose cleartext
in the list processor wouldn't work.  That's why I'm just a loudmouth
blowhard and not a real cryptographer. ;-) 


- -- 
   Alan Bostick             | "If I am to be held in contempt of court,
Seeking opportunity to      | your honor, it can only be because the court
develop multimedia content. | has acted contemptibly!"
Finger abostick@netcom.com for more info and PGP public key

-----BEGIN PGP SIGNATURE-----
Version: 2.6.2

iQB1AwUBMUB7v+VevBgtmhnpAQHKXwMAhcjT3R6hE8jtGBEY3uHZ7Y3cOycQEpXP
dSQ2TsK27vYpCCjFBe3JauxLBBpM6yPqhPq8rSerNaQ7a8lhAWB4UwcUTwh9S7U3
PobslFhkFEwPd9jnZwY4g0ZZKb3iABIO
=sLrM
-----END PGP SIGNATURE-----




{% endraw %}
```

## Thread

+ Return to [March 1996](/archive/1996/03)

+ Return to "[abostick<span>@</span>netcom.com (Alan Bostick)](/author/abostick_at_netcom_com_alan_bostick_)"
+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/author/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "["James Black (CS)" <black<span>@</span>eng.usf.edu>](/author/james_black_cs__black_at_eng_usf_edu_)"

+ 1996-03-07 (Thu, 7 Mar 1996 22:33:14 +0800) - [Re: Looking for code to run an encrypted mailing list](/archive/1996/03/4f9e56c5124257331bc2f7ffba22f085c4627f4773ddefeb7e2348a8a0fbaff4) - _Bill Stewart \<stewarts@ix.netcom.com\>_
  + 1996-03-08 (Sat, 9 Mar 1996 06:00:38 +0800) - Re: Looking for code to run an encrypted mailing list - _abostick@netcom.com (Alan Bostick)_
    + 1996-03-09 (Sun, 10 Mar 1996 04:00:56 +0800) - [Re: Looking for code to run an encrypted mailing list](/archive/1996/03/68b4ee4948da8a10c6abfb5d9df76be4c394e793da5bd478cce3f123912090bc) - _"James Black (CS)" \<black@eng.usf.edu\>_

