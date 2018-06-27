---
layout: default
---

# 1994-09-28 - Re: Mandatory email verification

## Header Data

From: dps<span>@</span>kafka.atinc.com (Doug Shapter)<br>
To: dcwill@ee.unr.edu<br>
Message Hash: ad8ee84b0debc60afb8d3e678b699efbadb227e0d18b73b3a08d8dd5f5cc08fa<br>
Message ID: \<9409280832.ZM12030@kafka.atinc.com\><br>
Reply To: \<199409272247.RAA18617@pentagon.io.com\><br>
UTC Datetime: 1994-09-28 12:32:17 UTC<br>
Raw Date: Wed, 28 Sep 94 05:32:17 PDT<br>

## Raw message

```
{% raw  %}From: dps@kafka.atinc.com (Doug Shapter)
Date: Wed, 28 Sep 94 05:32:17 PDT
To: dcwill@ee.unr.edu
Subject: Re: Mandatory email verification
In-Reply-To: <199409272247.RAA18617@pentagon.io.com>
Message-ID: <9409280832.ZM12030@kafka.atinc.com>
MIME-Version: 1.0
Content-Type: text/plain


Its my understanding that to be truly useful on multi-user
systems, digital signatures require some user input (eg, PGP
requires entering a pass phrase). Sendmail could be hacked
easily
enough to append signatures and to even ask the user for the
requisite pass phrase-- or sendmail can append the signature
automagically, using an environment variable (yuch, just a touch
insecure?) or some other method (a root-owned and executed shell
script).

The first method, having sendmail ask the user for the pass
phrase, is most secure, but also the most inconvienent. For
instance, at our site, we have several distributed
workstations. We send numerous mail messages to each other every
day, and signing each one would be a real pain. To prevent this
sendmail could be hacked to only require signatures on mail
messages addressed outside the domain. This still leaves us back
at the original problem-- one of us could flame the boss and
then
deny the authenticity of the message because it lacked our
signature.

The automagic method is frightfully insecure. Creating an
environment variable transparently requires that the pass phrase
be physically located on the system, instead of the user's
mind. (I wouldn't want to ask users to slip in their "pass
phrase" disk every morning when they log on). There is also a
question of trust-- a dishonest sysadm could easily break this
method. The dishonest sysadm could also easily break a shell
script method, as could anyone who got the root password.

Jim McCoy pointed out aptly that the hack could be done quickly,
but, laying technical issues aside, do we really want our
computers signing our mail for us (what about messages to
anonymous remailers-- a digital signature defeats that in short
order)? That's the real question.



-- 
Doug Shapter                
dps@kafka.atinc.com         
finger dps@kryten.atinc.com for PGP public key




{% endraw %}
```

## Thread

+ Return to [September 1994](/archive/1994/09)

+ Return to "[Adam Shostack <adam<span>@</span>bwh.harvard.edu>](/authors/adam_shostack_adam_at_bwh_harvard_edu_)"
+ Return to "["Dave Emery" <die<span>@</span>pig.die.com>](/authors/dave_emery_die_at_pig_die_com_)"
+ Return to "[dps<span>@</span>kafka.atinc.com (Doug Shapter)](/authors/dps_at_kafka_atinc_com_doug_shapter_)"
+ Return to "["Dr. D.C. Williams" <dcwill<span>@</span>ee.unr.edu>](/authors/dr_d_c_williams_dcwill_at_ee_unr_edu_)"
+ Return to "[m5<span>@</span>vail.tivoli.com (Mike McNally)](/authors/m5_at_vail_tivoli_com_mike_mcnally_)"
+ Return to "[mccoy<span>@</span>io.com (Jim McCoy)](/authors/mccoy_at_io_com_jim_mccoy_)"

+ 1994-09-27 (Tue, 27 Sep 94 14:25:48 PDT) - [Mandatory email verification](/archive/1994/09/f5e593b59431212121dfa811f865b7703bde884b6796959903b26c40a3091112) - _"Dr. D.C. Williams" \<dcwill@ee.unr.edu\>_
  + 1994-09-27 (Tue, 27 Sep 94 14:51:54 PDT) - [Mandatory email verification](/archive/1994/09/6311a1143635a578b1da238053ebecb4542e8b8df06ed8aa1198c7477f14613f) - _m5@vail.tivoli.com (Mike McNally)_
  + 1994-09-27 (Tue, 27 Sep 94 15:02:23 PDT) - [Re: Mandatory email verification](/archive/1994/09/7dfc29999a3aba066201f96bf2346da26c69c5e144b86f506e0e3fa939ff117a) - _Adam Shostack \<adam@bwh.harvard.edu\>_
  + 1994-09-27 (Tue, 27 Sep 94 15:48:37 PDT) - [Re: Mandatory email verification](/archive/1994/09/c65173cbe192248acc28896beb03a6e29cae4315efbf4e09a73be84ef258b31e) - _mccoy@io.com (Jim McCoy)_
    + 1994-09-28 (Wed, 28 Sep 94 05:32:17 PDT) - Re: Mandatory email verification - _dps@kafka.atinc.com (Doug Shapter)_
      + 1994-09-28 (Wed, 28 Sep 94 06:34:03 PDT) - [Re: Mandatory email verification](/archive/1994/09/c5fff81d413ad33f341c7d8b9b2d003aebcbab5ea6b3c6596e7805ca3c388848) - _"Dr. D.C. Williams" \<dcwill@ee.unr.edu\>_
        + 1994-09-28 (Wed, 28 Sep 94 13:56:47 PDT) - [Re: Mandatory email verification](/archive/1994/09/4022105d80dd8fc284de5163e9ef85b879dca465780f6ae2105d03231726e637) - _"Dave Emery" \<die@pig.die.com\>_
      + 1994-09-28 (Wed, 28 Sep 94 13:53:15 PDT) - [Re: Mandatory email verification](/archive/1994/09/bc6195cced017b4970d446d06218113b7a6f49695b9d68ad5021efaf881fedcc) - _mccoy@io.com (Jim McCoy)_

