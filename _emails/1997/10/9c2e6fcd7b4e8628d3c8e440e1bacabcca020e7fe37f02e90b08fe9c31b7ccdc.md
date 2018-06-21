---
layout: default
---

# 1997-10-08 - Re: What's really in PGP 5.5?

## Header Data

From: Adam Back \<aba@dcs.ex.ac.uk\><br>
To: randerso@ece.eng.wayne.edu<br>
Message Hash: 9c2e6fcd7b4e8628d3c8e440e1bacabcca020e7fe37f02e90b08fe9c31b7ccdc<br>
Message ID: \<199710082004.VAA00169@server.test.net\><br>
Reply To: \<3.0.2.32.19971008090442.0070305c@ece.eng.wayne.edu\><br>
UTC Datetime: 1997-10-08 22:07:01 UTC<br>
Raw Date: Thu, 9 Oct 1997 06:07:01 +0800<br>

## Raw message

```
{% raw  %}From: Adam Back <aba@dcs.ex.ac.uk>
Date: Thu, 9 Oct 1997 06:07:01 +0800
To: randerso@ece.eng.wayne.edu
Subject: Re: What's really in PGP 5.5?
In-Reply-To: <3.0.2.32.19971008090442.0070305c@ece.eng.wayne.edu>
Message-ID: <199710082004.VAA00169@server.test.net>
MIME-Version: 1.0
Content-Type: text/plain




Ryan Anderson <randerso@ece.eng.wayne.edu> writes:
> >
> >What you call "fragility" is properly called "security".  Would you
> >describe 128-bit keys as more "fragile" than 40-bit keys?  Why is PGP,
> >Inc. inventing propaganda terms for the authorities?
> 
> Okay, call it security but the point is, if you're protecting
> documents vital to your company using encryption (say the design of
> a new product) and the person who knows the passphrase dies, you've
> just lost a great deal of money.

Not at all.

People seem to be forgetting that we're talking about email security
here.

Email isn't that reliable.  Email goes missing now and then.  Your DNS
is out, the receivers mail hub has a glitch and swallows it, whatever.

Are you really claiming that you will have email in transit which is
so valuable that your whole company will be in jeopardy if the
intended recipient dies unexpectedly?

More likely: you get the sender to resend it.

Don't confuse the issues surrounding need for backup of storage keys
with communications keys.  There is a definate need to take care to
have backups of keys used to encrypt backups and disks.  Not so for
communications keys.

I gave some alternative GAK unfriendly ways of archiving email in my
longer reply to PGP's Jon Callas defensive article on the NYT article.

> Well, any company giving stock advice (and governed by SEC rules on
> stock tips, etc.) is already require to have all outgoing mail
> approved (e-mail and snail), so does it matter if they record it or
> not?

If a company has a policy of approving outgoing email, I'd argue for a two
tiered system.  One for "official statements" which is approved, archived,
signed with a transferable non-repudiable signature.  And one for unofficial
communications, signed with a non-transferable signature, and perhaps
delivered via mixmaster.

The way to archive your outgoing email is not to have the email in transit
encrypted to an extra recipient.  The way to do it is to archive sent mail
in the senders MUA or at least internal to the senders offices.

You will notice that this then involves storage keys, which the GAKkers
aren't interested in.  Why aren't they interested in access to storage keys? 
Because they would have to issue a supeona and take the disks away before
they would have any use for them.  At that stage they'd just as well list
the keys to decrypt anything which is encrypted on the disks they seize.

The reason the GAKkers want access to communications keys is so that
they can read your email without you knowing.  So they can go on
fishing expeditions and use the evidence by saying that "an unanmed
source" tipped them off, etc.

By implementing GAK for corporates in such a GAK friendly way, PGP Inc
has helped the GAKkers.  I would be interested to persuade them to
change their architecture for archiving sent and received email.

Adam
-- 
Now officially an EAR violation...
Have *you* exported RSA today? --> http://www.dcs.ex.ac.uk/~aba/rsa/

print pack"C*",split/\D+/,`echo "16iII*o\U@{$/=$z;[(pop,pop,unpack"H*",<>
)]}\EsMsKsN0[lN*1lK[d2%Sa2/d0<X+d*lMLa^*lN%0]dsXx++lMlN/dsM0<J]dsJxp"|dc`





{% endraw %}
```

## Thread

+ Return to [October 1997](/archive/1997/10)

+ 1997-10-08 (Wed, 8 Oct 1997 15:29:37 +0800) - [What's really in PGP 5.5?](/archive/1997/10/852daed3738aab8c6e56fea7cba8affcbc92e9aa5ffceebdc1c9e3d822d8f32b) - _Anonymous \<anon@anon.efga.org\>_
  + 1997-10-08 (Wed, 8 Oct 1997 21:16:25 +0800) - [Re: What's really in PGP 5.5?](/archive/1997/10/5988aaafee0856b2ff9f8bc66772dca3cf40e6d2fe897bd01302be55f4fa60dd) - _Ryan Anderson \<randerso@ece.eng.wayne.edu\>_
    + 1997-10-08 (Thu, 9 Oct 1997 06:07:01 +0800) - Re: What's really in PGP 5.5? - _Adam Back \<aba@dcs.ex.ac.uk\>_
    + 1997-10-09 (Thu, 9 Oct 1997 22:32:14 +0800) - [Re: What's really in PGP 5.5?](/archive/1997/10/096034611b09012929a9c1352a5c1b9602b8bf8ae9a27220675efdfa19fbfa0d) - _Ryan Anderson \<randerso@ece.eng.wayne.edu\>_
  + 1997-10-08 (Thu, 9 Oct 1997 00:13:02 +0800) - [Re: What's really in PGP 5.5?](/archive/1997/10/6baf064742a86c038c8da25bdf6e0a5ab4c587b751799fa5830d5c9bd977c6c6) - _Tim May \<tcmay@got.net\>_

