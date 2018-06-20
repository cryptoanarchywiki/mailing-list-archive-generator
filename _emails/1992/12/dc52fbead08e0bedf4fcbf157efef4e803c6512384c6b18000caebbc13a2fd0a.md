---
layout: default
---

# 1992-12-23 - Re: Signing ascii text

## Header Data

From: mark@coombs.anu.edu.au (Mark)<br>
To: cypherpunks@toad.com<br>
Message Hash: dc52fbead08e0bedf4fcbf157efef4e803c6512384c6b18000caebbc13a2fd0a<br>
Message ID: \<9212232118.AA01592@coombs.anu.edu.au\><br>
Reply To: _N/A_<br>
UTC Datetime: 1992-12-23 21:19:37 UTC<br>
Raw Date: Wed, 23 Dec 92 13:19:37 PST<br>

## Raw message

```
{% raw  %}From: mark@coombs.anu.edu.au (Mark)
Date: Wed, 23 Dec 92 13:19:37 PST
To: cypherpunks@toad.com
Subject: Re: Signing ascii text
Message-ID: <9212232118.AA01592@coombs.anu.edu.au>
MIME-Version: 1.0
Content-Type: text/plain


>Date: Wed, 23 Dec 92 11:02:31 PST
>From: Eric Messick <eric@parallax.com>

>It would canonicalize a file by
>turning all sequences of white space into a single space and trimming
>leading and trailing whitespace from the file before computing the
>hash.

If the message contained a table of figures formatted and seperated with
spaces then that method would destroy the readability of the table. If the
file was processed to change tabs to spaces, according to your .exrc
settings, then the message would be cleared of any ambiguities from
differing lengths of tabs. This is assuming none of the forwarding mail
systems between parties replaces a sequence of spaces with a single tab.
I personally havent seen such behaviour, nor would I expect it. It makes
too many (bad) assumptions.

Trailing spaces should of course be nulled as they serve little purpose.

Mark
mark@coombs.anu.edu.au




{% endraw %}
```

## Thread

+ Return to [December 1992](/years/1992/12)

+ 1992-12-23 (Wed, 23 Dec 92 13:19:37 PST) - Re: Signing ascii text - _mark@coombs.anu.edu.au (Mark)_

