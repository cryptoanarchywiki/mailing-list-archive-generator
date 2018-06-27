---
layout: default
---

# 1992-11-28 - Re: More comments on dongles

## Header Data

From: yanek<span>@</span>novavax.nova.edu (Yanek Martinson)<br>
To: karn@qualcomm.com (Phil Karn)<br>
Message Hash: f4317e76cf7ec6b223d3ebaa786d5e6353bd6ecfe5fb28b6df16aa8fd6cdba9f<br>
Message ID: \<9211280343.AA07573@novavax.nova.edu\><br>
Reply To: \<9211280249.AA10136@servo\><br>
UTC Datetime: 1992-11-28 03:43:52 UTC<br>
Raw Date: Fri, 27 Nov 92 19:43:52 PST<br>

## Raw message

```
{% raw  %}From: yanek@novavax.nova.edu (Yanek Martinson)
Date: Fri, 27 Nov 92 19:43:52 PST
To: karn@qualcomm.com (Phil Karn)
Subject: Re: More comments on dongles
In-Reply-To: <9211280249.AA10136@servo>
Message-ID: <9211280343.AA07573@novavax.nova.edu>
MIME-Version: 1.0
Content-Type: text/plain


I think we are using different terminologies, maybe even different
paradigms of how e-mail and other internet functions are accessed
by people.

In my terminology, "host" is the remote multiuser computer that is
on the internet, and provides access to users via dial-up modems,
local RS-232 terminals, and PC-s running terminal emulation programs.

The host could also be a BBS system (as in the case of FidoNet) which
provides mail forwarding for you.  It could be an on-line service
such as GENIE or Compu$erve.

Local equipment is the terminal, or Pc or Mac or whatever, that you 
use to connect to the host.  It could also be the laptop that you
connect to a cellular modem and connect to the host while mobile.

You could always use the same local equipment.  Or you may use different
types at different times (a terminal at work, a PC connected through
a modem from home, a firend's Mac, a borrowed laptop using a
cellular modem, etc).

The connection could be direct, as in the case of a terminal or
a direct dial-up by modem.

Or the connection could go through multiple channels.  For example
you could dial up a TYMNET POP, and then connect to your host.  Or,
you could call up a terminal server, log in to a guest account, and
then telnet or rlogin to your host.

In this scheme, the dongle sits right between the local equipment and
the connection.

> >The way I envision it, the host must NOT have the ability to turn it on
> >or off or do any of the other things you mentioned.  The assumption is
> >that you DON't trust the host.
> 
> If you don't trust the host, then why are you running your plaintext
> through it?

In view of what I have said above, I am NOT running the plaintext through
the host.  I am running it through local equipment, which I may or may
not trust.  The host (being the multiuser system, administered by 
someone else) is always less trustworthy.  It is directly on the network/
It could be immediately transmitting everything you type to NSA for all
you know.

> ...  if the worst that can happen is that the only slightly sensitive
> plaintext I'm working on at the moment is compromised. ...
> But I would probably NOT be willing to trust the same PC with my
> secret key, because it would compromise EVERYTHING I have ever ...
> Do you understand the distinction here?

Yes, I certainly do.  That is the reason for having a portable trusted
device in the first place.  But, in this sense our two approaches (my
smart dongle that does all the crypto functions, and yours that only
stores the private key) are absolutely equivalent.  None of the two
exposes the private key in any way.

> >So if the host does not even need to know the dongle exists, it is
> >automatically independent of what type of computer, operating system,
> 
> I seriously doubt this will be practical, even with constant
> interaction with the dongle's keyboard. 

See my next post "STORY: scenario of use of Crypto-Dongle" for my
vision on how this would work.  Then, if you see any problems with
it, or suggestions for improvement, please let me know, so I can
improve it.

> to truly sensitive things, like typing in my pass phrase to decrypt my
> RSA secret key, or perhaps hitting a key to re-enable the device after

That is the kind of things I intend the keypad to be used for.

> Most palmtop keyboards are a real pain to use ...

The dongle will have a numeric keypad, somewhat like the touch-tone 
phone, with letters on the number keys, and a couple of extra keys
such as * and # for functions. 

> >Again, you are trusting the host.  What if the decryption program on 
> 
> As I said earlier, your "fully-functional dongle" fails to prevent

This misunderstanding is due to our differing use of the word "host". 
When you said the host would send the rsa-encrypted key to the dongle,
receive the decrypted session key, and then decrypt the file, I 
understood you as meaning that the remote multiuser machine is doing
all this.  

Now I see that you meant for the local equipment to perform the decryption.

The problem with this is that you are depending on every piece of local
equioment to have a copy of the decryption program, and every version
of that program compatible with your dongle's commands structure and
key format.  Or you'd have to carry a several disks with you, with a
version of your software for every platform you could encounter.

> >Once the host decrypts the file (at a high speed, as you say), you want
> >to view the file, right?  That means the plaintext is transmitted from
> >the host to you.  Anywhere in the link (which could be a simple RS-232

> Eh? The model I have is a local PC, possibly hacked, with a serial
> port connected to my personal dongle sitting right beside it.

In this case, you would have to save the encrypted message into a file
on the host, download it to your local machine, and then decrypt it
using the above approach.  This would be some amount of hassle, when 
compared to just using the mail reader software on the host.

--
Yanek Martinson    mthvax.cs.miami.edu!safe0!yanek     uunet!medexam!yanek
this address preferred -->> yanek@novavax.nova.edu <<-- this address preferred
Phone (305) 765-6300 daytime   FAX: (305) 765-6708  1321 N 65 Way/Hollywood
      (305) 963-1931 evenings       (305) 981-9812  Florida, 33024-5819




{% endraw %}
```

## Thread

+ Return to [November 1992](/archive/1992/11)

+ Return to "[karn<span>@</span>qualcomm.com (Phil Karn)](/authors/karn_at_qualcomm_com_phil_karn_)"
+ Return to "[yanek<span>@</span>novavax.nova.edu (Yanek Martinson)](/authors/yanek_at_novavax_nova_edu_yanek_martinson_)"

+ 1992-11-28 (Fri, 27 Nov 92 18:49:41 PST) - [Re: More comments on dongles](/archive/1992/11/7d25aa61587f97f0d78c37e496c31fcbff8f3f30f0ca4b2f37b920fae653cc7c) - _karn@qualcomm.com (Phil Karn)_
  + 1992-11-28 (Fri, 27 Nov 92 19:43:52 PST) - Re: More comments on dongles - _yanek@novavax.nova.edu (Yanek Martinson)_

