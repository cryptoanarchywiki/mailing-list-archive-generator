---
layout: default
---

# 1993-08-20 - Blinded RSA signatures

## Header Data

From: nobody<span>@</span>shell.portal.com<br>
To: cypherpunks@toad.com<br>
Message Hash: 53bcd59ecc3a7437dbaae4239040dfaa5cfd4c5a89ec416eeabfa06cac84e36f<br>
Message ID: \<9308200544.AA15625@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-08-20 05:51:18 UTC<br>
Raw Date: Thu, 19 Aug 93 22:51:18 PDT<br>

## Raw message

```
{% raw  %}From: nobody@shell.portal.com
Date: Thu, 19 Aug 93 22:51:18 PDT
To: cypherpunks@toad.com
Subject: Blinded RSA signatures
Message-ID: <9308200544.AA15625@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


An excellent description of blinding and digital
cash, forwarded from sci.crypt:

In article <24924cINNg4c@network.ucsd.edu>, 
loki@sdphu3.ucsd.edu (Lance M Cottrell) writes:
 -----BEGIN PGP SIGNED MESSAGE-----
 Some time ago I read an article in Scientific American
 about using RSA and smart cards to achieve untraceable
 and unforgable electronic cash.  The system hinged on being
 able to "blind" a message which would be signed
 by the bank, and then the blinding would be removed
 without disturbing the signature.  The signed message
 would then decrypt to the original message, but the signer
 would not know what she had signed.  The article made no
 mention of how to do this "blinding".
 
 This morning I came up with a method which I would like
 comments upon.  First the notation
 
 ^ : exponentiation
 n : the bank's modulus (p*q in usual notation)
 e : the exponent used to encrypt the message sent
 	to the bank
 d : the exponent used to decrypt the bank's encryption.
 t : the text that you want signed.
 x : some random number with a multiplicative inverse mod n.
 y : the inverse of x mod n.
 c : the cipher text corresponding to t
 a : the blinded plain text
 b : the encrypted blinded text.
 
 Now the procedure.
 
 blind the plain text by
 	a = ((x^d) * t) mod n
 
 the bank encrypts a by
 	b = (a^e) mod n
 	  = ((((x^d)^e)mod n) * ((t^e)mod n)) mod n
 
 the blind is removed by multiplying through by y
 	since ((x^d)^e)mod n = (x^(d*e))mod n = x
 
 	c = y * b 
 	  = (y * x * ((t^e) mod n))mod n
 	  = (t^e) mod n
 
 
 The question is, can one find x and y such that
 (x*y) mod n = 1, and can the bank recover t when only given a.
 Also, please tell me if there is some fundamental error in
 my handeling of math mod n.
 
 Many thanks for any comments.  If anyone knows the method the
 original authors used, please post that as well.
 

Fine description of Chaum's blind signature protocol.  Your
math looks good.

It is easy to find y, given x and n, such that (x*y) mod n = 1,
(provided gcd(x,n)=1, as it is for most x ).
See Knuth Vol II section 4.5.2, or look up the extended
Euclid's algorithm in some good algorithms text.

The bank can not tell which t was signed via some a, since
for any t and a with t in the multiplicative group mod n,
there is some x such that a=x^d * t (mod n).

Thus (1)the procedure is tractable, (2)blind forgeries are 
only possible if RSA is weak, and (3)the "blind" is 
unconditionally secure.

Bryan Olson
olson@umbc.edu 





{% endraw %}
```

## Thread

+ Return to [August 1993](/archive/1993/08)

+ Return to "[Eric Hughes <hughes<span>@</span>soda.berkeley.edu>](/author/eric_hughes_hughes_at_soda_berkeley_edu_)"
+ Return to "[nobody<span>@</span>shell.portal.com](/author/nobody_at_shell_portal_com)"

+ 1993-08-20 (Thu, 19 Aug 93 22:51:18 PDT) - Blinded RSA signatures - _nobody@shell.portal.com_
  + 1993-08-20 (Fri, 20 Aug 93 11:31:34 PDT) - [Blinded RSA signatures](/archive/1993/08/613eb4cfd227867e672866b96d57eb48fb4bec5536e0508c824bf75bb04ae153) - _Eric Hughes \<hughes@soda.berkeley.edu\>_

