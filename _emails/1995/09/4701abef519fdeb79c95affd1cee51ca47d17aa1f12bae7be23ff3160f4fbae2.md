---
layout: default
---

# 1995-09-25 - New Netscape RNG

## Header Data

From: Ray Cromwell \<rjc<span>@</span>clark.net\><br>
To: cypherpunks@toad.com<br>
Message Hash: 4701abef519fdeb79c95affd1cee51ca47d17aa1f12bae7be23ff3160f4fbae2<br>
Message ID: \<199509250649.CAA27099@clark.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-09-25 06:49:16 UTC<br>
Raw Date: Sun, 24 Sep 95 23:49:16 PDT<br>

## Raw message

```
{% raw  %}From: Ray Cromwell <rjc@clark.net>
Date: Sun, 24 Sep 95 23:49:16 PDT
To: cypherpunks@toad.com
Subject: New Netscape RNG
Message-ID: <199509250649.CAA27099@clark.net>
MIME-Version: 1.0
Content-Type: text/plain




  I just glanced at the new Netscape RNG source. I don't really see
anything bad, but I haven't analyzed it. However, I'm curious
as to why variables like the username or the language locality
are used as sources of entropy. These seem to provide almost nil.
The username is going to be pretty much constant. In fact, even
the current directory which is used as a seed can't provide more
than a few bits of entropy. In all probability, the user
name will usually be the same, and so will the current directory
(and how many directories are there? 65,000 would only give you
16 bits of entropy, assuming you get a directory listing from the machine)
 
 I'm thinking from the standpoint of someone gathering data on someone
or some server to mount a specific attack. a "most common directories
on the macintosh" file for instance could be used to attack the
current directory method.

  Using those sources probably can't hurt, they just seemed
like odd choices, "grasping for straws" so to speak.

  Nevertheless, I would like to commend Netscape for releasing
the source code for public review. You guys are clearly an intelligent
company, in both your current developments, but also the way
you have handled this bad press.

-Ray

p.s. i hope you guys do a good internal review of your code to remove
buffer overflow bugs

 



{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ Return to "["David R. Conrad" <drc<span>@</span>russell.moore.com>](/authors/david_r_conrad_drc_at_russell_moore_com_)"
+ Return to "[jsw<span>@</span>neon.netscape.com (Jeff Weinstein)](/authors/jsw_at_neon_netscape_com_jeff_weinstein_)"
+ Return to "[Ray Cromwell <rjc<span>@</span>clark.net>](/authors/ray_cromwell_rjc_at_clark_net_)"

+ 1995-09-25 (Sun, 24 Sep 95 23:49:16 PDT) - New Netscape RNG - _Ray Cromwell \<rjc@clark.net\>_
  + 1995-09-25 (Mon, 25 Sep 95 00:32:57 PDT) - [Re: New Netscape RNG](/archive/1995/09/e6c1c76a1386e8d4687d17367063546d3a3263741ec83be41f3b2089752e9784) - _jsw@neon.netscape.com (Jeff Weinstein)_
  + 1995-09-26 (Tue, 26 Sep 95 04:57:51 PDT) - [Re: New Netscape RNG](/archive/1995/09/bdb99fb14a66e08f6873a2098ec75d11e285b85cadb170e6220889bbdc4b9b00) - _"David R. Conrad" \<drc@russell.moore.com\>_
  + 1995-09-27 (Tue, 26 Sep 95 17:50:03 PDT) - [Re: New Netscape RNG](/archive/1995/09/5123d0b4034d455fbed2b32943b91240a66c4988ff4feb770131186bbb5ab242) - _jsw@neon.netscape.com (Jeff Weinstein)_

