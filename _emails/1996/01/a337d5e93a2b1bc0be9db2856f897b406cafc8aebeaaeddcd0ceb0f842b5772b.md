---
layout: default
---

# 1996-01-30 - Re: FV Demonstrates Fatal Flaw in Software Encryption of Credit Cards

## Header Data

From: Nathaniel Borenstein \<nsb<span>@</span>nsb.fv.com\><br>
To: eric@remailer.net (Eric Hughes)<br>
Message Hash: a337d5e93a2b1bc0be9db2856f897b406cafc8aebeaaeddcd0ceb0f842b5772b<br>
Message ID: \<Ql3VnkqMc50eJIrCwz@nsb.fv.com\><br>
Reply To: \<199601292324.PAA10191@largo.remailer.net\><br>
UTC Datetime: 1996-01-30 13:55:21 UTC<br>
Raw Date: Tue, 30 Jan 1996 21:55:21 +0800<br>

## Raw message

```
{% raw  %}From: Nathaniel Borenstein <nsb@nsb.fv.com>
Date: Tue, 30 Jan 1996 21:55:21 +0800
To: eric@remailer.net (Eric Hughes)
Subject: Re: FV Demonstrates Fatal Flaw in Software Encryption of Credit Cards
In-Reply-To: <199601292324.PAA10191@largo.remailer.net>
Message-ID: <Ql3VnkqMc50eJIrCwz@nsb.fv.com>
MIME-Version: 1.0
Content-Type: text/plain


Excerpts from mail: 29-Jan-96 re: FV Demonstrates Fatal F.. Eric
Hughes@remailer.net (1441)

> I'm breaking my silence in cypherpunks to respond to what must be the
> most self-serving and fatuous expression of "concern" I've seen in a
> while.

It's a pity, Eric, that before coming down off the mountain, you didn't
stop to understand the real attack we're outlining.  I expected that
even if you didn't like what we were doing, you'd take the time to
understand it rather than embarass yourself.

> To wit:  Ohmygod!  PC's don't have perfect integrity!

The fact that PC's don't have perfect integrity is only *one* of the
four known vulnerabilities -- keyboard sniffing being another -- that we
have combined into a comprehensive, devastating attack that has never
been publicly mentioned before.

> Will someone please write a filter for common email packages which
> automatically removes selected First Virtual transactions from the
> confirmation messages?  

I've already written it.  So what?  Stealing or forging a single
transaction is EASY in almost ANY commerce system ever invented.    The
flaw we've uncovered in encrypted credit cards allows a single criminal
to automate the theft of millions of card numbers.  That's a very
different story.

> Encryption isn't the issue, Nathaniel, and you know it.  

Not only do I know it, I ***SAID*** it.  It's painfully obvious that you
didn't read our announcements very carefully, so I'll excerpt the
relevant paragraph:

> Encryption has high value in protecting sensitive information while in 
> transit. We strongly believe in encryption and use PGP, as licensed 
> users, daily. But it is clear that software-based encryption cannot 
> ensure secure credit card transactions. Encryption remains an important 
> part of computer security and is very important for protecting privacy. 
> But recognition of credit card numbers at the keyboard is trivial, and 
> therein lies the fatal flaw to software-based encryption of credit cards 
> -- sensitive information can be intercepted before it ever gets 
> encrypted. 

The issue is definitely not encryption.  The issue is that credit card
numbers are self-identifying one-way payment instruments, and there's no
way to make such instruments safe to use on insecure consumer computing
platforms.  The only reason that encryption even enters the discussion
is that there are OTHER parties who are claiming that their software
encryption products make such payment instruments safe.  They don't. 
That's all we're pointing out.

> To all those Internet payment analysts out there:
>    Financial institutions are in the business of risk transfer.  If
> you don't transfer risk in some form, you're not a financial
> institution but rather a service bureau.  Managing endpoint integrity
> risk is just one of the kinds of risk an Internet payments provider
has to deal with.  

Yes.  But the BIGGEST risk that an Internet payments provider has to
deal with is the threat of large-scale, systematic, automated fraud. 
And *that* is the hole we have just blown in the
software-encryption-of-credit-card schemes, and which you clearly didn't
take the time to understand.

> First Virtual has demonstrated time and again that
> they're pretty clueless about the whole subject of risk.  

Well, I think our financial industry partners will take our "clueless"
level of risk management any day.  We have fraud and chargeback rates so
low that they're scarcely believeable, because nearly all fraud AND
dissatisfied customers are caught by the email loop and never make it
into the credit card system in the first place.  Our acquiring bank
thinks that's pretty neat, I think.  In fact, it's worth noting that
after being our acquiring bank for over a year of live operation, and
having the most inside information possible about how our system works,
First USA Bank (one of the nation's largest credit card banks) made a
large equity investment in us last month.  Do you really think they
didn't do any risk analysis? -- Nathaniel
--------
Nathaniel Borenstein <nsb@fv.com>
Chief Scientist, First Virtual Holdings
FAQ & PGP key: nsb+faq@nsb.fv.com




{% endraw %}
```

## Thread

+ Return to [January 1996](/archive/1996/01)

+ Return to "[eric<span>@</span>remailer.net (Eric Hughes)](/authors/eric_at_remailer_net_eric_hughes_)"
+ Return to "[Nathaniel Borenstein <nsb<span>@</span>nsb.fv.com>](/authors/nathaniel_borenstein_nsb_at_nsb_fv_com_)"
+ Return to "["Paul M. Cardon" <pmarc<span>@</span>fnbc.com>](/authors/paul_m_cardon_pmarc_at_fnbc_com_)"

+ 1996-01-30 (Wed, 31 Jan 1996 00:40:53 +0800) - [re: FV Demonstrates Fatal Flaw in Software Encryption of Credit Cards](/archive/1996/01/83e34157bb56185d04c6470b2f2de9e9715ea67b8418ef80c76aa77db58f396d) - _eric@remailer.net (Eric Hughes)_
  + 1996-01-30 (Tue, 30 Jan 1996 21:55:21 +0800) - Re: FV Demonstrates Fatal Flaw in Software Encryption of Credit Cards - _Nathaniel Borenstein \<nsb@nsb.fv.com\>_
  + 1996-01-30 (Wed, 31 Jan 1996 01:46:52 +0800) - [Re: FV Demonstrates Fatal Flaw in Software Encryption of Credit Cards](/archive/1996/01/893a2d21d7f04ba7883113dcd33daceade39e0940231fb0a650b542db66f4757) - _"Paul M. Cardon" \<pmarc@fnbc.com\>_

