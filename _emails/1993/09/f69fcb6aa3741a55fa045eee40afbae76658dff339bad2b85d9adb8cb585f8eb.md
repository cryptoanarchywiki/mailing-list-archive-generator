---
layout: default
---

# 1993-09-05 - A question about pasting

## Header Data

From: nobody<span>@</span>eli-remailer<br>
To: cypherpunks@toad.com<br>
Message Hash: f69fcb6aa3741a55fa045eee40afbae76658dff339bad2b85d9adb8cb585f8eb<br>
Message ID: \<9309050727.AA15916@toad.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-09-05 07:27:29 UTC<br>
Raw Date: Sun, 5 Sep 93 00:27:29 PDT<br>

## Raw message

```
{% raw  %}From: nobody@eli-remailer
Date: Sun, 5 Sep 93 00:27:29 PDT
To: cypherpunks@toad.com
Subject: A question about pasting
Message-ID: <9309050727.AA15916@toad.com>
MIME-Version: 1.0
Content-Type: text/plain


-----BEGIN PGP SIGNED MESSAGE-----

This probably a naive question, but:

Is there any way, using a remailer, to paste something into the
header that will provide a return address (different from the
reamiler's) that can be recognized by a garden variety unix mail
program?

Because it seems to me that if it is, then it would be possible
to set up a mail forwarding site that would work in the following
way:

1.   A user would send in and register, possibly (preferably) via
     a remailer chain, a public-key and a remailer return
     address.  A remailer return address would be a PGP encrypted
     command bundled with a remailer address;  the PGP command
     would cause the remailer to forward the mail to the user
     through a chain of remailers.

2.   These would be stored under an alias, either user-defined or
     automatically allocated (like anon.penet.fi).

3.   Once registered, the server would send encrypted mail back
     to the user via the chain, and request that the user take
     some specific action (ie., send mail with the a random ten
     character string in the subject line, or whatever) to verify
     the address.  This would prevent people from creating
     anonymous identities that forwarded mail to someone else.

4.   Once the identity was registered and confirmed, then
     whenever mail is sent to that address, the forwarder will
     encrypt it with the public key and use the remailer chain to
     forward the mail.  The identity of the person sending mail
     to the alias and the subject line would be buried in the
     cyhpertext.

5.   The server will also make the public key of all identities
     available via a mail request, so that signatures can be
     verified by people who want to do that.

The whole point of this is that it would then be possible to have
mail that's very secure (except for traffic analysis).  You could
use PGP encrypted outgoing mail to everyone, even people who
don't know or care about remailers.  Your sysadmin wouldn't know
what your outgoing mail contained or who it was to.  None of the
people operating remailers would know that either, because you're
using a chain.

If you could paste a line into a header that would allow others
to mail to your alias by just pressing 'r' on their mailer, then
you wouldn't be asking your correspondents to sacrifice any
convenience on their end.

The people running the alias server wouldn't know who you really
were, and niether would any of the people running the remailers
on on the encrypted return chain.

The result of all this would be that all of your incoming and
outgoing mail would be encrypted, and the identities of your
correspondents would be hidden, as would the contents of your
letters;  and you wouldn't be depending upon any single person to
hold your secrets for you, because none of the individual
remailers would be able to piece anything together, and the alias
server wouldn't know anything about you at all.  And all of this
would be 100% compatible with the existing email system (you
could communicate with non-participants).

It's almost an axiom that any simple idea like this can't work,
or else it would already be implemented.  That suggests to me
that you *can't* paste something in the header that will
automatically route replies to an alias rather than back to where
the letter came from.

Is that the case?

     Alex
     astrashe@nyx.cs.du.edu


-----BEGIN PGP SIGNATURE-----
Version: 2.3a

iQCVAgUBLImSLbGKvmrRrQghAQGs8QQAsVR4TKqKEda04dYarEuwWgwN5eejQbKP
SCdRwEYhl7UhzcVuTCoRezHeqLYWa56a00hBu3qGY+HE/0VPWns7bmNodt4Ykdxl
sbpPfwTwS+dPDrQBUAIhYSxT1A1dxhjkI5uKK7zj4PqbUjcp0e9BBuiClQk6Yz3K
WXmsJ3byvEw=
=xMN5
-----END PGP SIGNATURE-----




{% endraw %}
```

## Thread

+ Return to [September 1993](/archive/1993/09)

+ Return to "[nobody<span>@</span>eli-remailer](/authors/nobody_at_eliremailer)"

+ 1993-09-05 (Sun, 5 Sep 93 00:27:29 PDT) - A question about pasting - _nobody@eli-remailer_

