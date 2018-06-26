---
layout: default
---

# 1995-07-28 - Re: Java, Netscape, OpenDoc, and Babel

## Header Data

From: Adam Shostack \<adam<span>@</span>bwh.harvard.edu\><br>
To: rjc@clark.net (Ray Cromwell)<br>
Message Hash: dd0b6c7cc62daedb7fc54e1f036e3e48abff5ca7ef3d614bc7e8efe547a38423<br>
Message ID: \<9507281941.AA10821@leonardo.bwh.harvard.edu\><br>
Reply To: \<199507281754.NAA11499@clark.net\><br>
UTC Datetime: 1995-07-28 19:41:57 UTC<br>
Raw Date: Fri, 28 Jul 95 12:41:57 PDT<br>

## Raw message

```
{% raw  %}From: Adam Shostack <adam@bwh.harvard.edu>
Date: Fri, 28 Jul 95 12:41:57 PDT
To: rjc@clark.net (Ray Cromwell)
Subject: Re: Java, Netscape, OpenDoc, and Babel
In-Reply-To: <199507281754.NAA11499@clark.net>
Message-ID: <9507281941.AA10821@leonardo.bwh.harvard.edu>
MIME-Version: 1.0
Content-Type: text/plain


Ray wrote, responding to me:

| > 	I suspect Ray is working in an environment less security
| > concious than Perry's.  Perry works on a lot of security-critical
| > applications where a lot of money is at stake.  If I were going to go
| > after financial institutions, I'd definetly look at which ones were
| > using Java, and see what I could upload into their systems.  Getting
| > copies of the recent files might be *very* informative.  I'd be
| > worried if I were at Solomon brothers.


|   If a business wants high security, they probably shouldn't be running
| anything but mail. Even allowing users ftp access is dangerous
| because someone could download a trojan horse. My college  took
| the /exec function out of IRC for this very reason. If data can 
| get  through a firewall by any means, DNS, mail, etc, it's possible to write
| some kind of program to send stolen information on those channels. Hell,
| there is a big enough problem with users bringing software from home
| into work and infecting company networks with viruses.

	FTP is available by mail.  So is web access.  Marcus Ranum
(formerly of TIS) has written a TCP/IP over SMTP. (He doesn't
distribute it.)

	The problem of securing a network in this environment is a
very difficult one.  Parts of it can be shown to be hard, although
partial solutions are possible.

	I suspect the risks are enhanced by easy to use clients, as is
the productivity of the workers.  Many experts recommend studying each
service and deciding whether or not to allow it based on a risk
assesment.  The size of Java makes it tough to evaluate, as does its
extensible nature.  I'm tempted to agree with Perry that its too big
and doesn't have enough fail-safes yet.  I'd be much happier if the
Java execution environment did a chroot() before running any code, and
code went to the executor through a one way funnel.  Making this
funnel truely one way limits the nifty things you can do with Java
substantially.

|   Once you actually browse some HotJava web pages with HotJava, the
| ordinary Web becomes static and boring. It's like the difference between
| ftp and Netscape, or TinyMUD and LambdaMOO. There's just so much
| potential, especially for crypto-clients. Because Java provides a
| single development platform, single execution environment, GUI, and
| network access.

	No argument here.  I think Java is way nifty, and might be
enough of a killer app for me to upgrade to a powerPC mac.

Adam


-- 
"It is seldom that liberty of any kind is lost all at once."
					               -Hume




{% endraw %}
```

## Thread

+ Return to [July 1995](/archive/1995/07)

+ Return to "[Adam Shostack <adam<span>@</span>bwh.harvard.edu>](/author/adam_shostack_adam_at_bwh_harvard_edu_)"
+ Return to "["Perry E. Metzger" <perry<span>@</span>imsi.com>](/author/perry_e_metzger_perry_at_imsi_com_)"
+ Return to "["Perry E. Metzger" <perry<span>@</span>panix.com>](/author/perry_e_metzger_perry_at_panix_com_)"
+ Return to "[Phil Fraering        <pgf<span>@</span>tyrell.net>](/author/phil_fraering_pgf_at_tyrell_net_)"
+ Return to "[Ray Cromwell <rjc<span>@</span>clark.net>](/author/ray_cromwell_rjc_at_clark_net_)"
+ Return to "[solman<span>@</span>MIT.EDU](/author/solman_at_mit_edu)"
+ Return to "[tcmay<span>@</span>sensemedia.net (Timothy C. May)](/author/tcmay_at_sensemedia_net_timothy_c_may_)"

+ 1995-07-28 (Thu, 27 Jul 95 23:23:31 PDT) - [Java, Netscape, OpenDoc, and Babel](/archive/1995/07/ada5bfd90cb2ef0cbb5558423143dd69cdaf83e18a692c92cb1e41b9e5be0cf8) - _tcmay@sensemedia.net (Timothy C. May)_
  + 1995-07-28 (Fri, 28 Jul 95 00:32:58 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/09a7e728b26e5213640f6f90da2ef4114842ba7a2bbaf369db1e6f22833ffba4) - _Ray Cromwell \<rjc@clark.net\>_
    + 1995-07-28 (Fri, 28 Jul 95 07:12:00 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/e24ed112c923a391dce9f2dfae06a6c3da7a6d9d4a467adfe3d3fb0048e1ee3d) - _"Perry E. Metzger" \<perry@imsi.com\>_
      + 1995-07-28 (Fri, 28 Jul 95 08:25:43 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/1531be13be86afb68f7b3d88b91bdba966403fe76251b9d8154de616c4677b03) - _solman@MIT.EDU_
        + 1995-07-28 (Fri, 28 Jul 95 08:30:53 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/d23c98bb22cee8a80ae8d78babf0dc6ac6035f50f7155e844566b10be298953d) - _"Perry E. Metzger" \<perry@imsi.com\>_
          + 1995-07-28 (Fri, 28 Jul 95 09:16:00 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/e2fff6da27ccac7b3cb01f757427bce255139a285e7b78a1abfe7838fabd78d5) - _solman@MIT.EDU_
            + 1995-07-28 (Fri, 28 Jul 95 09:33:40 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/d5531fa64e5b8f5b6384f22f7e659911e55c80ea3bb38aa7793e15a76db76303) - _"Perry E. Metzger" \<perry@imsi.com\>_
      + 1995-07-28 (Fri, 28 Jul 95 09:24:38 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/c25e4588b3c80b11ba8d735d8571754b672478369adea23426d99190526efdd4) - _Ray Cromwell \<rjc@clark.net\>_
        + 1995-07-28 (Fri, 28 Jul 95 09:37:06 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/9bb0f25f9863fc68c5e463b7297000c79840cad1335d128ce537130c4b9cbdf1) - _"Perry E. Metzger" \<perry@imsi.com\>_
          + 1995-07-28 (Fri, 28 Jul 95 10:03:03 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/cecf3d136f3ab41cefa7278859deae06015e9dd355d660355427cbed34912fd2) - _Ray Cromwell \<rjc@clark.net\>_
        + 1995-07-28 (Fri, 28 Jul 95 10:17:48 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/7b3685d8eab7187ed1b53ba7cce77e7dd5ac929931ce66d6d5237b7b15e08537) - _Adam Shostack \<adam@bwh.harvard.edu\>_
          + 1995-07-28 (Fri, 28 Jul 95 10:25:56 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/43f4c7dd40c7a469befaeaeeb8887977a3e67488c6511b77f774d37f7e6c224a) - _"Perry E. Metzger" \<perry@imsi.com\>_
          + 1995-07-28 (Fri, 28 Jul 95 10:54:29 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/3d3eb3ca1e3808d806a8adec3e910dc490fd2dc4f46009916812d248e78828c7) - _Ray Cromwell \<rjc@clark.net\>_
            + 1995-07-28 (Fri, 28 Jul 95 12:41:57 PDT) - Re: Java, Netscape, OpenDoc, and Babel - _Adam Shostack \<adam@bwh.harvard.edu\>_
      + 1995-07-28 (Fri, 28 Jul 95 13:07:53 PDT) - [Java, Netscape, OpenDoc, and Babel](/archive/1995/07/b2a2f11392999fc21b1815df31085f7b8b9c8a7e39fc4c835c93f67fafaca258) - _Phil Fraering        \<pgf@tyrell.net\>_
        + 1995-07-30 (Sun, 30 Jul 95 15:05:37 PDT) - [Re: Java, Netscape, OpenDoc, and Babel](/archive/1995/07/86110e1a4194cc91cc23d2f073e4fcbbdb1c0efdd714768ed23fc8bbfb036d08) - _"Perry E. Metzger" \<perry@panix.com\>_

