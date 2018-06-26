---
layout: default
---

# 1996-11-06 - Re: Information

## Header Data

From: "P. J. Ponder" \<ponder<span>@</span>freenet.tlh.fl.us\><br>
To: "Edward R. Figueroa" \<kb4vwa@juno.com\><br>
Message Hash: eebcf67e2e9d0c3cd4482c5a84d1f4bc1f27a6bf0964efad6f70d15eff0be0ae<br>
Message ID: \<Pine.OSF.3.91.961106181407.23406I-100000@fn3.freenet.tlh.fl.us\><br>
Reply To: \<19961105.131710.5207.1.kb4vwa@juno.com\><br>
UTC Datetime: 1996-11-06 23:50:13 UTC<br>
Raw Date: Wed, 6 Nov 1996 15:50:13 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: "P. J. Ponder" <ponder@freenet.tlh.fl.us>
Date: Wed, 6 Nov 1996 15:50:13 -0800 (PST)
To: "Edward R. Figueroa" <kb4vwa@juno.com>
Subject: Re: Information
In-Reply-To: <19961105.131710.5207.1.kb4vwa@juno.com>
Message-ID: <Pine.OSF.3.91.961106181407.23406I-100000@fn3.freenet.tlh.fl.us>
MIME-Version: 1.0
Content-Type: text/plain




On Tue, 5 Nov 1996, Edward R. Figueroa wrote:

> I'm a new Cyberpunk!   
> 
> I apologized if this is not the place to post this message request.
> 
> I have some interesting projects and questions for the Cyberpunk world.
> 
> I would like to know if there is any Cyberpunks in S. Florida (Miami) who
> could converse with me about Crypto?   I am very interested in making new
> Cyberpunk friends, meeting places,  etc.., or please send me E-mail.
> 
> I would like to know where to place my Public Key?   Note, I only have
> E-mail access at this time, and not the Net access, but could have a
> friend place the key for me.
> 
> Last,  I would like to know once and for all,  is PGP compromised,  is
> there a back door, and have we been fooled by NSA to believe it's
> secure?

As far as anyone knows that has publicly commented on it, PGP is presumed 
to be secure against known attacks.  By making the source code available, 
and basing the encryption on published methods - RSA and IDEA, PGP has 
been reviewed extensively by the world's experts on crypto, and those 
experts that publish their results have said there is no known easy way 
to crack it.  There are, of course, many experts who do not publish their 
results - for instance, cryptographers who work for intelligence 
gathering agencies.  What they have found out about RSA and IDEA the rest 
of us don't know.  There are efforts underway to prove mathematically how 
hard it is to break the sort of encryption that PGP is based on.

One thing to remember with PGP is that you must very carefully choose 
your pass phrase and keep it a secret.  If your pass phrase is easy to 
guess, then PGP won't offer you any real security.  Choose a long one, 
that is not composed of words likely to be found in dictionaries or 
published books, and memorize it.

Go to the library and get this book:

 _PGP: Pretty Good Privacy_,
by Simson Garfinkel, 
O'Reilly and Associates, Publishers
1995
ISBN 1-56592-098-8

If the library doesn't have it, ask the librarian to get for you by 
'Inter-Library Loan'.  If you still can't get it, try the library at one 
of the branch campuses of Miami-Dade Community College (MDCC) or Florida 
International University (FIU) on Tamiami Trail.  They should be able to 
help.

This is from the key server at MIT 
http://www-swiss.ai.mit.edu/~bal/pks-toplev.html 
and explains the process for dealing with PGP key servers if all you have 
is e-mail access:

---<begin quoted material>---

PGP Public Email Keyservers
---------------------------

There are PGP public email key servers which allow one to exchange public
keys running using the Internet and UUCP mail systems.
Those capable of accessing the WWW might prefer to use the WWW interface
available via http://www.pgp.net/pgp/www-key.html and managers of sites
which may want to make frequent lookups may care to copy the full keyring
from the FTP server at ftp.pgp.net:pub/pgp/

This service exists only to help transfer keys between PGP users.
It does NOT attempt to guarantee that a key is a valid key;
use the signatures on a key for that kind of security.

Each keyserver processes requests in the form of mail messages.
The commands for the server are entered on the Subject: line.
---------------------------------------------- ======== -----
Note that they should NOT be included in the body of the message.
--------------------- === ---------------------------------------

        To: pgp-public-keys@keys.pgp.net
        From: johndoe@some.site.edu
        Subject: help

Sending your key to ONE server is enough.  After it processes your
key, it will forward your add request to other servers automagically.

For example, to add your key to the keyserver, or to update your key if it
is already there, send a message similar to the following to any server:

        To: pgp-public-keys@keys.pgp.net
        From: johndoe@some.site.edu
        Subject: add

        -----BEGIN PGP PUBLIC KEY BLOCK-----
        Version: 2.6

        
        -----END PGP PUBLIC KEY BLOCK-----

COMPROMISED KEYS:  Create a Key Revocation Certificate (read the PGP
docs on how to do that) and mail your key to the server once again,
with the ADD command.

Valid commands are:

Command                Message body contains
---------------------- -------------------------------------------------
ADD                    Your PGP public key (key to add is body of msg)
INDEX                  List all PGP keys the server knows about (-kv)
VERBOSE INDEX          List all PGP keys, verbose format (-kvv)
GET                    Get the whole public key ring (split)
GET userid             Get just that one key
MGET regexp            Get all keys which match /regexp/
                       regexp must be at least two characters long
LAST days              Get the keys updated in the last `days' days
------------------------------------------------------------------------

---<end of quoted material>---

--
pj

> 
> Ed - 
> 
> kb4vwa@juno.com
> 




{% endraw %}
```

## Thread

+ Return to [November 1996](/archive/1996/11)

+ Return to "[C Matthew Curtin <cmcurtin<span>@</span>research.megasoft.com>](/author/c_matthew_curtin_cmcurtin_at_research_megasoft_com_)"
+ Return to "[Dale Thorn <dthorn<span>@</span>gte.net>](/author/dale_thorn_dthorn_at_gte_net_)"
+ Return to "[kb4vwa<span>@</span>juno.com (Edward R. Figueroa)](/author/kb4vwa_at_juno_com_edward_r_figueroa_)"
+ Return to "["P. J. Ponder" <ponder<span>@</span>freenet.tlh.fl.us>](/author/p_j_ponder_ponder_at_freenet_tlh_fl_us_)"

+ 1996-11-05 (Tue, 5 Nov 1996 10:13:35 -0800 (PST)) - [Information](/archive/1996/11/49ede31248df99348707cf7de9cef27dda7ea8bb78016c73905bdbc856d1e337) - _kb4vwa@juno.com (Edward R. Figueroa)_
  + 1996-11-06 (Wed, 6 Nov 1996 05:23:34 -0800 (PST)) - [Re: Information](/archive/1996/11/9b847438bc19e7b6a1abd0d160283a41821fc92ed8713cf2fef0db2ba7a8c601) - _C Matthew Curtin \<cmcurtin@research.megasoft.com\>_
  + 1996-11-06 (Wed, 6 Nov 1996 15:50:13 -0800 (PST)) - Re: Information - _"P. J. Ponder" \<ponder@freenet.tlh.fl.us\>_
    + 1996-11-07 (Wed, 6 Nov 1996 21:57:21 -0800 (PST)) - [Re: Information](/archive/1996/11/b2d50b5894956a9fcf85d7f7b0001a4659fec5ed771e10fd5da28182512cfe49) - _Dale Thorn \<dthorn@gte.net\>_

