---
layout: default
---

# 1996-06-29 - Re: Crack for DOS

## Header Data

From: Bill Stewart \<stewarts<span>@</span>ix.netcom.com\><br>
To: Steve O \<privsoft@ix.netcom.com\><br>
Message Hash: 6ab80d0e0f42b0f74f19f9bcda43befaaf2a315af7206c2ebd77fed9bc71bf92<br>
Message ID: \<199606280620.XAA24528@cygnus.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-06-29 02:18:25 UTC<br>
Raw Date: Sat, 29 Jun 1996 10:18:25 +0800<br>

## Raw message

```
{% raw  %}From: Bill Stewart <stewarts@ix.netcom.com>
Date: Sat, 29 Jun 1996 10:18:25 +0800
To: Steve O <privsoft@ix.netcom.com>
Subject: Re: Crack for DOS
Message-ID: <199606280620.XAA24528@cygnus.com>
MIME-Version: 1.0
Content-Type: text/plain


At 06:17 PM 6/27/96 -0700, you wrote:
>2. If you were looking to compare single key block ciphers like Blowfish,
>DES, 3xDES etc. Which one would be considered the best for implementation in
>a software security package, assuming maximal key lengths irreverant of the
>governmental restrictions.

"Best" really depends on your criteria for goodness....

DES has been thoroughly explored, and people have a good idea of how
strong it is and how easy it is to implement well in software.
It's not strong enough (you can do a bit better than 2**55 brute force tries,
and 2**55 isn't enough given modern computers), but you can take care 
of that by using Triple DES, preferably the 3-key form, which
is strong enough for the forseeable future.  It's also annoyingly
slow in software form, having been designed for bit-twiddling hardware,
but there are well-optimized versions on the usual archive servers.

Blowfish is new, so perhaps there are flaws that 10-20 years of analysis
will find.  But it's pretty good - it's small, fast in software,
and has an annoyingly slow key-schedule which makes it difficult to
use brute-force crackers on.  It's got variable key lengths.

RC4 and RC5 are also new, fast, have variable key lengths, and appear to
be quite strong if used with adequate choices of parameters.
RC5 is patented; RC4 was a trade secret, since leaked, and you may
get flak for using the _name_ RC4 in a commercial product.
40-bit keys make it exportable but easily brute-forced;
128-bit keys are quite strong.

#				Thanks;  Bill
# Bill Stewart +1-415-442-2215 stewarts@ix.netcom.com
# http://www.idiom.com/~wcs
#				Distract Authority!





{% endraw %}
```

## Thread

+ Return to [June 1996](/archive/1996/06)

+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/authors/bill_stewart_stewarts_at_ix_netcom_com_)"

+ 1996-06-29 (Sat, 29 Jun 1996 10:18:25 +0800) - Re: Crack for DOS - _Bill Stewart \<stewarts@ix.netcom.com\>_

