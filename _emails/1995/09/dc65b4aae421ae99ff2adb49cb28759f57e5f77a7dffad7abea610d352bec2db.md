---
layout: default
---

# 1995-09-10 - 64 bit crypto

## Header Data

From: thad@hammerhead.com (Thaddeus J. Beier)<br>
To: cypherpunks@toad.com<br>
Message Hash: dc65b4aae421ae99ff2adb49cb28759f57e5f77a7dffad7abea610d352bec2db<br>
Message ID: \<199509101504.IAA04932@hammerhead.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-09-10 15:12:45 UTC<br>
Raw Date: Sun, 10 Sep 95 08:12:45 PDT<br>

## Raw message

```
{% raw  %}From: thad@hammerhead.com (Thaddeus J. Beier)
Date: Sun, 10 Sep 95 08:12:45 PDT
To: cypherpunks@toad.com
Subject: 64 bit crypto
Message-ID: <199509101504.IAA04932@hammerhead.com>
MIME-Version: 1.0
Content-Type: text/plain



Say that we wanted to use 80 bit RC4 for our crypto application, but we were
only allowed to use 64 bit crypto because we lived in some police state that
enforced its wishes.   Couldn't we modify RC4 easily to provide the same
security against brute-force attacks by just running the key-setup phase
65536 times instead of just once?  That would slow down the key-setup (on
my machine) from 50,000 per second to just over 1 second, but so what?  It
takes ATT more than 1 second to set up a long distance call, I can wait
another second to start the conversation.

If our breaking of 40 bit RC4 was a one, then this 64 bit RC4-modified would
be a 109,951,162,776, well beyond possibilities that I can imagine.  You might
say that you could save all 2^64 key tables, but that is a huge amount of data,
millions of terabyte-capacity tapes.

In the GAK proceedings, I have never heard of any limitation on the algorithm,
just that it be public and 64 bits or less.  And, of course, have GAK.  Of
course, it wouldn't surprise me for this kind of technical fix to be
immediately outlawed by the aforementioned police state.


thad
-- Thaddeus Beier                   email:  thad@hammerhead.com
   Technology Development             vox:  408) 286-3376
   Hammerhead Productions             fax:  408) 292-8624




{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ 1995-09-10 (Sun, 10 Sep 95 08:12:45 PDT) - 64 bit crypto - _thad@hammerhead.com (Thaddeus J. Beier)_

