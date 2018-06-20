---
layout: default
---

# 1994-07-08 - Re: Mastercard, Visa, Access, Barclaycard, Amex, JCB ...

## Header Data

From: Ian Farquhar \<ifarqhar@laurel.ocs.mq.edu.au\><br>
To: jamiel@sybase.com (Jamie Lawrence)<br>
Message Hash: de0eaafca62bedfe4c7105e521f5103c564616a0aa9e3c8d1f06aeeedf7fd29c<br>
Message ID: \<199407080101.AA07281@laurel.ocs.mq.edu.au\><br>
Reply To: \<9407071722.AB05853@ralph.sybgate.sybase.com\><br>
UTC Datetime: 1994-07-08 01:03:10 UTC<br>
Raw Date: Thu, 7 Jul 94 18:03:10 PDT<br>

## Raw message

```
{% raw  %}From: Ian Farquhar <ifarqhar@laurel.ocs.mq.edu.au>
Date: Thu, 7 Jul 94 18:03:10 PDT
To: jamiel@sybase.com (Jamie Lawrence)
Subject: Re: Mastercard, Visa, Access, Barclaycard, Amex, JCB ...
In-Reply-To: <9407071722.AB05853@ralph.sybgate.sybase.com>
Message-ID: <199407080101.AA07281@laurel.ocs.mq.edu.au>
MIME-Version: 1.0
Content-Type: text/plain


>I believe modern card readers for at least MC/Visa use some form of
>encryption, but for backwards compatibility the central offices also
>work unencrypted. In the hotel I used to work in, the card reader
>certainly didn't encrypt.

My fiance regularly configures remote EFTPOS (Electronic Financial Transcation
at Point Of Sale) terminals from her job in the 24 hour answer centre of a
major bank in this state, and when she is doing so she reads a "public key" 
off the screen to for the vendor to key into the unit.  Sounds very much like 
some sort of assymetric session key exchange to me, and I'd lay money on the 
symmetric cipher behind that being DES.  Apparently there is also an 
Australian Standard for the ecryptographic exchange of pin numbers, and I 
know that DES is also sanctified in an AS (and recommended by DSD, who even 
now still consider DES "appropriate" for the banking industry).

						Ian.



{% endraw %}
```

## Thread

+ Return to [July 1994](/archive/1994/07)

+ 1994-07-07 (Thu, 7 Jul 94 10:24:32 PDT) - [Re: Mastercard, Visa, Access, Barclaycard, Amex, JCB ...](/archive/1994/07/7fc8536cf05eb9ad99b9ca4cbc73bd0764fb57739533337dc445c599942a7072) - _jamiel@sybase.com (Jamie Lawrence)_
  + 1994-07-08 (Thu, 7 Jul 94 18:03:10 PDT) - Re: Mastercard, Visa, Access, Barclaycard, Amex, JCB ... - _Ian Farquhar \<ifarqhar@laurel.ocs.mq.edu.au\>_

