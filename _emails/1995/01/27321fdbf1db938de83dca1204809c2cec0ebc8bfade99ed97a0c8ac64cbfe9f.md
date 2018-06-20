---
layout: default
---

# 1995-01-30 - ESP Unix encrypted session protocol software

## Header Data

From: Matt Blaze \<mab@research.att.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: 27321fdbf1db938de83dca1204809c2cec0ebc8bfade99ed97a0c8ac64cbfe9f<br>
Message ID: \<9501301554.AA08155@merckx.info.att.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-01-30 16:01:55 UTC<br>
Raw Date: Mon, 30 Jan 95 08:01:55 PST<br>

## Raw message

```
{% raw  %}From: Matt Blaze <mab@research.att.com>
Date: Mon, 30 Jan 95 08:01:55 PST
To: cypherpunks@toad.com
Subject: ESP Unix encrypted session protocol software
Message-ID: <9501301554.AA08155@merckx.info.att.com>
MIME-Version: 1.0
Content-Type: text/plain


Folks,

I'm releasing, for experimental use, source code for a preliminary
version of my simple Unix->Unix encrypted terminal session manager,
ESP.  Basically, ESP provides a pseudo-terminal interface to a local
shell session that you can use to establish an encrypted terminal
session with a another, remote machine.  (See the README file below
for usage examples).  Once the bugs are shaken out, ESP will become
part of my CFS package, which will eventually grow into a larger
suite of free, practical tools for secure internetworked computing.
At the present time, I'm just releasing a "pre-release" to small
groups, including interested folks on the cypherpunks list.

I've tested ESP under BSDI and SunOS 4.x; you'll also need RSAREF 2.0
(from rsa.com) to compile it.  You're on your own for other platforms.
This release is NOT production software; it is by no means "ready for
prime time".  It's slow (reduces bandwidth by 50% and takes 45 seconds
to start up).  The user interface needs a bit of work, and you really
have to know what's going on to make effective use of it.  Future
versions of ESP will use a more efficient encoding and will add
features like a "palmtop" mode that allows secure remote entry of
things like passwords from dumb terminals with the encryption done on
a disconnected palmtop machine.  I hope to eventually have a PC
terminal client as well.  This version, however, only supports
Unix->Unix terminal sessions.

Because of export restrictions (and a large cabal of paranoid, rabid
lawyers watching my every move), I'm not able to send ESP out of the
US or Canada or make it available by anonymous ftp.  Sorry.  If you
want a copy of the ESP-beta sources, send an Email message to
cfs@research.att.com (NOT mab@research.att.com) telling me the
following:
	- that you're in the US or Canada, and
	- that you're a US or Canadian citizen or legal permanent
	  resident, and
	- that you've read and understand the license and export
	  conditions in the README file below.

Remember, you also need to get RSAREF 2.0 to build ESP.

-matt


========================= ESP README ==============================
This is Version 0.5c (BETA) of ESP, the Encrypted Session Protocol.

 * The author of this software is Matt Blaze.
 *              Copyright (c) 1995 by AT&T.
 * Permission to use, copy, and modify this software without fee
 * is hereby granted, provided that this entire notice is included in
 * all copies of any software which is or includes a copy or
 * modification of this software and in all copies of the supporting
 * documentation for such software.
 *
 * This software is subject to United States export controls.
 *
 * THIS SOFTWARE IS BEING PROVIDED "AS IS", WITHOUT ANY EXPRESS OR IMPLIED
 * WARRANTY.  IN PARTICULAR, NEITHER THE AUTHORS NOR AT&T MAKE ANY
 * REPRESENTATION OR WARRANTY OF ANY KIND CONCERNING THE MERCHANTABILITY
 * OF THIS SOFTWARE OR ITS FITNESS FOR ANY PARTICULAR PURPOSE.

ESP is an encrypted session protocol layer for managing remote
encrypted sessions.  It does 1024 bit DH key exchange (from RSAREF)
and 3-des in 8bit cfb mode for the traffic encryption.  See the
man page (esp.1 in this distribution).

To compile ESP you'll need the RSAREF 2.0 library, available for free
for non-commercial use in the US and Canada from RSA Laboratories
(anonymous ftp to rsa.com for details).

Once you have RSAREF working, this distribution should compile without
problems under SunOS 4.x and BSDI; you're on your own with other platforms.

The best way to explain esp is with an example.  Here's
an encrypted session from alice to bob:

	alice$ esp
	ESP v0.5 - encrypted session protocol layer
	    by Matt Blaze, AT&T Bell Labs, January 1995
	Randomizing (takes about 45 secs)......................done
	local layer ready (run 'esp -s' on remote)
	alice$ rsh bob
	bob$ ./esp -s                                          
	ESP v0.5 - encrypted session protocol layer
	    by Matt Blaze, AT&T Bell Labs, January 1995
	Randomizing (takes about 45 secs)......................done
	remote server ready
	Starting remote side of 1024 bit key exchange.
	~~L
	Starting local key exchange.
	entering ENCRYPTED mode; type ctrl-^ to escape
	bob$
	...
	[encrypted session from alice to bob]
	...
	bob$ exit
	Press <enter> to return CLEARTEXT mode:
	bob$ exit
	alice$ 

You can also use ESP to provide an encrypted login session;
simply create a user "esp" with "esp -s -e login" as the login
shell.  (Getting this to work properly will require some tweaking
on your local system). Run esp -l on the local machine and from
there log in to the esp account on the remote machine.  Such a
configuration encrypts the real account name and password over
the network:

	alice$ esp                                  
	ESP v0.5 - encrypted session protocol layer
	    by Matt Blaze, AT&T Bell Labs, January 1995
	Randomizing (takes about 45 secs)......................done
	local layer ready (run 'esp -s' on remote)
	alice$ telnet bob
	Trying 123.45.67.12...
	Connected to bob
	Escape character is '^]'.

	bob login: esp
	ESP v0.5 - encrypted session protocol layer
	    by Matt Blaze, AT&T Bell Labs, January 1995
	Randomizing (takes about 45 secs)......................done
	remote server ready
	Starting remote side of 1024 bit key exchange.
	~~L
	Starting local key exchange.
	entering ENCRYPTED mode; type ctrl-^ to escape
	login: mab
	Password:
	bob$
	...

It's primitive and slow, but seems to work.  Comments, bug fixes,
ports to new platforms and complaints are welcome.

Matt Blaze
mab@research.att.com
(for esp or cfs questions, use cfs@research.att.com).




{% endraw %}
```

## Thread

+ Return to [January 1995](/archive/1995/01)

+ 1995-01-30 (Mon, 30 Jan 95 08:01:55 PST) - ESP Unix encrypted session protocol software - _Matt Blaze \<mab@research.att.com\>_
  + 1995-01-30 (Mon, 30 Jan 95 09:06:17 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/01/26090af98ef03986fa4a74739418b2ba8836d531598cf151084b98690c237850) - _Alan Barrett \<barrett@daisy.ee.und.ac.za\>_

