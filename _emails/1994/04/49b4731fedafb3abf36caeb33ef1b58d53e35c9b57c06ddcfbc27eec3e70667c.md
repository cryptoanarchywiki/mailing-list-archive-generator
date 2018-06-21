---
layout: default
---

# 1994-04-25 - Re: Wow, what a key!

## Header Data

From: "Perry E. Metzger" \<perry@snark.imsi.com\><br>
To: Ed Carp \<ecarp@netcom.com\><br>
Message Hash: 49b4731fedafb3abf36caeb33ef1b58d53e35c9b57c06ddcfbc27eec3e70667c<br>
Message ID: \<9404252120.AA05992@snark.imsi.com\><br>
Reply To: \<Pine.3.89.9404251427.A28811-0100000@netcom10\><br>
UTC Datetime: 1994-04-25 21:21:03 UTC<br>
Raw Date: Mon, 25 Apr 94 14:21:03 PDT<br>

## Raw message

```
{% raw  %}From: "Perry E. Metzger" <perry@snark.imsi.com>
Date: Mon, 25 Apr 94 14:21:03 PDT
To: Ed Carp <ecarp@netcom.com>
Subject: Re: Wow, what a key!
In-Reply-To: <Pine.3.89.9404251427.A28811-0100000@netcom10>
Message-ID: <9404252120.AA05992@snark.imsi.com>
MIME-Version: 1.0
Content-Type: text/plain



Ed Carp says:
> > As I've mentioned previously to people, there is an actual, live,
> > honest to god RFC for doing authentication and encryption of telnet
> > sessions, and the 4.4 BSD release contains the actual, honest to god
> > code. I would suggest looking at that before reinventing the wheel.
> > All sites ought to support it -- its a big win.
> 
> Well, last time I looked for it, I couldn't find it.  And doesn't it use DES?

The RFC doesn't specify an encryption system. Its been a while since
I've looked at the Cray code.

> What does it use for key exchange?

I don't believe the Cray implementation had a key exchange system, but
I believe that hooks for one were present in the protocol.

> I'd also have to hack it quite a bit to port it to linux, I think.

I believe Linux has a fairly conventional sockets library.

In any case, Jim Thompson has promised us an improved version of the
code, so I'd wait for his hacks...

Perry




{% endraw %}
```

## Thread

+ Return to [April 1994](/archive/1994/04)

+ 1994-04-25 (Mon, 25 Apr 94 11:31:26 PDT) - [Re: Wow, what a key!](/archive/1994/04/16826b802e4d7a09eea59fa61ae7556d16bbb17602f8e9558d1dee93dd3d3579) - _jim@Tadpole.COM (Jim Thompson)_
  + 1994-04-25 (Mon, 25 Apr 94 12:25:38 PDT) - [Re: Wow, what a key!](/archive/1994/04/e11f3b3997a97319d98162de249c1ff9fce12373ccd40dad828baac93d6f2aa1) - _tcmay@netcom.com (Timothy C. May)_
    + 1994-04-25 (Mon, 25 Apr 94 12:43:07 PDT) - [Re: Wow, what a key!](/archive/1994/04/59d05565b5b42490fd6e7374e5bd8fbd987b943763e3a68b8fccf032d6ddab6b) - _Ed Carp \<ecarp@netcom.com\>_
      + 1994-04-25 (Mon, 25 Apr 94 13:20:25 PDT) - [Re: Wow, what a key!](/archive/1994/04/972add4c079a32528fb89538eaa91465d0e9156ace49b53a3cac5a5556181ab7) - _"Perry E. Metzger" \<perry@snark.imsi.com\>_
        + 1994-04-25 (Mon, 25 Apr 94 14:16:24 PDT) - [Re: Wow, what a key!](/archive/1994/04/d3ebcb57f746be4500c02ac915f5ce70dbb296181ddb335694121847dea53385) - _Ed Carp \<ecarp@netcom.com\>_
          + 1994-04-25 (Mon, 25 Apr 94 14:21:03 PDT) - Re: Wow, what a key! - _"Perry E. Metzger" \<perry@snark.imsi.com\>_
            + 1994-04-26 (Mon, 25 Apr 94 17:19:51 PDT) - [Re: Wow, what a key!](/archive/1994/04/407d8febf090cd35cdb76bfd0c5882ac334d641d1b437ab76d7f2d26553b8d69) - _Martin Janzen \<janzen@idacom.hp.com\>_
        + 1994-04-26 (Mon, 25 Apr 94 17:04:52 PDT) - [Re: Wow, what a key!](/archive/1994/04/5ec34f00f64c3ec572e2bf2446211a9e13e08f8131c5789b1e984efd3c5b5c74) - _Paul Schauble \<pls@crl.com\>_
          + 1994-04-26 (Tue, 26 Apr 94 04:07:12 PDT) - [Re: Wow, what a key!](/archive/1994/04/e8017351252f5e73ac354d50c8b45f454385699fa7535b75baefbf09bad88f6c) - _"Perry E. Metzger" \<perry@snark.imsi.com\>_

