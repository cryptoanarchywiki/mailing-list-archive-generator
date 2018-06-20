---
layout: default
---

# 1994-08-25 - $10M breaks MD5 in 24 days

## Header Data

From: Hal \<hfinney@shell.portal.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: a6cf9e2cb4a81847daccdfce2b97e5f1add02c1ca0ee3c80871e1ba3c4d5cb99<br>
Message ID: \<199408252058.NAA12488@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-08-25 20:58:33 UTC<br>
Raw Date: Thu, 25 Aug 94 13:58:33 PDT<br>

## Raw message

```
{% raw  %}From: Hal <hfinney@shell.portal.com>
Date: Thu, 25 Aug 94 13:58:33 PDT
To: cypherpunks@toad.com
Subject: $10M breaks MD5 in 24 days
Message-ID: <199408252058.NAA12488@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


I am not attending the Crypto conference, but I sat in on the evening
"rump session" the other day.  One of the more interesting papers had
a claim (with little detail, unfortunately) that for ten million dollars
you could build a machine that would "break" MD5, in the sense of finding
another message which would hash to the same as a chosen one, in 24
days.  This result did not depend on any internal structure in MD5, but
was purely a result of the hash size (128 bits) and the time it takes
to calculate a hash.

The main new result which allowed this was a more efficient way of
handling a parallel search for collisions (two messages which hash to
the same thing).  In some earlier methods, n machines provide only a
sqrt(n) speedup.  The new method improves this, although my notes don't
show exactly how close they come to an n-fold speedup.

The Secure Hash Standard (SHS, aka SHA) is, they said, 64K times slower,
hence this technique would take 64K times longer (or cost ~64K times
more?) to break that hash.

I don't think this is probably anything to really worry about, but
maybe it points out a need for a longer hash in the next few years.

Hal

P.S. The paper was by Paul C. van Oorschot & Michael J. Wiener.




{% endraw %}
```

## Thread

+ Return to [August 1994](/archive/1994/08)

+ 1994-08-25 (Thu, 25 Aug 94 13:58:33 PDT) - $10M breaks MD5 in 24 days - _Hal \<hfinney@shell.portal.com\>_
  + 1994-08-26 (Thu, 25 Aug 94 17:01:47 PDT) - [Re: $10M breaks MD5 in 24 days](/archive/1994/08/7560da5d6922fc8bb8c34a9f08fc20caf31b1d7dfc8efc87393b8245363b5352) - _alex \<cp@omaha.com\>_
    + 1994-08-26 (Thu, 25 Aug 94 17:37:35 PDT) - [Re: $10M breaks MD5 in 24 days](/archive/1994/08/c0c7e7f80c3c757325baab9699d8a38bc5bca72880e6673700d6b28e2c9e2cf6) - _"Perry E. Metzger" \<perry@imsi.com\>_

