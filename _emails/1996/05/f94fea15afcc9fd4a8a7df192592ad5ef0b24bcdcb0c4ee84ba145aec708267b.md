---
layout: default
---

# 1996-05-29 - Re: Layman's explanation for limits on escrowed encryption ...

## Header Data

From: "Mark M." \<markm<span>@</span>voicenet.com\><br>
To: Andrew Loewenstern \<andrew_loewenstern@il.us.swissbank.com\><br>
Message Hash: f94fea15afcc9fd4a8a7df192592ad5ef0b24bcdcb0c4ee84ba145aec708267b<br>
Message ID: \<Pine.LNX.3.93.960528160536.176B-100000@gak\><br>
Reply To: \<9605281800.AA00525@ch1d157nwk\><br>
UTC Datetime: 1996-05-29 01:13:43 UTC<br>
Raw Date: Wed, 29 May 1996 09:13:43 +0800<br>

## Raw message

```
{% raw  %}From: "Mark M." <markm@voicenet.com>
Date: Wed, 29 May 1996 09:13:43 +0800
To: Andrew Loewenstern <andrew_loewenstern@il.us.swissbank.com>
Subject: Re: Layman's explanation for limits on escrowed encryption ...
In-Reply-To: <9605281800.AA00525@ch1d157nwk>
Message-ID: <Pine.LNX.3.93.960528160536.176B-100000@gak>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

On Tue, 28 May 1996, Andrew Loewenstern wrote:

> Mark M. <markm@voicenet.com> writes:
> >  The normal key-length recommendation was 96 bits.  64 bits
> >  and 80 bits are equivalent to 512 bits and 768 bits respectively.
> >  I would guess that a 1024-bit key is about as strong as an
> >  96-bit key.  The first two numbers are from _Applied
> >  Cryptography_; my estimate is an extrapolation from the data
> >  = in AC.
> 
> These number should be qualified with the date on which the estimate was  
> determined.  New factoring techniques increase the number of RSA key bits  
> required to make factoring work equivalent to a given brute-force search.
> 
> Also, I would think that the NFS makes 512 bit RSA key factoring easier than  
> brute-forcing 64-bits of key space...

Quite true.  These estimates were made in 1995 so they are probably still
pretty accurate.  The rate at which factoring time decreases is greater than
the rate at which brute-force time decreases.  As to your claim that factoring
a 512 bit number is easier than bruting a 64-bit key space, it is not feasible
for anyone except maybe the NSA to do either of these.  I have heard that an
effort similar to that of factoring RSA 127 will be launched against a 512-
bit modulus.  I think that the difficulty is about equal to that of brute-
forcing a 64-bit key.

- -- Mark

=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
markm@voicenet.com              | finger -l for PGP key 0xe3bf2169
http://www.voicenet.com/~markm/ | d61734f2800486ae6f79bfeb70f95348
((2b) || !(2b))                 | Old key now used only for signatures
"The concept of normalcy is just a conspiracy of the majority" -me


-----BEGIN PGP SIGNATURE-----
Version: 2.6.3
Charset: noconv

iQCVAwUBMatd7bZc+sv5siulAQHZZAP/eyguOKHDmfYtVEr7JVH0jxuTRVWdWDxJ
ICEuHrhKnF0xG3kaBirOMtvZjnga90cFRk++pEv/zbAS0qyEoizA1YxnKUQrqHn5
emuYf+lbm83fzBBOcKwdspoSg8W25TTtJIH2BX7JpNiyVzfco7DcHJOPxlDxspGZ
LgUf7G9L4vI=
=uO8h
-----END PGP SIGNATURE-----




{% endraw %}
```

## Thread

+ Return to [May 1996](/archive/1996/05)

+ Return to "[Andrew Loewenstern <andrew_loewenstern<span>@</span>il.us.swissbank.com>](/authors/andrew_loewenstern_andrew_loewenstern_at_il_us_swissbank_com_)"
+ Return to "["E. ALLEN SMITH" <EALLENSMITH<span>@</span>ocelot.Rutgers.EDU>](/authors/e_allen_smith_eallensmith_at_ocelot_rutgers_edu_)"
+ Return to "["Mark M." <markm<span>@</span>voicenet.com>](/authors/mark_m__markm_at_voicenet_com_)"

+ 1996-05-25 (Sat, 25 May 1996 15:57:51 +0800) - [Re: Layman's explanation for limits on escrowed encryption ...](/archive/1996/05/7266b6edcb9504b039d04fbed00ae1c88d0c0a1b4d0abeb7ead8e4aa0c913f50) - _"E. ALLEN SMITH" \<EALLENSMITH@ocelot.Rutgers.EDU\>_
  + 1996-05-28 (Tue, 28 May 1996 13:50:10 +0800) - [Re: Layman's explanation for limits on escrowed encryption ...](/archive/1996/05/18db79102d7cdeefab9567c47d33d893e10d45315a60b541601b61e186d9ada7) - _"Mark M." \<markm@voicenet.com\>_
    + 1996-05-29 (Wed, 29 May 1996 08:15:58 +0800) - [Re: Layman's explanation for limits on escrowed encryption ...](/archive/1996/05/6d7bbaedc8b5d791e25448fa722383a7be71ef0cd974889058403f71a58935a8) - _Andrew Loewenstern \<andrew_loewenstern@il.us.swissbank.com\>_
      + 1996-05-29 (Wed, 29 May 1996 09:13:43 +0800) - Re: Layman's explanation for limits on escrowed encryption ... - _"Mark M." \<markm@voicenet.com\>_

