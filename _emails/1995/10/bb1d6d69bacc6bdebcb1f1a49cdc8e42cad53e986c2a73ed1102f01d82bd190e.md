---
layout: default
---

# 1995-10-06 - Re: subjective names and MITM

## Header Data

From: Hal \<hfinney<span>@</span>shell.portal.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: bb1d6d69bacc6bdebcb1f1a49cdc8e42cad53e986c2a73ed1102f01d82bd190e<br>
Message ID: \<199510061708.KAA27047@jobe.shell.portal.com\><br>
Reply To: \<2264.9510061657@misun2.mi.leeds.ac.uk\><br>
UTC Datetime: 1995-10-06 17:10:07 UTC<br>
Raw Date: Fri, 6 Oct 95 10:10:07 PDT<br>

## Raw message

```
{% raw  %}From: Hal <hfinney@shell.portal.com>
Date: Fri, 6 Oct 95 10:10:07 PDT
To: cypherpunks@toad.com
Subject: Re: subjective names and MITM
In-Reply-To: <2264.9510061657@misun2.mi.leeds.ac.uk>
Message-ID: <199510061708.KAA27047@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


jbaber@mi.leeds.ac.uk writes (where I have taken the liberty of
reformatting for 80 columns):

> Now mail is far easier to fake/intercept than a digital
> signature/encryption - at least I hope so. Therefore if Hal where to
> sign all of his messages I could check the signatures with a public key
> obtained from anywhere at all and if they passed then I could be
> confident that the messages were all written by the entity with control
> of the secret part of the key - at least far more confident than I am
> at all of the mail from hfinney@shell.portal.com actually comes from
> there. So instead of me getting the idea that hfinney@shell.portal.com
> posts interesting messages I get the idea that the holder of the secret
> key posts interesting messages - I would probably still use the mail
> address as keys are less convenient with current mail readers but that
> is an implementation problem. Hals reputation is therefore transfered
> to they key - no matter where I got the key from. So if I send
> encrypted mail to the person with the private part of Hal's key I can
> be sure that it can only be read by the person who actually sent the
> messages pertaining to be from Hal.

Well, this is not necessarily the case.  A MITM may be signing my
messages for me, and then putting them back the way they were before I
am allowed to see them.  Granted, this would not be easy, and perhaps
the difficulty of this would be great enough that you will feel
comfortable using an unsigned key.  But if it were accomplished, then
your messages to me would actually be insecure.  No matter how
convinced you became of my sincerity and trustworthiness, actually our
conversations would be overheard by a third party despite both of our
efforts to the contrary.  Our use of encryption would be rendered
futile.  Doesn't this bother you?

Hal




{% endraw %}
```

## Thread

+ Return to [October 1995](/archive/1995/10)

+ Return to "[Hal <hfinney<span>@</span>shell.portal.com>](/author/hal_hfinney_at_shell_portal_com_)"
+ Return to "[jbaber<span>@</span>mi.leeds.ac.uk](/author/jbaber_at_mi_leeds_ac_uk)"
+ Return to "[Jiri Baum <jirib<span>@</span>sweeney.cs.monash.edu.au>](/author/jiri_baum_jirib_at_sweeney_cs_monash_edu_au_)"

+ 1995-10-06 (Fri, 6 Oct 95 09:05:53 PDT) - [Re: subjective names and MITM](/archive/1995/10/99aa9c7fedfd05a01ed205b672a7dfe094caf3c0003fdd675a0ac28d1c9879af) - _jbaber@mi.leeds.ac.uk_
  + 1995-10-06 (Fri, 6 Oct 95 10:10:07 PDT) - Re: subjective names and MITM - _Hal \<hfinney@shell.portal.com\>_
    + 1995-10-24 (Tue, 24 Oct 95 00:10:45 PDT) - [Re: subjective names and MITM](/archive/1995/10/ed9db55a20c0173319aa24815e8de682a4198001ec746efe4e8d44d46bc13700) - _Jiri Baum \<jirib@sweeney.cs.monash.edu.au\>_
      + 1995-10-24 (Tue, 24 Oct 95 10:14:29 PDT) - [Re: subjective names and MITM](/archive/1995/10/4bad5eb93a496d0d046d26b2a62982061b69cc2af56eabc07fc5ec42aebf3533) - _Hal \<hfinney@shell.portal.com\>_

