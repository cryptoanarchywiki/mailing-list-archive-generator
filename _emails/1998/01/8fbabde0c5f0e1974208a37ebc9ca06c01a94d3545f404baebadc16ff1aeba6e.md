---
layout: default
---

# 1998-01-16 - Eternity - an alternative approach

## Header Data

From: Kay Ping \<kping<span>@</span>nym.alias.net\><br>
To: cypherpunks@toad.com<br>
Message Hash: 8fbabde0c5f0e1974208a37ebc9ca06c01a94d3545f404baebadc16ff1aeba6e<br>
Message ID: \<19980116220255.3116.qmail@nym.alias.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1998-01-16 22:28:53 UTC<br>
Raw Date: Sat, 17 Jan 1998 06:28:53 +0800<br>

## Raw message

```
{% raw  %}From: Kay Ping <kping@nym.alias.net>
Date: Sat, 17 Jan 1998 06:28:53 +0800
To: cypherpunks@toad.com
Subject: Eternity - an alternative approach
Message-ID: <19980116220255.3116.qmail@nym.alias.net>
MIME-Version: 1.0
Content-Type: text/plain



-----BEGIN PGP SIGNED MESSAGE-----

In one of the messages on the eternity thread someone suggested using
radio signals. This is an interesting approach which certainly deserves
further attention but digital radio requires special hardware which I prefer 
to avoid. However, some of the characteristics of radio signals can be 
emulated on the internet.

Radio links are perfect for hiding the location of receivers. The
equivalent for this is of course services like usenet and IRC. Both are
already used for providing anonymity.

Radio is also quite good at hiding the location of the transmitter - you
tune your radio and the signals are just there, coming down your antenna.
It takes special equipment to locate where they originated.

It occured to me that the equivalent on the net would be to receive
packets with invalid source addresses. They are just there, coming dowm
the phone line to your modem. It takes significant resources and snooping
on a massive scale to locate where they are coming from.. All this is
assuming you can find some way to send a request with your address to the
server.

For eternity this means that the location of servers where documents are
stored can be kept secret if they transmit the documents using packets
with invalid source addresses. Receivers of eternity documents will not
be able to tell where they are coming from.

Since there is no bidirectional link between transmitter and receiver the
protocol must be implemented over UDP. To protect against packet loss the
data may be encoded with redundancy. The correction code can be similar
to that used on RAID disk arrays - adding redundant blocks consisting of
XOR of other blocks. Missing blocks can be reconstructed by XORing
together other blocks received.

To provide even better anonymity the transmitter may send the messages
through one or more onion routers which decrypt one layer of encryption.
These routers do not store information, do not know what information
passes through them and do not know where it's coming from. Any packets
they forward are sent without a valid source address. This should make
them less vulnerable to attacks of all kinds. Can anyone speculate about
their liability under US law?

Putting caches on the routers will help both performance and security.
Will it affect their liability in any way?

If encryption is implemented properly all packets will look identical:
blocks of random data of the same size and no source address. This will
make traffic analysis difficult. The distance to the transmitter can be
hidden by initializing the packet's time-to-live field to a value with
random variations.

That was the easy part. The hard part is to get the requests to the
document servers without knowing their addresses. This can be done
through the equivalent of remailer reply blocks or some kind of broadcast
medium.

The reply blocks would be implemented by the onion routers. Each hop
could generate several copies, both for redundancy and as decoys.
Packets used in reply blocks can look identical to packets with document
data, including the use of invalid source addresses.

In the broadcast version clients and servers subscribe to channels with
many participants to hide their identity in the crowd. The system could
use an existing service like IRC or a dedicated network, possibly based
on modified IRC server code.

Sympathizers with bandwidth to spare can subscribe too to provide better
cover for the actual document servers. Servers could listen using trusted
proxies or chains of semi-trusted proxies. The division into channels
allows growth of the system if the total bandwidth of requests becomes
too high.

Using the public IRC networks has the advantages of being less suspicious
and not requiring the deployment of new infrastructure. Requests could
even be hidden steganographically in IRC traffic. Unfortunately, IRC
server operators are touchy about abuse of their systems.

Requests should be small. This allows replicating them to a large number
of receivers without taking too much bandwidth. They can also be made to
be of fixed size and contain no controversial information. Requests
contain the document index as a compact one-way hash, the requester's IP
address and the server's ID code. It may also contain hashcash or ecash
payment. Requests should be encrypted to the server's public key. To keep
them small, elliptic curve encryption may be used.

A server may send random cover packets to hide the correlation between
a request and its response. It may also add random delay before
responding to the request. Delay will also help limit the bandwidth.
Users of eternity need to be more patient that the average web surfer and
the protocol should use generous timeouts. Since UDP has no flow control
the server should always assume the client is using a modem connection
and limit its transmission speed accordingly. Security has a price.

The client software may be implemented as a local web proxy (in Java?)
which identifies requests to eternityspace and converts them to this
protocol. Public gateways may be set up to allow anyone to read eternity
URLs. These public may also be used to protect the anonymity of the
reader like the Anonymizer.

Document servers and routers must be located on networks where there is
no spoofed packet filtering. Since the common use of spoofed packets is
in denial-of-service attacks more and more filters are being installed.
It may become harder in the future to find places to put the servers and
routers. I believe it should always be possible since it is not practical
to implement filtering in places where there is a lot of traffic from
different sources. In cases where the document server is located on a
filtered network it may have to trust the routers to hide its location.

This system is far from perfect: it has too many components and the weakest link is the transmission of requests to servers. I still believe it has some interesting sides which deserve further discussion. Your ideas are welcome.

- -----------------
Kay Ping 
nop 'til you drop

finger kping@nym.alias.net for key
DF 6D 91 18 A6 59 41 96 - 89 01 69 B7 9D0 4 AE 53

-----BEGIN PGP SIGNATURE-----
Version: 2.6.3ia
Charset: cp850

iQEPAwUBNL26txHPAso8Qp7tAQGLEAfPeRgIL3OqiG67CLBO9TCe/oV5lmw66Pz1
Wl17ajHeSCX6qjACSZ3La73drUjIftL0G/18PkLd48VGmsF6izCnXB4fh8MAB6Ve
QWjhRTvRSkKkwXK4t2tx6CUCdxOaJ9Phd6J02Z+MdjEGJ3jAdUdaHWo5zM5i6Ris
wkgATEhGMpw8tjlnvR4erwu51iSrt62huPWJXl1pjyPfQbl0iyQtcGdQ1spIWLJC
oaOI7QchHK3LjSuzN54MVCjRdz8fiI6JHAUnlqqsW29LBOZQkSnQedORCuIALwqe
qOhSxMKbciLdVde3BBtpILpz5y91ulAecxOOwcnc7m5Pjw==
=iLP5
-----END PGP SIGNATURE-----






{% endraw %}
```

## Thread

+ Return to [January 1998](/archive/1998/01)
+ Return to [December 1998](/archive/1998/12)

+ Return to "[? the Platypus {aka David Formosa} <dformosa<span>@</span>st.nepean.uws.edu.au>](/author/_the_platypus_aka_david_formosa_dformosa_at_st_nepean_uws_edu_au_)"
+ Return to "[Dave Emery <die<span>@</span>die.com>](/author/dave_emery_die_at_die_com_)"
+ Return to "[Eric Blossom <eb<span>@</span>comsec.com>](/author/eric_blossom_eb_at_comsec_com_)"
+ Return to "[Kay Ping <kping<span>@</span>nym.alias.net>](/author/kay_ping_kping_at_nym_alias_net_)"
+ Return to "[Markus Kuhn <Markus.Kuhn<span>@</span>cl.cam.ac.uk>](/author/markus_kuhn_markus_kuhn_at_cl_cam_ac_uk_)"
+ Return to "[Steve Schear <schear<span>@</span>lvcm.com>](/author/steve_schear_schear_at_lvcm_com_)"

+ 1998-01-16 (Sat, 17 Jan 1998 06:28:53 +0800) - Eternity - an alternative approach - _Kay Ping \<kping@nym.alias.net\>_
  + 1998-01-17 (Sun, 18 Jan 1998 01:27:41 +0800) - [Locating radio receivers](/archive/1998/01/4d5f6d5e429e677c0901458538000f6c5d976d11ed5e983cbedb0e4979ecd2a8) - _Markus Kuhn \<Markus.Kuhn@cl.cam.ac.uk\>_
    + 1998-01-19 (Tue, 20 Jan 1998 06:42:42 +0800) - [Re: Locating radio receivers](/archive/1998/01/40540270a95c1bf7037f31ff78fc31d40df73b28e08a3be90407bafaaad6f0d0) - _Eric Blossom \<eb@comsec.com\>_
      + 1998-12-27 (Sun, 27 Dec 1998 14:05:43 +0800) - [Re: Locating radio receivers](/archive/1998/12/1b4320a25c52151f7009884b830715a0b167b8a8fab0684ed7a7498726281c9d) - _Steve Schear \<schear@lvcm.com\>_
    + 1998-01-20 (Tue, 20 Jan 1998 14:58:51 +0800) - [Re: Locating radio receivers](/archive/1998/01/c1a533ac89582a901d7aada743c7d4452704e67b78dd62143eade3ea9f4f77f4) - _Dave Emery \<die@die.com\>_
    + 1998-01-21 (Wed, 21 Jan 1998 15:40:00 +0800) - [Re: Locating radio receivers](/archive/1998/01/219ec7c9034c6371ec776df977be50f8b356e7b4bcab844c235d916b17ca98cb) - _? the Platypus {aka David Formosa} \<dformosa@st.nepean.uws.edu.au\>_

