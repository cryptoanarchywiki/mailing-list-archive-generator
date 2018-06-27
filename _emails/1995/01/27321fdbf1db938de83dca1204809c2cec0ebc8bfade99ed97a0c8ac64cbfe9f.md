---
layout: default
---

# 1995-01-30 - ESP Unix encrypted session protocol software

## Header Data

From: Matt Blaze \<mab<span>@</span>research.att.com\><br>
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
+ Return to [February 1995](/archive/1995/02)

+ Return to "[Alan Barrett <barrett<span>@</span>daisy.ee.und.ac.za>](/authors/alan_barrett_barrett_at_daisy_ee_und_ac_za_)"
+ Return to "[eric<span>@</span>remailer.net (Eric Hughes)](/authors/eric_at_remailer_net_eric_hughes_)"
+ Return to "[Matt Blaze <mab<span>@</span>research.att.com>](/authors/matt_blaze_mab_at_research_att_com_)"
+ Return to "["Perry E. Metzger" <perry<span>@</span>imsi.com>](/authors/perry_e_metzger_perry_at_imsi_com_)"
+ Return to "[Thomas Grant Edwards <tedwards<span>@</span>src.umd.edu>](/authors/thomas_grant_edwards_tedwards_at_src_umd_edu_)"

+ 1995-01-30 (Mon, 30 Jan 95 08:01:55 PST) - ESP Unix encrypted session protocol software - _Matt Blaze \<mab@research.att.com\>_
  + 1995-01-30 (Mon, 30 Jan 95 09:06:17 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/01/26090af98ef03986fa4a74739418b2ba8836d531598cf151084b98690c237850) - _Alan Barrett \<barrett@daisy.ee.und.ac.za\>_
  + 1995-01-30 (Mon, 30 Jan 95 09:42:48 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/01/9fcc5e9263c69c4345c8ebaa0936bbef5bd89d670c3847880f6b53354cce1406) - _Thomas Grant Edwards \<tedwards@src.umd.edu\>_
    + 1995-01-30 (Mon, 30 Jan 95 10:07:52 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/01/017385537ac16c731409f57893b21935a8377af8556f1f2bef4c998dcb0f8944) - _Matt Blaze \<mab@research.att.com\>_
      + 1995-01-30 (Mon, 30 Jan 95 11:23:32 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/01/be4c854c342e4b12b641ee208910429414aedeeeb6c9da407f7ba68a837b9544) - _Thomas Grant Edwards \<tedwards@src.umd.edu\>_
        + 1995-01-30 (Mon, 30 Jan 95 13:05:57 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/01/1593a6cb88c6b7bec6c6a4309e6f7978879d17a94451b927eea0fdfc3018393a) - _"Perry E. Metzger" \<perry@imsi.com\>_
          + 1995-01-31 (Mon, 30 Jan 95 23:56:13 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/01/d3ce194c9f81ed14e0b869fdd7834e8c4118acf44109fda9e52d86dfef9dc485) - _Alan Barrett \<barrett@daisy.ee.und.ac.za\>_
      + 1995-02-01 (Tue, 31 Jan 95 21:29:07 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/02/d3b6c2def416501b6c04a59d1900f189c1a8b62d79ae9afbddce742aa0fa7e74) - _eric@remailer.net (Eric Hughes)_
        + 1995-02-01 (Tue, 31 Jan 95 23:49:33 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/02/c5a409653c9e9cc0ac51d4feba5f5c58520f2d45117ee8b767ebed9c62fb9e92) - _Thomas Grant Edwards \<tedwards@src.umd.edu\>_
          + 1995-02-01 (Wed, 1 Feb 95 08:58:07 PST) - [Re: ESP Unix encrypted session protocol software](/archive/1995/02/5f992d1bb3e8ce71fd73bc52f90e36bde02744db97a930db7463e57db06674a0) - _eric@remailer.net (Eric Hughes)_

