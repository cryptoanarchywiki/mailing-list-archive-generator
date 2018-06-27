---
layout: default
---

# 1998-10-08 - Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)

## Header Data

From: Adam Back \<aba<span>@</span>dcs.ex.ac.uk\><br>
To: fod@brd.ie<br>
Message Hash: 1c4bf161f1aee9ddcdf6cc6285bb823ce63bec071f052cefbecebd635d40f972<br>
Message ID: \<199810081945.UAA14149@server.eternity.org\><br>
Reply To: \<361CE49F.C858A2CE@brd.ie\><br>
UTC Datetime: 1998-10-08 20:36:37 UTC<br>
Raw Date: Fri, 9 Oct 1998 04:36:37 +0800<br>

## Raw message

```
{% raw  %}From: Adam Back <aba@dcs.ex.ac.uk>
Date: Fri, 9 Oct 1998 04:36:37 +0800
To: fod@brd.ie
Subject: Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)
In-Reply-To: <361CE49F.C858A2CE@brd.ie>
Message-ID: <199810081945.UAA14149@server.eternity.org>
MIME-Version: 1.0
Content-Type: text/plain




Frank O'Dwyer writes:
> I'm familiar with C2Net. If Stronghold is any good, that is because
> C2net and/or the Apache team know what they are doing, not just because
> they picked up a free SSL library on the net. It's easy to build
> insecure products on good crypto, and many other companies are busy
> doing just that. 

Perry recently posted a summary of his views on the appropriateness of
GPL vs BSD vs other licenses for achieving various aims, "free
software" under the GNU meaning, vs crypto software deployment.  I
found Perrys summary to be the clearest on the topic so far.

You appear to be arguing with another aim in mind.  You seem to be
arguing that the primary goal should be to have best security, from
the outset.  ie one gets the impression from reading your previous two
posts that you consider ultimate security more important than
deployment.  If this is what you are saying, I disagree.

As I argued further down, I think cypherpunk type goals are better met
my getting people to deploy first, then if they bodge it to encourage
them to fix it, and I gave the example of the Netscape RNG weakness
which was very quicly fixed once it was found:

> > Cypherpunks also get involved in breaking crypto, and this is usually
> > enough to get massively commercially deployed strong crypto with
> > unintentional flaws converted quickly into massively deployed crypto
> > without the flaws.  eg. Netscape's random number generator weakness,
> > which netscape fixed immediately.
> 
> That's condescending and irrelevant. Did anyone ever fix web spoofing?

Which is not in the least condescending or irrelevant as it gives an
example showing that having what turns out to be less than perfect
security can be fairly quickly remedied.  And security is hard, even
competent people make mistakes.  The important thing is to admit and
quickly fix such mistakes.

I've taken your comments on web spoofing to another post.

> Then I guess you agree that closed-source deployment is neither
> necessary nor sufficient to achieve "strong crypto". Not really sure why
> you're arguing in that case.

I don't think anyone suggesed that closed source deployment was in
anyway better than open source, and obviously open source is better
for verifying the quality of crypto software.

However, as was previously suggested, if deployment is the goal, and
if one uses for example a GNU license it tends to discourage
commercial (typically closed source) deployers, and as Lucky said:

: Many companies will not be able to source contaminated by GNU-style
: licensing restrictions. Consequently, alternatives would be
: found. Some of those alternatives, include using no crypto at all or
: using crypto written by somebody that does not understand
: crytography.  Hardly the outcome a Cypherpunk would desire.

And I think at this stage something is vastly better than nothing.

> > You don't get it, but then have you ever written any crypto code with
> > the objective of undermining the power of the state?  Is this your aim
> > in writing your open source application code that you name dropped?
> 
> Yes, and yes. 

Cool, what application area are these in?  Got a URL?

> (I don't think you understand the term "name dropped" btw.  

Just a comment on the Rick Smith (of Secure Computing) syndrome (read
crytopgraphy list you'll know about the book he wrote, because every
other post he makes involves it).  Perhaps not appropriate in your
case, but if people mention software, it is nice to know some details:
why should we be interested in your software etc.

> But given the name-dropping and appeal-to-authority tone of your
> whole post, I wonder if you understand the term "irony").

Irony?  Your post was intended to be ironic?  What is ironic about
arguing that first cut security is more important than deployment?

This is cypherpunks, people tend to speak their mind, and usually
aren't too delicate about it -- welcome to the cypherpunks list.

Adam
-- 
print pack"C*",split/\D+/,`echo "16iII*o\U@{$/=$z;[(pop,pop,unpack"H*",<>
)]}\EsMsKsN0[lN*1lK[d2%Sa2/d0<X+d*lMLa^*lN%0]dsXx++lMlN/dsM0<J]dsJxp"|dc`




{% endraw %}
```

## Thread

+ Return to [October 1998](/archive/1998/10)

+ Return to "[Adam Back <aba<span>@</span>dcs.ex.ac.uk>](/authors/adam_back_aba_at_dcs_ex_ac_uk_)"
+ Return to "[Bill Frantz <frantz<span>@</span>netcom.com>](/authors/bill_frantz_frantz_at_netcom_com_)"
+ Return to "["Frank O'Dwyer" <fod<span>@</span>brd.ie>](/authors/frank_odwyer_fod_at_brd_ie_)"
+ Return to "["Jim McCoy" <mccoy<span>@</span>yahoo-inc.com>](/authors/jim_mccoy_mccoy_at_yahooinc_com_)"
+ Return to "[Lucky Green <shamrock<span>@</span>netcom.com>](/authors/lucky_green_shamrock_at_netcom_com_)"
+ Return to "[Richard Stallman <rms<span>@</span>gnu.org>](/authors/richard_stallman_rms_at_gnu_org_)"

+ 1998-10-07 (Thu, 8 Oct 1998 04:06:20 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source   code)](/archive/1998/10/baf74756cfea7b417c75051bb1a9fd52f3479c1819652d04e3a2590fcfa0d95a) - _"Jim McCoy" \<mccoy@yahoo-inc.com\>_
  + 1998-10-07 (Thu, 8 Oct 1998 06:59:35 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source   code)](/archive/1998/10/7f92d43a9d8190926a12c834b3251dbc796b6cb279f4f0e579e8a1e79b9fe054) - _"Frank O'Dwyer" \<fod@brd.ie\>_
    + 1998-10-08 (Thu, 8 Oct 1998 09:36:08 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)](/archive/1998/10/bf164f61234475646b77b3d2d00ed4dbcf9d12571cac7a2527188e16c914cea8) - _Lucky Green \<shamrock@netcom.com\>_
      + 1998-10-08 (Thu, 8 Oct 1998 20:42:54 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)](/archive/1998/10/9c577728f8f02a44739b3770a10e3467b42f4f9f45c5cee8eb550873c2ec2fac) - _"Frank O'Dwyer" \<fod@brd.ie\>_
        + 1998-10-08 (Thu, 8 Oct 1998 22:29:53 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)](/archive/1998/10/dccb405fbfd8981c05ee00b71e5a8fe7dab2f96f4f7c24e62ab5479ec9cff9d5) - _Adam Back \<aba@dcs.ex.ac.uk\>_
          + 1998-10-08 (Fri, 9 Oct 1998 00:39:32 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)](/archive/1998/10/7a7e019cfbf8f2f0315517c9532fb6a9e569d91737c752d6d4b04943f0bc7e59) - _"Frank O'Dwyer" \<fod@brd.ie\>_
            + 1998-10-08 (Fri, 9 Oct 1998 04:36:37 +0800) - Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code) - _Adam Back \<aba@dcs.ex.ac.uk\>_
              + 1998-10-08 (Fri, 9 Oct 1998 06:50:44 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)](/archive/1998/10/0abc4e18047ab7a766e17272506967dbe8ee228deba3a8e5a3bd4c767468afe5) - _"Frank O'Dwyer" \<fod@brd.ie\>_
                + 1998-10-09 (Fri, 9 Oct 1998 08:09:09 +0800) - [importance of GUIs / secure distributed IRC (Re: propose: `cypherpunks license')](/archive/1998/10/7830e125270ca3aa35eec3acea5b043d26778a367dc97ee29eb0665119463a4a) - _Adam Back \<aba@dcs.ex.ac.uk\>_
            + 1998-10-08 (Fri, 9 Oct 1998 04:36:48 +0800) - [HTTPS:// hyperlink spoofing (Re: propose: `cypherpunks license')](/archive/1998/10/4f3bccd1854b2ddb538c0883279f2462422b60bacea8927e95b38eb1d8d7a35b) - _Adam Back \<aba@dcs.ex.ac.uk\>_
      + 1998-10-08 (Fri, 9 Oct 1998 01:24:50 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish sourcecode)](/archive/1998/10/26bd73052790740646e0d70ad221d2260ec2072a2a41f97b09f2d750c43b3fe4) - _Bill Frantz \<frantz@netcom.com\>_
      + 1998-10-09 (Fri, 9 Oct 1998 08:45:02 +0800) - [Re: propose: `cypherpunks license' (Re: Wanted: Twofish source code)](/archive/1998/10/39cfc7f4dc761f4d7ef37010445e912b582b9b73f263fc4251a9a460f76f5dc9) - _Richard Stallman \<rms@gnu.org\>_

