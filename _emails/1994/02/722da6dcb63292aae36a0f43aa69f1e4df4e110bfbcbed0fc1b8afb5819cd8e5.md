---
layout: default
---

# 1994-02-15 - Detweiler abuse again

## Header Data

From: hughes@ah.com (Eric Hughes)<br>
To: cypherpunks@toad.com<br>
Message Hash: 722da6dcb63292aae36a0f43aa69f1e4df4e110bfbcbed0fc1b8afb5819cd8e5<br>
Message ID: \<9402151753.AA22610@ah.com\><br>
Reply To: \<199402151730.JAA06052@jobe.shell.portal.com\><br>
UTC Datetime: 1994-02-15 18:01:41 UTC<br>
Raw Date: Tue, 15 Feb 94 10:01:41 PST<br>

## Raw message

```
{% raw  %}From: hughes@ah.com (Eric Hughes)
Date: Tue, 15 Feb 94 10:01:41 PST
To: cypherpunks@toad.com
Subject: Detweiler abuse again
In-Reply-To: <199402151730.JAA06052@jobe.shell.portal.com>
Message-ID: <9402151753.AA22610@ah.com>
MIME-Version: 1.0
Content-Type: text/plain


>I'm not sure Eric's idea about connecting via sockets would eliminate all
>possibilities of logging.  

I did not mean to imply this.  Using daemons would get rid of the
_default_ loging that occurs on systems.  Changing logging from
opt-out to opt-in would make a large practical difference right now.

>It seems that with telnet, at least, the systems
>that you connect to are able to find your host name.  Still, host names
>would be more private than full addresses.

This was exactly my point in a previous article.  An email address
identifies both a machine and a user, where an IP connection (e.g.
telnet) only reveals the machine.  Now if the sysadmin of the
originating machine logs and shares information with the destination
machine, the user can be identified.  But again, this is an opt-in
monitoring system.

Eric




{% endraw %}
```

## Thread

+ Return to [February 1994](/archive/1994/02)

+ 1994-02-15 (Tue, 15 Feb 94 09:33:58 PST) - [Re: Detweiler abuse again](/archive/1994/02/675e9f15e112029716b3ff5a63c77b05a6f72ed9ebb79e0b3085a726196dc2fc) - _Hal \<hfinney@shell.portal.com\>_
  + 1994-02-15 (Tue, 15 Feb 94 10:01:41 PST) - Detweiler abuse again - _hughes@ah.com (Eric Hughes)_
    + 1994-02-15 (Tue, 15 Feb 94 11:31:42 PST) - [Re: Detweiler abuse again](/archive/1994/02/51292e703550864907efcb46e39a0d82f57a22fd77e3df5c8e0c5d5f46ae17e9) - _"Jon 'Iain' Boone" \<boone@psc.edu\>_

