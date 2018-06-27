---
layout: default
---

# 1993-02-24 - Re: Crypto goals

## Header Data

From: Timothy Newsham \<newsham<span>@</span>wiliki.eng.hawaii.edu\><br>
To: fnerd@smds.com (FutureNerd Steve Witham)<br>
Message Hash: a4e8ccbf4dba5cbc52cb952fbf205a42be6c12fdb383cb6d5f0a73f657d34dbb<br>
Message ID: \<9302240821.AA27032@toad.com\><br>
Reply To: \<9302231806.AB16915@smds.com\><br>
UTC Datetime: 1993-02-24 08:21:07 UTC<br>
Raw Date: Wed, 24 Feb 93 00:21:07 PST<br>

## Raw message

```
{% raw  %}From: Timothy Newsham <newsham@wiliki.eng.hawaii.edu>
Date: Wed, 24 Feb 93 00:21:07 PST
To: fnerd@smds.com (FutureNerd Steve Witham)
Subject: Re: Crypto goals
In-Reply-To: <9302231806.AB16915@smds.com>
Message-ID: <9302240821.AA27032@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


> 
> Encrypted computing.  This is even harder than non-disassemblable code.
> The idea is that you couldn't even tell what happened to the data if you
> watched it compute, tried again with slightly different inputs, etc.
> I've heard that some restricted sort of encrypted computing is possible
> with an exponential time cost!
> 
> The main application I have in mind is a mix that would be trustworthy
> even if it was run by your worst enemies with the best computers in the
> world.
> 
> This seems impossible but I don't have proof.
> 
> -fnerd
> fnerd@smds.com (FutureNerd Steve Witham)
> 
> 
How can multiple keys be chosen?  The decryption key is needed
to execute the code, it can either be (1) built into the hardware
or (2) loaded in.  In #2, if its loaded in, it can be had before
it is loaded.  In #1,  how do you change keys?  only people who
know how to encrypt for that key can program the thing.  If a
public key scheme was used,  the processor could be built with
a private key inside, and you assemble and then encode in the
public key,  only the processor (and whoever else has the 
private key) can check the code.  Quite a bit of complexity, 
also how do you do encryption in small enough units for the
cpu to use?  How do you decrypt w/ random access any part
of the data?  If you choose too large blocks (ie. cache) how
do you keep enemy programs from grabbig already decrypted data?
obviously some data must go out as plaintext (for I/O)  then
you have to keep track of which data is to always remain crypted
and which needs to go to plaintext..   wow..  what a nightmare.
I think its probably possible...
sorry for the free-form :)






{% endraw %}
```

## Thread

+ Return to [February 1993](/archive/1993/02)

+ Return to "[fnerd<span>@</span>smds.com (FutureNerd Steve Witham)](/authors/fnerd_at_smds_com_futurenerd_steve_witham_)"
+ Return to "[Timothy Newsham <newsham<span>@</span>wiliki.eng.hawaii.edu>](/authors/timothy_newsham_newsham_at_wiliki_eng_hawaii_edu_)"

+ 1993-02-24 (Tue, 23 Feb 93 21:33:09 PST) - [Re: Crypto goals](/archive/1993/02/214537bedbda0306576e943526bfef927e9f546442ababe802af76024d6bc746) - _fnerd@smds.com (FutureNerd Steve Witham)_
  + 1993-02-24 (Wed, 24 Feb 93 00:21:07 PST) - Re: Crypto goals - _Timothy Newsham \<newsham@wiliki.eng.hawaii.edu\>_

