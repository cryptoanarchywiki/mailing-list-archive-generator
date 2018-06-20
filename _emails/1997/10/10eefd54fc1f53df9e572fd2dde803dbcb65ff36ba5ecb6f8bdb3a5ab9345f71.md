---
layout: default
---

# 1997-10-30 - Re: PGP Employee on MKR

## Header Data

From: Adam Back \<aba@dcs.ex.ac.uk\><br>
To: stewarts@ix.netcom.com<br>
Message Hash: 10eefd54fc1f53df9e572fd2dde803dbcb65ff36ba5ecb6f8bdb3a5ab9345f71<br>
Message ID: \<199710301702.RAA03029@server.test.net\><br>
Reply To: \<3.0.3.32.19971030025716.006cdf80@popd.ix.netcom.com\><br>
UTC Datetime: 1997-10-30 18:18:22 UTC<br>
Raw Date: Fri, 31 Oct 1997 02:18:22 +0800<br>

## Raw message

```
{% raw  %}From: Adam Back <aba@dcs.ex.ac.uk>
Date: Fri, 31 Oct 1997 02:18:22 +0800
To: stewarts@ix.netcom.com
Subject: Re: PGP Employee on MKR
In-Reply-To: <3.0.3.32.19971030025716.006cdf80@popd.ix.netcom.com>
Message-ID: <199710301702.RAA03029@server.test.net>
MIME-Version: 1.0
Content-Type: text/plain




Bill Stewart <stewarts@ix.netcom.com> writes:
> At 02:38 AM 10/27/1997 -0800, mark@unicorn.com wrote:
> >Really? I seem to recall Jon Callas saying my system 'redesigned CMR' 
> >but was simpler than theirs. The mere fact that CMR requires an enforcer 
> >implies that it's a convoluted and hasty design. 
> 
> Not true - you can't implement CMR without a mail enforcer unless
> you can stop your employees from using non-CMR versions of PGP,
> which is nearly impossible.  Even with an enforcer, of course,
> you can't stop the determined employee from double-encrypting and
> steganizing and otherwise getting their outbound bits past your enforcer
> or Pointy-Haired-Boss randomness, 

If the corporate is serious about preventing encrypted messages
leaving their net that they can't read, the simple solution is to
disallow employees from using encryption -- have the enforcer encrypt
it.

Even if you were to use CMR, it is dumb, dumb, dumb, to allow the
snoop key to remain after the message has passed the enforcer -- it
should strip it off on the way out.

> but they could also carry a floppy disk out the door or beam
> infrared out the window from their Newton.

Attempting to compress the plaintext helps -- if it won't compress
(much) you get suspicious.

Pointy-Haired-Boss randomness always works -- compresses well and can
encode anything.

> Similarly, on incoming mail, you can't stop people from sending your
> employees non-CMRed mail without an inbound-mail enforcer and
> can't stop your employees from reading it with their own warez.

Even with enforcer and CMR it's possible to get past it,
super-encryption, garbage in CMRK second recipient field, and
Pointy-Haired-Boss randomness.

Simpler, safer, and more effective to just escrow the employees
company use key -- that ensures there is only one recipient on the
message passing over the internet.

> More importantly, though, PGP isn't a mail program, it's an encryptor,
> and if you're trying to stop people from sending encrypted mail
> back and forth, you've got to control the mail system as well as the
> encryptors, 

So ultimately prevention largely falls back to controlling what
software people are running inside the building -- no laptops in or
out, no floppies in or out, no installing software, metal detector at
door, body scan, the works.


Detection of sending encrypted mails is easier -- just try to decrypt
everything and have all keys necessary escrowed.  Anything which can't
be read doesn't make it in; anything sent which can't be read results
in a sacked employee.


Companies which aren't after this level of paranoia, but just want to
be able to recover company business mails queued when employee is away
-- fine have separate personal use keys attached to the same
signature key.

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

+ 1997-10-27 (Mon, 27 Oct 1997 19:28:22 +0800) - [Re: PGP Employee on MKR](/archive/1997/10/cfd93b066d709199289416aa4da0549b649dd2437a66a580665a84693f5ec68c) - _mark@unicorn.com_
  + 1997-10-30 (Thu, 30 Oct 1997 19:29:57 +0800) - [Re: PGP Employee on MKR](/archive/1997/10/100668118e43fa3aeb3d9e26b628787942632db6d4b43ab77635b6dd6d4cd132) - _Bill Stewart \<stewarts@ix.netcom.com\>_
    + 1997-10-30 (Fri, 31 Oct 1997 02:18:22 +0800) - Re: PGP Employee on MKR - _Adam Back \<aba@dcs.ex.ac.uk\>_

