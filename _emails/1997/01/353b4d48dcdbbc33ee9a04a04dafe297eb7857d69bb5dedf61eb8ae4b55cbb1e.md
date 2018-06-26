---
layout: default
---

# 1997-01-27 - S/KEY (was: 2 Questions)

## Header Data

From: Peter M Allan \<peter.allan<span>@</span>aeat.co.uk\><br>
To: cypherpunks@toad.com<br>
Message Hash: 353b4d48dcdbbc33ee9a04a04dafe297eb7857d69bb5dedf61eb8ae4b55cbb1e<br>
Message ID: \<199701271949.LAA03073@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-01-27 19:49:15 UTC<br>
Raw Date: Mon, 27 Jan 1997 11:49:15 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: Peter M Allan <peter.allan@aeat.co.uk>
Date: Mon, 27 Jan 1997 11:49:15 -0800 (PST)
To: cypherpunks@toad.com
Subject: S/KEY (was: 2 Questions)
Message-ID: <199701271949.LAA03073@toad.com>
MIME-Version: 1.0
Content-Type: text/plain



Steven M Orrin <privsoft@ix.netcom.com> wrote:
> Hey guys,
> 2 quick questions:

> Are there any known hacks or weaknesses in S/Key?


S/Key has a rather limited scope, in aiming to prevent replay attacks.
These are where somebody snoops on your network to obtain passwords,
an uses them in later login attempts.  This is undoubtedly a major
weakness in most current networks.  S/Key addresses this replay of data
obtained in passive eavesdropping, but that is all it does.

Several attacks against S/Key have been discussed [1], including:

   race attacks:  eavesdropping most of the hash, and racing the user
                  to provide the rest of it

   active attacks:  impersonating the server to learn future hashes
                    or simply hijacking an established session.

Strengthening S/Key really means expanding the scope to get an
authenticated and encrypted 2-way connection.  [John Gilmore's S/WAN may
end up achieving this.  I'm not familiar with it (yet?).]

Ideas for improving S/Key that involve secret data stored on the server
tend to get frowned on, as the original aim was to avoid that.  In any case
you cannot get the full encrypted 2-way connection without getting a whole
lot more complicated.

Recent discussions [2] have centred on ways to rekey the list of hashes remotely when
the count runs down.  These changes, and S/Key itself, are better than nothing
but where's the ham sandwich ? [3]

Beside the protocol weakness there is potential for finding collisions in the hash
function (MD4 originally).  A choice of hash functions can be provided. See RFC-1938.
  

1) See also SecureID, which is more complicated and still subject
   to similar attacks.

2) Not here.

3) Old joke.  A ham sandwich is better than nothing, and nothing is better than
   a life of complete happiness, so ......




 -- Peter Allan    peter.allan@aeat.co.uk







{% endraw %}
```

## Thread

+ Return to [January 1997](/archive/1997/01)

+ Return to "[Peter M Allan <peter.allan<span>@</span>aeat.co.uk>](/author/peter_m_allan_peter_allan_at_aeat_co_uk_)"

+ 1997-01-27 (Mon, 27 Jan 1997 11:49:15 -0800 (PST)) - S/KEY (was: 2 Questions) - _Peter M Allan \<peter.allan@aeat.co.uk\>_

