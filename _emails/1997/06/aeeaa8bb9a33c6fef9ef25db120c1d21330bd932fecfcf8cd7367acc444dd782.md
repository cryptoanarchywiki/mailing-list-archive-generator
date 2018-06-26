---
layout: default
---

# 1997-06-21 - Re: Party on IRC

## Header Data

From: Bill Stewart \<stewarts<span>@</span>ix.netcom.com\><br>
To: Robert Hettinga \<rah@shipwright.com\><br>
Message Hash: aeeaa8bb9a33c6fef9ef25db120c1d21330bd932fecfcf8cd7367acc444dd782<br>
Message ID: \<3.0.2.32.19970621023432.0077a4ac@popd.ix.netcom.com\><br>
Reply To: \<v0302093bafd0130a7fac@[139.167.130.247]\><br>
UTC Datetime: 1997-06-21 09:50:03 UTC<br>
Raw Date: Sat, 21 Jun 1997 17:50:03 +0800<br>

## Raw message

```
{% raw  %}From: Bill Stewart <stewarts@ix.netcom.com>
Date: Sat, 21 Jun 1997 17:50:03 +0800
To: Robert Hettinga <rah@shipwright.com>
Subject: Re: Party on IRC
In-Reply-To: <v0302093bafd0130a7fac@[139.167.130.247]>
Message-ID: <3.0.2.32.19970621023432.0077a4ac@popd.ix.netcom.com>
MIME-Version: 1.0
Content-Type: text/plain



>Robert Hettinga <rah@shipwright.com> writes:
>>Is there an encrypted IRC available?
>>If not, shouldn't there be?
>>Is such a thing even possible?

You'd have to think about what you wanted it to do,
but it should be quite doable.  IRC is normally for sharing
conversations between an amorphous, changing bunch of people,
which isn't really a standard thing to do with crypto.  
But I can see several basic models:
0) Just Speak Finnish :-)
1) Two-person, with Diffie-Hellman key exchange
2) N-person shared-key - you'd probably use RSA to give the session key
to each new participant, or use PGP to do it.
3) N person, one key per sender, shared as above.
4) Ignore the application layer, and build the crypto as an IPsec tunnel.
5) Ignore the IRC protocols, and build a similar conversation server
using web forms and SSL.

Some tools you'd want`for 1-3:
a) Convenient cut&paste between the IRC makes integrating things easier,
such as key exchange, e.g. drop in a PGP message with today's key.

b) The ability to mix encrypted and unencrypted messages, 
so it's easier to do things like join the channel and negotiate keys.

c) A crypto operating mode that doesn't depend on sequence -
probably a line basis is about right.  ECB mode is boring and unsafe,
but you could use a session key (distributed with RSA/DH/etc.) 
to encrypt a per-line nonce key, and encrypt the line with the nonce,
transmitting "encryptednonce, encryptedline" for each line of data.

Perhaps this is less secure (?), but can you do something like
linekey = Hash( Hash(sessionkey, nonce), sessionkey ) 
transmitting "nonce, encryptedline"?  This would let you use a hash
instead of a symmetric crypto for the key on each line,
and might make it more convenient to choose a stream cypher such as RC4/160 
instead of a slower block cypher such as IDEA or DES for the line encryption.



#			Thanks;  Bill
# Bill Stewart, +1-415-442-2215 stewarts@ix.netcom.com
# You can get PGP outside the US at ftp.ox.ac.uk/pub/crypto/pgp
#   (If this is a mailing list or news, please Cc: me on replies.  Thanks.)





{% endraw %}
```

## Thread

+ Return to [June 1997](/archive/1997/06)

+ Return to "[3umoelle<span>@</span>informatik.uni-hamburg.de (Ulf =?iso-8859-1?Q?M=F6ller?=)](/author/3umoelle_at_informatik_unihamburg_de_ulf_iso88591qmf6ller_)"
+ Return to "[Bill Stewart <stewarts<span>@</span>ix.netcom.com>](/author/bill_stewart_stewarts_at_ix_netcom_com_)"
+ Return to "[iang<span>@</span>cs.berkeley.edu (Ian Goldberg)](/author/iang_at_cs_berkeley_edu_ian_goldberg_)"
+ Return to "[janke<span>@</span>unixg.ubc.ca (Leonard Janke)](/author/janke_at_unixg_ubc_ca_leonard_janke_)"
+ Return to "["John A. Perry" <perry<span>@</span>alpha.jpunix.com>](/author/john_a_perry_perry_at_alpha_jpunix_com_)"
+ Return to "[Kevin L Prigge <Kevin.L.Prigge-2<span>@</span>tc.umn.edu>](/author/kevin_l_prigge_kevin_l_prigge2_at_tc_umn_edu_)"
+ Return to "[Lucky Green <shamrock<span>@</span>netcom.com>](/author/lucky_green_shamrock_at_netcom_com_)"
+ Return to "[Robert Hettinga <rah<span>@</span>shipwright.com>](/author/robert_hettinga_rah_at_shipwright_com_)"

+ 1997-06-20 (Fri, 20 Jun 1997 11:09:05 +0800) - [Party on IRC](/archive/1997/06/d0a8e573f9db5e0356a89d041cc3599c93facb11febb83c3e43c29640fa12dd9) - _Lucky Green \<shamrock@netcom.com\>_
  + 1997-06-20 (Fri, 20 Jun 1997 20:12:14 +0800) - [Re: Party on IRC](/archive/1997/06/111e206c3b7f15b9cee12c7dfdcdd6c0e20fa6c015b76035faac1063dbcff3c9) - _Robert Hettinga \<rah@shipwright.com\>_
    + 1997-06-21 (Sat, 21 Jun 1997 10:03:21 +0800) - [Re: Party on IRC](/archive/1997/06/1e148c58465cdbde266005d6eca6fe2c1fc580f31eca284584b2d0c57402a51c) - _3umoelle@informatik.uni-hamburg.de (Ulf =?iso-8859-1?Q?M=F6ller?=)_
    + 1997-06-21 (Sat, 21 Jun 1997 17:50:03 +0800) - Re: Party on IRC - _Bill Stewart \<stewarts@ix.netcom.com\>_
      + 1997-06-22 (Sun, 22 Jun 1997 16:15:30 +0800) - [Re: Party on IRC](/archive/1997/06/2436b560afeced443811d47f9967a507ba6620c90490446f3c1466e3dc2ee55d) - _Bill Stewart \<stewarts@ix.netcom.com\>_
      + 1997-06-22 (Sun, 22 Jun 1997 18:45:18 +0800) - [Re: Party on IRC](/archive/1997/06/80ac4c51b41e444a322d0873a3b85e2066bd2e8de0e4d8634f99c364db1859c7) - _"John A. Perry" \<perry@alpha.jpunix.com\>_
      + 1997-06-22 (Mon, 23 Jun 1997 00:06:51 +0800) - [Re: Party on IRC](/archive/1997/06/331418e16360b2bcf3d6d882f718899576f97711c41e27b293ad5ea8ae934d00) - _iang@cs.berkeley.edu (Ian Goldberg)_
    + 1997-06-21 (Sat, 21 Jun 1997 21:41:59 +0800) - [Re: Party on IRC](/archive/1997/06/3f60bf60dc7d1976574b9a8c5049d686261ae27ef1ed4f26d07a35fb2096c6ef) - _janke@unixg.ubc.ca (Leonard Janke)_
      + 1997-06-23 (Tue, 24 Jun 1997 05:59:14 +0800) - [Re: Party on IRC](/archive/1997/06/ddac12b550b40d318d2ae00027b87e09842068634ec0ae6e234205a115779c0d) - _Kevin L Prigge \<Kevin.L.Prigge-2@tc.umn.edu\>_

