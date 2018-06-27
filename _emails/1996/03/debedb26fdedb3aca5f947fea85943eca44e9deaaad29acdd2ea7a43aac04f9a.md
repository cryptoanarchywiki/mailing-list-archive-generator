---
layout: default
---

# 1996-03-12 - Re: PGP reveals  the key ID of the recipient of encrypted msg

## Header Data

From: John Pettitt \<jpp<span>@</span>software.net\><br>
To: "Robert A. Rosenberg" \<hal9001@panix.com\><br>
Message Hash: debedb26fdedb3aca5f947fea85943eca44e9deaaad29acdd2ea7a43aac04f9a<br>
Message ID: \<2.2.32.19960312003621.00b780f4@mail.software.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-03-12 06:34:22 UTC<br>
Raw Date: Tue, 12 Mar 1996 14:34:22 +0800<br>

## Raw message

```
{% raw  %}From: John Pettitt <jpp@software.net>
Date: Tue, 12 Mar 1996 14:34:22 +0800
To: "Robert A. Rosenberg" <hal9001@panix.com>
Subject: Re: PGP reveals  the key ID of the recipient of encrypted msg
Message-ID: <2.2.32.19960312003621.00b780f4@mail.software.net>
MIME-Version: 1.0
Content-Type: text/plain



>At 2:25 3/11/96, savron@world-net.sct.fr wrote:
>
>>I began testing PGP  a few days ago ( I'm a PGP newbie ) and I found
>>that it gives out the key ID of an encrypted message . From this you
>>can get the  identification of the recipient of the message , if it's
>>someone who has publicaly  distributed his  key (keyserver , homepage
>>...) . So even if you are unable to decode the message you  can find
>>who is the recipient of a given message . I think this is a big
>>privacy problem .
>

and "Robert A. Rosenberg" <hal9001@panix.com> replied:

>There is little that can be done about this. There must be something in the
>message to identify who it is intended to be read by. As someone else has
>stated, you can always set up private keys to be used to send to you that
>are different from your Public KeyID for cases where you want to hide your
>identity or that of the party you are communicating with.
>

I can see a case where one would want to broadcast a message (say on usenet)
with *no* indication of the intended recipient (not even a non registered
key-id).  It would seem to be easy enough to hack up something that does not
have key-IDs - to know if it's for you try decryption and if it works then
it was for you.  This does not scale well as the recipient must trial
decrypt all messages which could use *a lot* (tm) of CPU time.

John
John Pettitt, jpp@software.net
VP Engineering, CyberSource Corporation, 415 473 3065
 "Technology is a way of organizing the universe so that man
  doesn't have to experience it." - Max Frisch

PGP Key available at:
http://www-swiss.ai.mit.edu/htbin/pks-extract-key.pl?op=get&search=0xB7AA3705





{% endraw %}
```

## Thread

+ Return to [March 1996](/archive/1996/03)

+ Return to "[John Pettitt <jpp<span>@</span>software.net>](/authors/john_pettitt_jpp_at_software_net_)"

+ 1996-03-12 (Tue, 12 Mar 1996 14:34:22 +0800) - Re: PGP reveals  the key ID of the recipient of encrypted msg - _John Pettitt \<jpp@software.net\>_

