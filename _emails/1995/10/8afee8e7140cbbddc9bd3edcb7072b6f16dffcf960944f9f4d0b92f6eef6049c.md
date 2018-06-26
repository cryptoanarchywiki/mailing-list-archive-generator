---
layout: default
---

# 1995-10-27 - Re: Linux security issues

## Header Data

From: "Rev. Mark Grant" \<mark<span>@</span>unicorn.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: 8afee8e7140cbbddc9bd3edcb7072b6f16dffcf960944f9f4d0b92f6eef6049c<br>
Message ID: \<Pine.3.89.9510271651.A410-0100000@unicorn.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-10-27 18:08:35 UTC<br>
Raw Date: Sat, 28 Oct 1995 02:08:35 +0800<br>

## Raw message

```
{% raw  %}From: "Rev. Mark Grant" <mark@unicorn.com>
Date: Sat, 28 Oct 1995 02:08:35 +0800
To: cypherpunks@toad.com
Subject: Re: Linux security issues
Message-ID: <Pine.3.89.9510271651.A410-0100000@unicorn.com>
MIME-Version: 1.0
Content-Type: text/plain


On Thu, 26 Oct 1995, Bill Frantz wrote:

> However, the pass phrase is not the only dangerous information. 
> Intermediate forms used for decrypting the RSA private keys, and the
> decrypted RSA private keys also have to be protected.  The logic of PGP
> requires that it keep at least one of these around for a long time, so it
> will probably be written to swap space.

Couldn't you use mmap() to map a disk file into your address space, keep 
all your secret data in that part of the address space, and then 
carefully wipe that file before exiting ?

I guess you'd then have the problem that people could just read that file
(if they had the priviledges to do so) to find all the secret data rather
than having to trawl through the swap file though.. and you'd still have
to worry about disk buffering. So it probably wouldn't be a big
improvement. 

	Mark





{% endraw %}
```

## Thread

+ Return to [October 1995](/archive/1995/10)

+ Return to "["Rev. Mark Grant" <mark<span>@</span>unicorn.com>](/author/rev_mark_grant_mark_at_unicorn_com_)"

+ 1995-10-27 (Sat, 28 Oct 1995 02:08:35 +0800) - Re: Linux security issues - _"Rev. Mark Grant" \<mark@unicorn.com\>_

