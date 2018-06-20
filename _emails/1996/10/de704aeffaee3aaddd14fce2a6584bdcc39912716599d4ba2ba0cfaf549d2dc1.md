---
layout: default
---

# 1996-10-18 - Re: DES cracker.

## Header Data

From: "Geoffrey C. Grabow" \<gcg@pb.net\><br>
To: Gary Howland \<gary@systemics.com\><br>
Message Hash: de704aeffaee3aaddd14fce2a6584bdcc39912716599d4ba2ba0cfaf549d2dc1<br>
Message ID: \<3.0b36.32.19961018101502.0069a5e4@mail.pb.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-10-18 14:18:16 UTC<br>
Raw Date: Fri, 18 Oct 1996 07:18:16 -0700 (PDT)<br>

## Raw message

```
{% raw  %}From: "Geoffrey C. Grabow" <gcg@pb.net>
Date: Fri, 18 Oct 1996 07:18:16 -0700 (PDT)
To: Gary Howland <gary@systemics.com>
Subject: Re: DES cracker.
Message-ID: <3.0b36.32.19961018101502.0069a5e4@mail.pb.net>
MIME-Version: 1.0
Content-Type: text/plain


At 13:54 10/18/96 +0200, Gary Howland wrote:
>Geoffrey C. Grabow wrote:
>> 
>
>> Tell me what you need.  A large part of my job is providing hardware
>> security modules to banks to secure (among other things) their ATM networks
>> (Automated Teller MAchines, not Async Transfer Mode).  Do you need PIN
>> encryption formats, transmission message protocols, or what?  Just LMK.
>
>It would be nice to get some confirmation that PINs are generated using
>a DES encryption of the account number.
>
Actually, there are several methods.  The most common one by far is called
IBM3624.  That uses 12 digits of the Primary Account Number (PAN), which in
most cases is the card number, and encrypts it with DES.  That result is
then "decimalized" to change all hex letters to numbers.  The first n
digits of that result are then used to perform a MOD10 subtract from the
customers selected PIN.  That result is called an offset and is stored on
track 2 of the card, the bank's database or both.

 
                                                     G.C.G.

 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 | Geoffrey C. Grabow       |      Great people talk about ideas.       |
 | Oyster Bay, New York     |     Average people talk about things.     |
 | gcg@pb.net               |      Small people talk about people.      |
 |----------------------------------------------------------------------|
 |     PGP 2.6.2 public key available at http://www.pb.net/~wizard      |
 |          and on a plethora of key servers around the world.          |
 |                          Key ID = 0E818EC1                           |
 |   Fingerprint =  A6 7B 67 D7 E9 96 37 7D  E7 16 BD 5E F4 5A B2 E4    |
 |----------------------------------------------------------------------|
 | That which does not kill us, makes us stranger.   - Trevor Goodchild |
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~




{% endraw %}
```

## Thread

+ Return to [October 1996](/archive/1996/10)

+ 1996-10-18 (Fri, 18 Oct 1996 07:18:16 -0700 (PDT)) - Re: DES cracker. - _"Geoffrey C. Grabow" \<gcg@pb.net\>_

