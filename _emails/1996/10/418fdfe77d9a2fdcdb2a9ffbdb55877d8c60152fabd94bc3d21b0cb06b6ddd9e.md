---
layout: default
---

# 1996-10-18 - RE: Binding cryptography - a fraud-detectible alternative to  ke

## Header Data

From: everheul<span>@</span>mail.rijnhaave.nl<br>
To: cypherpunks@toad.com<br>
Message Hash: 418fdfe77d9a2fdcdb2a9ffbdb55877d8c60152fabd94bc3d21b0cb06b6ddd9e<br>
Message ID: \<199610181057.LAA11997@mail.rijnhaave.nl\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-10-18 10:57:45 UTC<br>
Raw Date: Fri, 18 Oct 1996 03:57:45 -0700 (PDT)<br>

## Raw message

```
{% raw  %}From: everheul@mail.rijnhaave.nl
Date: Fri, 18 Oct 1996 03:57:45 -0700 (PDT)
To: cypherpunks@toad.com
Subject: RE: Binding cryptography - a fraud-detectible alternative to  ke
Message-ID: <199610181057.LAA11997@mail.rijnhaave.nl>
MIME-Version: 1.0
Content-Type: text/plain


Bill Stewart[SMTP:stewarts@ix.netcom.com] wrote:
>I haven't seen the technical papers behind the postings you've made
Our original is on: http://cwis.kub.nl/~frw/people/koops/binding.htm
At the end of that (also available as
http://cwis.kub.nl/~frw/people/koops/bindtech.htm) there is a
technical description of one implementation of Binding Cryptography. 

>to the net, but the overall approach sounds very similar to "Clipper
>II", the Software Key Encryption work that the TIS people (Steve
>Walker?) and Dorothy Denning were touting a year or so ago.  It
>wasn't in your references, and it's clearly close enough to be worth
>your attention.  The design was interesting - it chose a set of
>public and symmetric key encryption that allows the recipient to
>validate the sessionkey-encrypted-to-key-copy-holder*.
They are mentioned  in the final paper.

/* I will only go into the technique now, not the politics */
In fact our technique is inspired on that technique (that is being
used by several other as well). In this technique users' encrypted
messages basically consist of three components:
1. the (actual) message encrypted with any symmetric system, using a random session
key;
2. the session key encrypted with the public key(s) of the
addressee(s);
3. the session key encrypted with the public key of a

Trusted Retrieval Party (TRP). With the TIS scheme a TRP is called Key
Escrow Agency (KEA), but that is just a name.

When a law-enforcement agency is conducting a lawful intercept and
strikes upon an enciphered message, they take the third information
component to the TRP. If shown an appropriate warrant, the TRP
decrypts the information component and hands over the session key, so
that the law-enforcement agency has access to the message. 

The TIS commerical Key Escrow (CKE) leaves it at that. So unilateral
(i.e without help of the recipient) fraud is easily possible; just
send another (or none) session key in the thrid component. Nobody is
going to know; the three packets look OK. Only when there is a
law-enforcement agency is conducting a lawful intercept then they will
know fraude is committed. (BTW "fraude" means using something
(voluntarily) without complying with the *AGREED* rules. Hence fraude
in voluntary systems is possible. PLEASE PLEASE PLEASE let us not have
that discussion again!). Not willing to jeopardize the investigation,
the LEA is then probably not going to do much about it.

In the "TIS software key escrow paralleling Clipper" this unilateral
fraude has been made impossible: as the recipient knows the session
key (from decrypting the second component), he is capabel to
recalculate the third session key and compare it with it the actual
sent to him. Of course this comparison is incorperated in the software
of the recipient; if the comparison fails then the decryption of the
first component will not take place (in France your monitor might
explode (-;) Although preventing unilateral fraude, this does not
prevent colluding of frauders. Indeed, by a conceptually simple
manipulation in the decryption software the outcome of the comparison
can be made "positive" all the time. So in this fashion, without
anybody knowing (seeing) about it colluding people will use the
security benefits of the system, but not it "law enforcement"
disadvantages.

We liked the general techinque as it is rather liberal and
internationally useable (you don't have to escrow any secret keys, the
choice of TRPs is very flexible), but we did not like the colluding
property. The idea in our scheme is that the colluding fraude is still
possible, but must be at least *detectable* by third parties that have
access to all data anyway (network operators, internet service
providers). Moreover, for this detection no secret information is
needed (or gained), so user' privacy is not jeopardized by it. With
respect to this; I was surprised to read in the papers that Bangemann
(European Commision) proposed to make Internet Service Provides
responsible for checking the authenticity of certain types of sent
data.

In resume: we believe that our scheme is the middle of key-escrow
(Clipper III) and the TIS scheme and is flexible enough to form a
worldwide security infrastructure, where each participating country
can implement its *own* crypto policy with. In particular, if, how
(random, offline?) and by who checking is done is a matter for each
country to decide on his own. Also the organization of TRPs is a
matter of each country of its own.

> A major capability that was missing from Walker's SKE work is the
> ability to split the copied* key into two or more parts, all of
> which are need to recover the session key, while making it possible
> to validate that the pieces do add up to the session key.  

Splitting the session-key in binding data can be done by the sender
(sending all shares to different TRPs); this can be checked by anyone.
More importantly, in our ElGamal implementation of binding
cryptography the splitting of the secret keys of TRP can be done in a
very elegant way, that seems to be put there for (controlled) LEA-use. We will put
that in the technical paper as well.

Best regards, Eric




{% endraw %}
```

## Thread

+ Return to [October 1996](/archive/1996/10)

+ Return to "[everheul<span>@</span>mail.rijnhaave.nl](/authors/everheul_at_mail_rijnhaave_nl)"

+ 1996-10-18 (Fri, 18 Oct 1996 03:57:45 -0700 (PDT)) - RE: Binding cryptography - a fraud-detectible alternative to  ke - _everheul@mail.rijnhaave.nl_

