---
layout: default
---

# 1993-05-04 - tripple des

## Header Data

From: Timothy Newsham \<newsham<span>@</span>wiliki.eng.hawaii.edu\><br>
To: cypherpunks@toad.com<br>
Message Hash: ec9ead82c98bd99c1baa82f708abec5335a40cca458ddbe34c3aa9b3e3c7a07b<br>
Message ID: \<9305042013.AA25148@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-05-04 20:13:45 UTC<br>
Raw Date: Tue, 4 May 93 13:13:45 PDT<br>

## Raw message

```
{% raw  %}From: Timothy Newsham <newsham@wiliki.eng.hawaii.edu>
Date: Tue, 4 May 93 13:13:45 PDT
To: cypherpunks@toad.com
Subject: tripple des
Message-ID: <9305042013.AA25148@toad.com>
MIME-Version: 1.0
Content-Type: text/plain



Crypto question:
why was the following chosen for tripple DES :
   EN(DE(EN(data,k1),k2),k3);   

The encryption would involve passing data through IP,
then doing 16 rounds forward with k1,
(factoring out the IP-1 and IP)
then doing 16 rounds backwards with k2
(factoring out the next IP-1 and IP)
then doing 16 rounds forward with k3
then going through IP-1

How would this compare with
   EN(EN(EN(data,k1),k2),k3);

which goes through IP,  does 16 rounds each with k1, k2 then
k3, then IP-1 ?

The only difference is that the key scheduler rotates backwards
(or another interpretation keys used in reverse order) for the
second stage.

Does anyone know the rationale behind this?




{% endraw %}
```

## Thread

+ Return to [May 1993](/archive/1993/05)

+ Return to "[Joe Thomas <jthomas<span>@</span>access.digex.net>](/authors/joe_thomas_jthomas_at_access_digex_net_)"
+ Return to "[Timothy Newsham <newsham<span>@</span>wiliki.eng.hawaii.edu>](/authors/timothy_newsham_newsham_at_wiliki_eng_hawaii_edu_)"

+ 1993-05-04 (Tue, 4 May 93 13:13:45 PDT) - tripple des - _Timothy Newsham \<newsham@wiliki.eng.hawaii.edu\>_
  + 1993-05-04 (Tue, 4 May 93 14:18:38 PDT) - [Re: tripple des](/archive/1993/05/bff6e89482897a8e1e530e100056b183c91fb0365d27bdf9f8bbfc65597afa1e) - _Joe Thomas \<jthomas@access.digex.net\>_
    + 1993-05-04 (Tue, 4 May 93 14:31:52 PDT) - [Re: tripple des](/archive/1993/05/e2d9ce0a1e81e976719e72e9d961f3f0c2e175deb32eee68b8f3c6e689d007ef) - _Timothy Newsham \<newsham@wiliki.eng.hawaii.edu\>_

