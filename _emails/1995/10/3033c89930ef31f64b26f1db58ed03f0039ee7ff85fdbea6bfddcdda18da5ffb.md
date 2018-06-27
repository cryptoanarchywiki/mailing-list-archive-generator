---
layout: default
---

# 1995-10-31 - Re: /dev/random for FreeBSD [was: Re: /dev/random for Linux]

## Header Data

From: shields<span>@</span>tembel.org (Michael Shields)<br>
To: cypherpunks@toad.com<br>
Message Hash: 3033c89930ef31f64b26f1db58ed03f0039ee7ff85fdbea6bfddcdda18da5ffb<br>
Message ID: \<473k3p$pt2@yage.tembel.org\><br>
Reply To: \<199510301925.VAA27116@grumble.grondar.za\><br>
UTC Datetime: 1995-10-31 00:02:31 UTC<br>
Raw Date: Tue, 31 Oct 1995 08:02:31 +0800<br>

## Raw message

```
{% raw  %}From: shields@tembel.org (Michael Shields)
Date: Tue, 31 Oct 1995 08:02:31 +0800
To: cypherpunks@toad.com
Subject: Re: /dev/random for FreeBSD [was: Re: /dev/random for Linux]
In-Reply-To: <199510301925.VAA27116@grumble.grondar.za>
Message-ID: <473k3p$pt2@yage.tembel.org>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

In article <199510301925.VAA27116@grumble.grondar.za>,
Mark Murray <mark@grondar.za> wrote:
> Something I didn't mention earlier; we felt that letting the unwashed
> masses read /dev/*random was not a good idea, as they could deplete
> the pool of entropy all to easily for attack purposes.

That's really just a DOS attack, isn't it?  An application that needs
true randomness should be using /dev/random, which you can slow but not
disturb, and an application that is using /dev/urandom should be ok with
less than full entropy.

-----BEGIN PGP SIGNATURE-----
Version: 2.6.2

iQCVAwUBMJVTqeyjYMb1RsVfAQGqYwP/W6xUdsxwCMrWlvmuPrfV4yfaYpZWt3JW
/ld8HsqyQt5XRkbNwq/hcXDle13exEaqzXe2l6qHtR3qySEaU/4WF/BgSTwqpQa+
iA6p8KL51XPluNF9oagMrmOR2J4yxMPldrx5m/+WcZRJj4mdfzxQoMQ9J4agTVsC
l2spGY8iNkA=
=9cfz
-----END PGP SIGNATURE-----
-- 
Shields.




{% endraw %}
```

## Thread

+ Return to [October 1995](/archive/1995/10)

+ Return to "[Mark Murray <mark<span>@</span>grondar.za>](/authors/mark_murray_mark_at_grondar_za_)"
+ Return to "[shields<span>@</span>tembel.org (Michael Shields)](/authors/shields_at_tembel_org_michael_shields_)"
+ Return to "["Theodore Ts'o" <tytso<span>@</span>MIT.EDU>](/authors/theodore_tso_tytso_at_mit_edu_)"

+ 1995-10-30 (Tue, 31 Oct 1995 05:12:39 +0800) - [Re: /dev/random for FreeBSD [was: Re: /dev/random for Linux]](/archive/1995/10/88052b8069b3a27907f30d4af5c2be1b8b1b73737f8d14e948e8c5deaf38cbe9) - _Mark Murray \<mark@grondar.za\>_
  + 1995-10-30 (Tue, 31 Oct 1995 07:10:10 +0800) - [Re: /dev/random for FreeBSD [was: Re: /dev/random for Linux]](/archive/1995/10/0845d30c258ef42bdbe4fc34f521c30e602c6fe1181dcf44de6eeb4378525559) - _"Theodore Ts'o" \<tytso@MIT.EDU\>_
  + 1995-10-31 (Tue, 31 Oct 1995 08:02:31 +0800) - Re: /dev/random for FreeBSD [was: Re: /dev/random for Linux] - _shields@tembel.org (Michael Shields)_

