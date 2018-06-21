---
layout: default
---

# 1998-01-29 - Chaining ciphers

## Header Data

From: Tim May \<tcmay@got.net\><br>
To: cypherpunks@Algebra.COM<br>
Message Hash: 6daf91863278dda1bdebe5dc9d588977bd85e1b8e05d9dfe6b0d9fef3fb09ebc<br>
Message ID: \<v03102806b0f599c3ba80@[207.167.93.63]\><br>
Reply To: \<9801290026.AA13035@mentat.com\><br>
UTC Datetime: 1998-01-29 02:36:23 UTC<br>
Raw Date: Thu, 29 Jan 1998 10:36:23 +0800<br>

## Raw message

```
{% raw  %}From: Tim May <tcmay@got.net>
Date: Thu, 29 Jan 1998 10:36:23 +0800
To: cypherpunks@Algebra.COM
Subject: Chaining ciphers
In-Reply-To: <9801290026.AA13035@mentat.com>
Message-ID: <v03102806b0f599c3ba80@[207.167.93.63]>
MIME-Version: 1.0
Content-Type: text/plain



At 4:26 PM -0800 1/28/98, Jim Gillogly wrote:

>Doesn't seem terribly likely.  Typically ciphers will look strong until
>someone discovers a chink.  The chink will sometimes lead to a serious
>break, but not always, and not always quickly -- but at that point the
>cipher looks weak.  Your best chance at encrypting stuff that needs a
>long shelf life is with a cipher that's had a lot of analysis and
>plenty of intrinsic key, like 3DES.

Carl Ellison talks about his strategy for chaining several ciphers.

I'm surprised more emphasis isn't given to doing this. For example, suppose
one chains 3DES, Blowfish, MISTY, IDEA, and GHOST together (I haven't
checked Schneier on these, but you all presumably get the idea). Then if
any one of these ciphers is shown to be weak, the overall chain remains
strong. The overall chain is as strong as its strongest link, not its
weakest link.

I don't think 3DES is weak, but chaining-in additional ciphers can't hurt.
(Just a minor slowdown in encipherment speed, presumably not important for
some critical uses.)

-- Tim May

The Feds have shown their hand: they want a ban on domestic cryptography
---------:---------:---------:---------:---------:---------:---------:----
Timothy C. May              | Crypto Anarchy: encryption, digital money,
ComSec 3DES:   408-728-0152 | anonymous networks, digital pseudonyms, zero
W.A.S.T.E.: Corralitos, CA  | knowledge, reputations, information markets,
Higher Power: 2^2,976,221   | black markets, collapse of governments.
"National borders aren't even speed bumps on the information superhighway."







{% endraw %}
```

## Thread

+ Return to [January 1998](/archive/1998/01)

+ 1998-01-29 (Thu, 29 Jan 1998 08:34:07 +0800) - [Re: Predicting cipher life / NSA rigged DES? / Destroying encrypted data (Tangent to Re: Burning papers)](/archive/1998/01/fe6e4878233c097937e79ebf7ab35b1bfcb773a96c7c398461ddce41e166668d) - _jim@mentat.com (Jim Gillogly)_
  + 1998-01-29 (Thu, 29 Jan 1998 10:36:23 +0800) - Chaining ciphers - _Tim May \<tcmay@got.net\>_
  + 1998-01-31 (Sat, 31 Jan 1998 09:31:02 +0800) - [Re: Predicting cipher life / NSA rigged DES? / Destroying encrypted data (Tangent to Re: Burning papers)](/archive/1998/01/be3c09e1db2911e99952a3a5ef2a170215189cf71e64c1ece73aa69986799278) - _"Uhh...this is Joe [Randall Farmer]" \<rfarmer@HiWAAY.net\>_
  + 1998-01-31 (Sat, 31 Jan 1998 10:13:49 +0800) - [Re: Predicting cipher life / NSA rigged DES? ...](/archive/1998/01/0cbad4028a4b1037870504d7e98612b0e5050067c57c37f0db142e7e29dedd47) - _Tim May \<tcmay@got.net\>_
    + 1998-01-31 (Sun, 1 Feb 1998 00:23:48 +0800) - [Re: Predicting cipher life / NSA rigged DES? ...](/archive/1998/01/b44ed46083952669727d39a64b4926c20de3ca00bd9ed2e26d8adc8c0d1a80fd) - _"Uhh...this is Joe [Randall Farmer]" \<rfarmer@HiWAAY.net\>_

