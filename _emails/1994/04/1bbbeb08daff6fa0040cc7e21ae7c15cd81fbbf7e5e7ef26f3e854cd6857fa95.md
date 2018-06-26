---
layout: default
---

# 1994-04-11 - RE: Code review is requested

## Header Data

From: anonymous<span>@</span>extropia.wimsey.com<br>
To: cypherpunks@toad.com<br>
Message Hash: 1bbbeb08daff6fa0040cc7e21ae7c15cd81fbbf7e5e7ef26f3e854cd6857fa95<br>
Message ID: \<199404112240.AA05488@xtropia\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-04-11 22:52:00 UTC<br>
Raw Date: Mon, 11 Apr 94 15:52:00 PDT<br>

## Raw message

```
{% raw  %}From: anonymous@extropia.wimsey.com
Date: Mon, 11 Apr 94 15:52:00 PDT
To: cypherpunks@toad.com
Subject: RE: Code review is requested
Message-ID: <199404112240.AA05488@xtropia>
MIME-Version: 1.0
Content-Type: text/plain


>> 3) There may be other RNG's in existence which are accessed in a
>> different way, or have different IO drivers. If you have knowledge of
>> such RNG's please post the info to the cypherpunks mailing list.
>
>In Cryptosystems Journal, published by Tony S Patti, Volume 2 Number 2
>is a description, circuit board layouts, parts list, etc. for Ranger
>hardware RNG. It produced 6,750 bits per second into the parallel port of a
>standard PC. The author says that you can build a Ranger for less than $40
>worth of parts.
>
>Cryptosystyems Journal
>P.O. Box 188
>Newtown PA 18940-0188
>
>I have not seen any reviews of this device, but it has been arround for a
>while, and may have been covered before I got interested in the field.
>

Could not the operating systems' IO driver be used for the interface
to the parallel port be used as the interface to the RNG?

The hack has support for a device which can be accessed thru
an IO driver that returns one random byte for each byte read.
(RANDDRIVER).

Would this be adequate for such a device, or would special
code be required? Is the IO driver for the parallel port
that comes with MS-DOS OK for this purpose?

Has anyone out there built such a device?

Yours in anonymity
XXX




{% endraw %}
```

## Thread

+ Return to [April 1994](/archive/1994/04)

+ Return to "[anonymous<span>@</span>extropia.wimsey.com](/author/anonymous_at_extropia_wimsey_com)"

+ 1994-04-11 (Mon, 11 Apr 94 15:52:00 PDT) - RE: Code review is requested - _anonymous@extropia.wimsey.com_

