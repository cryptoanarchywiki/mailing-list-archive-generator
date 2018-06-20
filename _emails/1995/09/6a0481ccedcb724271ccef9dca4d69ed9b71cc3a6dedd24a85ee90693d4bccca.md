---
layout: default
---

# 1995-09-19 - Re: NYT on Netscape Crack

## Header Data

From: aba@dcs.exeter.ac.uk<br>
To: eay@mincom.oz.au<br>
Message Hash: 6a0481ccedcb724271ccef9dca4d69ed9b71cc3a6dedd24a85ee90693d4bccca<br>
Message ID: \<28592.9509191106@exe.dcs.exeter.ac.uk\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-09-19 11:12:01 UTC<br>
Raw Date: Tue, 19 Sep 95 04:12:01 PDT<br>

## Raw message

```
{% raw  %}From: aba@dcs.exeter.ac.uk
Date: Tue, 19 Sep 95 04:12:01 PDT
To: eay@mincom.oz.au
Subject: Re: NYT on Netscape Crack
Message-ID: <28592.9509191106@exe.dcs.exeter.ac.uk>
MIME-Version: 1.0
Content-Type: text/plain



Eric Young <eay@au.oz.mincom> writes:
> I will defend Netscapes code on the point about the RNG even though
> I have not seen any.  I assume the Netscape code is quite large and
> each release would have to pass various fuctionality tests.  How can
> you test that the RND seeding is wrong?  You have to actually look
> at the code, the number coming out are still random.  As of last
> week I was told by Mike_Spreitzer.PARC@xerox.com that the random
> number generator seed routine in my DES library was only copying in
> 4 bytes of passed data instead of 8.  Given des_cblock data;, it was
> 
> memcpy(init,data,sizeof(data));
> 
> it should have been
> 
> memcpy(init,data,sizeof(des_cblock));
> 
> Rather hard to notice unless you know that des_cblock is passed as a 
> pointer and even this can be compiler dependent.

Sure that's hard to notice, but what you describe was an accident, ie
the code wasn't working as you thought it was.

The netscape one by the sound of it, and the earlier posts of the
reverse-engineered ran no code, was working to spec, it was just a
dumb spec.

I felt sorry for netscape when they got chosen as the example of an
ITAR crippled app to break, the breakers intention obviously being to
tar ITAR, but some of the bad publicity rubbing off on netscape, who
were obviously fully aware of the weakness of 40 bit keys.

This one tho' sounds very much like due to sloppy design which is
inexcusable, especially given that they are going around selling the
128 bit RC4 browser to people who may have been relying on it, at it's
word, and presume the rest of the cryptographic system was up to
suitable standard to match 128 bit keys.

aka what's the point having 128 bit keys if you use a 32 bit, or 40
bit or 48 bit seed, which can be further narrowed with non-root access
to the machine, and even with external info leaked by the machine.

> The moral of the story I suppose is to be 
> paranoid about checking routines relating to RNG.

Well that is a valid, and very good moral, but the netscape story is a
different story I think, as they knew what their code was doing, and
somehow didn't think it was a problem, or didn't even pause to
consider the ran no generation security.  Reckon any bad publicity
they get out of this one is entirely their own fault.

The moral in netscapes story is that closed systems are bad news.
These things ideally need open review.  And of course designing things
with the expectation that they are secure with the *given* that the
full algorithm is known.

Real shame because the rest of the software is very innovative
compared to other browsers, and apparently good quality.  Also may be
a set back for net commerce, which is bad news.

Adam
--
Munitions-T home page:  http://www.obscura.com/~shirt/

#!/bin/perl -s-- -export-a-crypto-system-sig -RSA-3-lines-PERL
$m=unpack(H.$w,$m."\0"x$w),$_=`echo "16do$w 2+4Oi0$d*-^1[d2%Sa
2/d0<X+d*La1=z\U$n%0]SX$k"[$m*]\EszlXx++p|dc`,s/^.|\W//g,print
pack('H*',$_)while read(STDIN,$m,($w=2*$d-1+length($n)&~1)/2)





{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ 1995-09-19 (Tue, 19 Sep 95 04:12:01 PDT) - Re: NYT on Netscape Crack - _aba@dcs.exeter.ac.uk_
  + 1995-09-19 (Tue, 19 Sep 95 07:08:27 PDT) - [Re: NYT on Netscape Crack](/archive/1995/09/f7837d3b9cc2e5e5cc1bfb46f9317022523edf4d6ef9dd743b69d032366bc8ee) - _sameer \<sameer@c2.org\>_

