---
layout: default
---

# 1995-12-30 - Re: blind validation

## Header Data

From: futplex<span>@</span>pseudonym.com (Futplex)<br>
To: cypherpunks@toad.com (Cypherpunks Mailing List)<br>
Message Hash: f68d0bd8a00d2ef3adf62bc0ffa1cbd9be21ac7f6eb9b6e484a453a7bfb98930<br>
Message ID: \<199512300908.EAA07360@opine.cs.umass.edu\><br>
Reply To: \<199512281849.MAA08259@proust.suba.com\><br>
UTC Datetime: 1995-12-30 09:23:09 UTC<br>
Raw Date: Sat, 30 Dec 1995 17:23:09 +0800<br>

## Raw message

```
{% raw  %}From: futplex@pseudonym.com (Futplex)
Date: Sat, 30 Dec 1995 17:23:09 +0800
To: cypherpunks@toad.com (Cypherpunks Mailing List)
Subject: Re: blind validation
In-Reply-To: <199512281849.MAA08259@proust.suba.com>
Message-ID: <199512300908.EAA07360@opine.cs.umass.edu>
MIME-Version: 1.0
Content-Type: text/plain


Alex Strasheim writes:
[discussion and assumptions liberally elided]
> 1.   Alice initiates a transaction with Bob.  (Perhaps by asking
>      him for a file.)
> 
> 2.   Bob generates a random number and sends it back to Alice.
> 
> 3.   Alice blinds Bob's number and sends it to Trent, along with
>      proof of her validatability.
> 
> 4.   Trent checks Alice's proof, signs the blinded number, and
>      then returns it to Alice.
> 
> 5.   Alice unblinds Bob's number, then sends it to Bob.
> 
> 6.   Bob checks Trent's signature and makes sure that the number
>      he recieved matches the one he sent out.  Then Bob processes
>      Alice's transaction.
> 
> If Bob always follows this protocol, he can prove to Sam that
> he's followed the law.  Alice remains anonymous.  Alice can still
> transfer the file, but she has to give it away herself:  she
> can't give away the ability to get it directly from Bob without
> giving away the ability to prove Aliceness to Trent.  

I'm not convinced that your last point is true. It appears that the signed
Bobnet-access-number is still just a transferrable ticket. Charlie can
place an order with Bob, forward the Bobnet-access-number to Alice, wait for
Alice & Trent to do the blinding & signing tango, forward the signed Bobnet-
access-number to Bob, and get the goods from Bob.
  
Charlie can't use the signed Bobnet-access-number to prove to Trent
that he's Alice. In fact, since it's unblinded, Charlie can't even prove
that he's linked to a particular validation performed by Trent. (If Alice
foolishly gave him the blinded version too, he could show that he shares
Alice's knowledge about this validation.) 

[...]
> The main problems that I can see with this protocol are:
> 
> 1.   It's vulernable to traffic analysis.
> 2.   Sam has to trust Trent, which he may be unwilling to do.
> 3.   You can infer stuff about Alice from the kinds of requests
>      she makes of Trent.  Someone who always asks Trent for proof
>      that he's not a felon might tag himself as a person who buys
>      a lot of guns or ammunition, for example.

3. is OK as long as Alice trusts Trent. The trick is selecting a Trent
trusted by both Alice and Sam ;)

-Futplex	<futplex@pseudonym.com>




{% endraw %}
```

## Thread

+ Return to [December 1995](/archive/1995/12)

+ Return to "[Alex Strasheim <alex<span>@</span>proust.suba.com>](/authors/alex_strasheim_alex_at_proust_suba_com_)"
+ Return to "[Alex Strasheim <cp<span>@</span>proust.suba.com>](/authors/alex_strasheim_cp_at_proust_suba_com_)"
+ Return to "[futplex<span>@</span>pseudonym.com (Futplex)](/authors/futplex_at_pseudonym_com_futplex_)"

+ 1995-12-29 (Fri, 29 Dec 1995 13:00:08 +0800) - [blind validation](/archive/1995/12/ff055af84b58ac48c1251f8c4499d4a13e14c65b6a7f760fe7ce8186a87a677b) - _Alex Strasheim \<alex@proust.suba.com\>_
  + 1995-12-30 (Sat, 30 Dec 1995 17:23:09 +0800) - Re: blind validation - _futplex@pseudonym.com (Futplex)_
    + 1995-12-30 (Sun, 31 Dec 1995 04:33:56 +0800) - [Re: blind validation](/archive/1995/12/35926491bbd2bb7183ef96e8ceabc460b3cbfe96a08cb616a2080b6701933bf9) - _Alex Strasheim \<cp@proust.suba.com\>_

