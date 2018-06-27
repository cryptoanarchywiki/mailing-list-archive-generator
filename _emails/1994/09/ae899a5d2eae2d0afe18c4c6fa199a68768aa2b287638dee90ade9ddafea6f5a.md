---
layout: default
---

# 1994-09-28 - Re: SUFFERANCE remailers

## Header Data

From: jamiel<span>@</span>sybase.com (Jamie Lawrence)<br>
To: "Gary Jeffers" \<CCGARY@MIZZOU1.missouri.edu\><br>
Message Hash: ae899a5d2eae2d0afe18c4c6fa199a68768aa2b287638dee90ade9ddafea6f5a<br>
Message ID: \<aaaf52df000210034e7e@[130.214.233.13]\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-09-28 18:02:26 UTC<br>
Raw Date: Wed, 28 Sep 94 11:02:26 PDT<br>

## Raw message

```
{% raw  %}From: jamiel@sybase.com (Jamie Lawrence)
Date: Wed, 28 Sep 94 11:02:26 PDT
To: "Gary Jeffers" <CCGARY@MIZZOU1.missouri.edu>
Subject: Re: SUFFERANCE remailers
Message-ID: <aaaf52df000210034e7e@[130.214.233.13]>
MIME-Version: 1.0
Content-Type: text/plain


At 8:11 PM 9/27/94, Gary Jeffers wrote:

>   Anybody got any idea at all how to build a Fortress remailer?

As I see it, the main things one must defend a single machine
acting as a remailer against are physical accesibility, denial
of service and violation through monitoring mail flow.

The physical accesibility problem is tricky, but obviously has
been done for other physical items.. Stick it somewhere secret.
Of course you can't know how secret it is until someone tries
to find it. Wireless communication, as others pointed out, are
pretty nessessary for this.

The other two problems are software, and have been discussed quite
a bit here.

The answers above aren't bery compelling, and I don't see much way
around this. Groups with large amounts resources are typically good
at finding things when they put thier minds to it.

The solution here, and I think this has been talked about here, too,
is to create redundant destributed remailers.

Issues here are trust, protocol and availability.

Trust could be developed through the web of trust method, encouraged
by existing remailers using this protocol, but the key issue is being
able to trust a message going over potentially insecure remailer nodes
can be considered valid if delivered. That way if Julf ends up being a
under-deep-cover NSA agent and this hypothetical remailer-web is infested
with bad-guys, there is still nothing they can do except render a message
undeliverable.

I'm trying to come up with something good here, but am still working
on it. The vision I have for remailers in a perfect world is that
everyone runs one and bounces around message 'packets' (small parts of
the message (all signed and encrypted multiple times, of course)
according to specific instructions. In a less than perfect world,
a smaller network running this method could be created.

This takes the form of the originator dumping the message into the
stream, and forwards them off to some other sites. The message would
be split into small packets which are encrypted multiple times to
multiple different sites into the stream. This would probably have
to be done by software, as it would be a complex task to manually
split, encrypt etc. any but the smallest message. The software would
need to be kept up to date about all potential public keys to encrypt
to, and need to pick a set at random from this info. It would also
insert routing intstructions as needed.

The next site checks to see if it can decrypt the packet it
recieves. If it can, it does so and  sends it forwards it somewhere
else, and repeat. If not, it just sends it onward. This continues for
n layers of encryption for each packet, with the final message in the
form of x packets encrypted only once ending up at the proper destination,
which reassembles  the message. All remailers reorder packets and insert
noise as apporpriate.

Obvious problems are bandwidth, time delay and having a site the
message was signed to go down. The last issue can be taken care of
by having group keys for this purpose, so that a given layer of
encryption can be decrypted by any one of n sites with key m. This
adds the problem of someone collecting all the keys and being able
to crack the whole thing, but I think this is surmoutable.

Band width and time delay stem from the same problem, and obviously
this system would never work on the internet as it stands. If this
web were, say, 300 sites worldwide, then they could work conjunction
with the pre- existing remailers now available.

Also, if the network grew to the point where it was impracticle to bounce
at random, intermediate steps could be added, such as 'send me to austalia'
or 'send me to mafiaNet', which would then cut down the number of bounces
before a layer of decription was achived.

As far as availability, well, it doesn't exist.

Comments? Is this dumb? Did I just duplicate someone elses idea?





{% endraw %}
```

## Thread

+ Return to [September 1994](/archive/1994/09)

+ Return to "[jamiel<span>@</span>sybase.com (Jamie Lawrence)](/authors/jamiel_at_sybase_com_jamie_lawrence_)"

+ 1994-09-28 (Wed, 28 Sep 94 11:02:26 PDT) - Re: SUFFERANCE remailers - _jamiel@sybase.com (Jamie Lawrence)_

