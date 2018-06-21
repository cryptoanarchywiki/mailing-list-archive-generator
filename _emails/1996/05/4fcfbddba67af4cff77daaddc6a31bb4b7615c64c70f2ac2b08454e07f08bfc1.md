---
layout: default
---

# 1996-05-06 - Re: WWW proxies?

## Header Data

From: Dan McGuirk \<mcguirk@indirect.com\><br>
To: unicorn@schloss.li<br>
Message Hash: 4fcfbddba67af4cff77daaddc6a31bb4b7615c64c70f2ac2b08454e07f08bfc1<br>
Message ID: \<Pine.BSD/.3.91.960505222735.24544H-100000@bud.indirect.com\><br>
Reply To: \<v02120d03adb27fe340c9@[192.0.2.1]\><br>
UTC Datetime: 1996-05-06 09:33:08 UTC<br>
Raw Date: Mon, 6 May 1996 17:33:08 +0800<br>

## Raw message

```
{% raw  %}From: Dan McGuirk <mcguirk@indirect.com>
Date: Mon, 6 May 1996 17:33:08 +0800
To: unicorn@schloss.li
Subject: Re: WWW proxies?
In-Reply-To: <v02120d03adb27fe340c9@[192.0.2.1]>
Message-ID: <Pine.BSD/.3.91.960505222735.24544H-100000@bud.indirect.com>
MIME-Version: 1.0
Content-Type: text/plain


On Sun, 5 May 1996, Lucky Green wrote:
> At 0:30 5/5/96, Lou Poppler wrote:
> >On Fri, 26 Apr 1996 19:13:06 -0400 (EDT),
> >Black Unicorn <unicorn@schloss.li> wrote:
> >}
> >} Has anyone developed such a beast yet?

Here's a simple one in 3 lines of perl.  It only supports HTTP GET, and 
it ignores all of the MIME headers on the original request.  It requires the 
LWP perl module, but the RSA code requires dc, so I guess it's fair :)

#!/usr/bin/perl5 --# HTTP proxy, GET/http only;  usage: 'lwp-proxy <port>'
use LWP::Simple;sub w{wait;}$SIG{'CHLD'}='w';$SIG{'CLD'}='w';socket(S,2,1,6);
bind(S,pack(Sna4x8,2,$ARGV[0]));listen(S,5);while(1){accept(N,S);if(!fork){
open(STDERR,">&N");chop($r=<N>);$r=~s/^GET //i;select(N);getprint($r);exit;}}  




{% endraw %}
```

## Thread

+ Return to [May 1996](/archive/1996/05)

+ 1996-05-05 (Mon, 6 May 1996 04:05:42 +0800) - [Re: WWW proxies?](/archive/1996/05/b427be03f3690f27783379f9a5e001162f9011dc987d7de5b3cafc897b2c2f9a) - _shamrock@netcom.com (Lucky Green)_
  + 1996-05-05 (Mon, 6 May 1996 06:50:13 +0800) - [Re: WWW proxies?](/archive/1996/05/bb0bb2cbeb24a562d658fc6058cc9dbf40b12ab58a64eb170dc7e92f1621cb6a) - _"Mark M." \<markm@voicenet.com\>_
  + 1996-05-06 (Mon, 6 May 1996 17:33:08 +0800) - Re: WWW proxies? - _Dan McGuirk \<mcguirk@indirect.com\>_
  + 1996-05-07 (Tue, 7 May 1996 12:14:01 +0800) - [Re: WWW proxies?](/archive/1996/05/5d9847f24b9e1fa9e36bf02c77b1145d805ce9257eb2209e9b38c50000f2f072) - _sameer \<sameer@c2.org\>_

