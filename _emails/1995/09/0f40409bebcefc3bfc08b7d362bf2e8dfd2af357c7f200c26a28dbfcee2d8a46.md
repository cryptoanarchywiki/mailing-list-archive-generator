---
layout: default
---

# 1995-09-08 - Re: Scientology tries to break PGP - and fails?

## Header Data

From: Andrew Loewenstern \<andrew_loewenstern<span>@</span>il.us.swissbank.com\><br>
To: trollins@hns.com (Tom Rollins)<br>
Message Hash: 0f40409bebcefc3bfc08b7d362bf2e8dfd2af357c7f200c26a28dbfcee2d8a46<br>
Message ID: \<9509081654.AA03407@ch1d157nwk\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-09-08 16:55:01 UTC<br>
Raw Date: Fri, 8 Sep 95 09:55:01 PDT<br>

## Raw message

```
{% raw  %}From: Andrew Loewenstern <andrew_loewenstern@il.us.swissbank.com>
Date: Fri, 8 Sep 95 09:55:01 PDT
To: trollins@hns.com (Tom Rollins)
Subject: Re: Scientology tries to break PGP - and fails?
Message-ID: <9509081654.AA03407@ch1d157nwk>
MIME-Version: 1.0
Content-Type: text/plain


Tom Rollins writes:
>  If this is the file that the Co$ is trying to crack, then what the
>  is being asked for is a pass phrase that can be handed to the Co$
>  that will pass the PGP valid key check and still not decrypt the
>  data to anything usefull.

Well, I don't have the PGP 'conventional' encryption format memorized, but  
there is probably a constant after the IV that is prepended to the data.  The  
constant is used to determine if the key is correct.  Since the conventional  
encryption runs in CFB mode and there is a full block of random IV at the  
beginning of the file, it is extremely unlikely that a key could be found  
that would properly decrypt only the first two blocks while leaving the rest  
unreadable...

>  If Larry Wollersheim does have the valid key.  It would be a simpler
>  process to know what fake key to use and work it backwards through
>  the MD5 to arrive at an ascii string to produce the fake key.

Not really.  Even if you could find an IDEA key that would produce the  
desired output it would be hard to find a passphrase that would produce that  
key when hashed.  One of the properties of one-way hash functions is that it  
is difficult to find a plaintext that produces a given hash.  Hence the term  
'one-way'....  Even if you did find a passphrase (which, if MD5 is strong,  
would require something like 2^64 operations), it would likely be long, have  
8-bit chars, and would be impossible to type in.  It would be tough to  
convince anyone that it was the real passphrase.


andrew




{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ Return to "[adwestro<span>@</span>ouray.cudenver.edu (Alan Westrope)](/authors/adwestro_at_ouray_cudenver_edu_alan_westrope_)"
+ Return to "[Andrew Loewenstern <andrew_loewenstern<span>@</span>il.us.swissbank.com>](/authors/andrew_loewenstern_andrew_loewenstern_at_il_us_swissbank_com_)"
+ Return to "[Black Unicorn <unicorn<span>@</span>polaris.mindport.net>](/authors/black_unicorn_unicorn_at_polaris_mindport_net_)"
+ Return to "[cypherpunks<span>@</span>toad.com](/authors/cypherpunks_at_toad_com)"

+ 1995-09-08 (Fri, 8 Sep 95 09:55:01 PDT) - Re: Scientology tries to break PGP - and fails? - _Andrew Loewenstern \<andrew_loewenstern@il.us.swissbank.com\>_
  + 1995-09-09 (Fri, 8 Sep 95 17:45:44 PDT) - [Re: Scientology tries to break PGP - and fails?](/archive/1995/09/5645d7a3f7962851f503e71e7938426ec7e1b8b2308b829e220c774a289f97af) - _adwestro@ouray.cudenver.edu (Alan Westrope)_
    + 1995-09-13 (Wed, 13 Sep 95 16:20:57 PDT) - [Re: Scientology tries to break PGP - and fails?](/archive/1995/09/95e3aed2327b40118b94ab267c2660b95220dc02633f784776dfa93eed357b90) - _Black Unicorn \<unicorn@polaris.mindport.net\>_
  + 1995-09-09 (Sat, 9 Sep 95 01:46:19 PDT) - [Re: Scientology tries to break PGP - and fails?](/archive/1995/09/853ca65bf93f119777942ac6dded14a63a20c5af7751f1cabe49e1d7c27d1697) - _cypherpunks@toad.com_

