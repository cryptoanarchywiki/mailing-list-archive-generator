---
layout: default
---

# 1998-11-28 - Re: Securing data in memory (was "Locking physical memory (fwd)

## Header Data

From: Jim Choate \<ravage@einstein.ssz.com\><br>
To: cypherpunks@einstein.ssz.com (Cypherpunks Distributed Remailer)<br>
Message Hash: 02ff0e2f7df6c824ebff92dcf48443aa839edd0cd7f89a91a2fceaf57fb1babd<br>
Message ID: \<199811281744.LAA04641@einstein.ssz.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1998-11-28 18:07:18 UTC<br>
Raw Date: Sun, 29 Nov 1998 02:07:18 +0800<br>

## Raw message

```
{% raw  %}From: Jim Choate <ravage@einstein.ssz.com>
Date: Sun, 29 Nov 1998 02:07:18 +0800
To: cypherpunks@einstein.ssz.com (Cypherpunks Distributed Remailer)
Subject: Re: Securing data in memory (was "Locking physical memory (fwd)
Message-ID: <199811281744.LAA04641@einstein.ssz.com>
MIME-Version: 1.0
Content-Type: text



Forwarded message:

> Date: Sat, 28 Nov 1998 17:41:53 +0100
> From: Anonymous <nobody@replay.com>
> Subject: Re: Securing data in memory (was "Locking physical memory (fwd)

> What is Choate thinking when he says the ENTIRE OS is run under this?

My mistake. Since it really does only handle individual apps it's of limited
utility in the Windows world because of the numerous ways to get system
level access.

> This is a driver which is used by the application to allocate specific
> memory buffers in non-swappable memory.  It allows the app to lock down
> those buffers so that they won't swap to disk.  These buffers can then
> be used to hold sensitive data.

Considering that this doesn't prohibit apps from getting access to that
memory, it only prohibits that memory page from being written to disk, it
has limited utility. It's only real protection is against disk scans.

For example a bogus service could gain system level and initiate a DMA
transfer of that non-swappable ram into their own address space.

> It is neither possible nor desirable to run the ENTIRE OS out of
> such buffers.

Sure it is. It's the entire reason to have big online memory pools. Idealy
you'd have a computer with nothing but gig's and gig's of ram and no hard
drive at all.

> It is not possible because the OS is already written.
> It is Windows 3.x/95/98 (see above).  That OS does not make the special
> driver calls which would be necessary to allocate non-swappable memory.
> You would have to rewrite Windows to use the special calls, which isn't
> possible for a luser like Choate.

No, simply provide it enough ram it never has to swap out to disk except in
the case of updates to files. If ram's that cheap we could do away with the
drive completely.

> And it's not even desirable.  There is no reason to make the ENTIRE OS
> use non-swappable memory.

They why do I (and you unless youre using a tty) keep adding ram to my
Win/Linux/Solaris/AIX/HP/etc. boxes to reduce the swapping that is taking
place? It's slow, we put up with it because we can't afford those hundreds
of meg's of ram to hold our app and the entire database file (for example).

>  Most memory is simply not that sensitive.
> It holds public data, or data which is already on the disk in some form.
> Putting the ENTIRE OS into non-swappable memory gives up much of the
> advantage of having virtual memory in the first place.  It would be a
> giant step backwards in OS architecture.

No, it wouldn't. The question of swap or virtual space is one of economics
and not computer architecture. If it were economicaly feasible there would
be no drives just fast main ram.


    ____________________________________________________________________
 
             Technology cannot make us other than what we are.

                                           James P. Hogan

       The Armadillo Group       ,::////;::-.          James Choate
       Austin, Tx               /:'///// ``::>/|/      ravage@ssz.com
       www.ssz.com            .',  ||||    `/( e\      512-451-7087
                           -====~~mm-'`-```-mm --'-
    --------------------------------------------------------------------




{% endraw %}
```

## Thread

+ Return to [November 1998](/archive/1998/11)

+ 1998-11-28 (Sun, 29 Nov 1998 02:07:18 +0800) - Re: Securing data in memory (was "Locking physical memory (fwd) - _Jim Choate \<ravage@einstein.ssz.com\>_
  + 1998-11-30 (Mon, 30 Nov 1998 12:18:26 +0800) - [Re: Securing data in memory (was "Locking physical memory (fwd)](/archive/1998/11/346ffc87cf49eb981dd7629ea5c4e8b05323241f54f23bbf921402a21ac960ca) - _Bill Stewart \<bill.stewart@pobox.com\>_

