---
layout: default
---

# 1997-10-15 - Document on Customizing OpenBSD after install

## Header Data

From: Marshall Midden \<m4<span>@</span>nts.umn.edu\><br>
To: tech@openbsd.org<br>
Message Hash: fdb841b89ed5ab0afbf93eadf9872788bc7a5e5ddad9ea39d7586b1eade31da8<br>
Message ID: \<199710152020.PAA24415@unet.unet.umn.edu\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-10-15 23:03:42 UTC<br>
Raw Date: Wed, 15 Oct 1997 16:03:42 -0700 (PDT)<br>

## Raw message

```
{% raw  %}From: Marshall Midden <m4@nts.umn.edu>
Date: Wed, 15 Oct 1997 16:03:42 -0700 (PDT)
To: tech@openbsd.org
Subject: Document on Customizing OpenBSD after install
Message-ID: <199710152020.PAA24415@unet.unet.umn.edu>
MIME-Version: 1.0
Content-Type: text/plain


Is there a checklist someplace on what to do after the install of OpenBSD 2.2?

I'm thinking like:
   1) Go into /etc
	a) Verify disks and network interfaces configured correctly.
	   Files: fstab, hosts, myname, hostname.le0, mygate, resolv.conf, defaultdomain.
	   You might wish to turn off multicast routing in /etc/netstart.
	b) Edit motd to make lawyers comfortable and delete "Welcome".
	c) Fix passwd via "vipw" to change passwords, set up users, etc.
	   Make sure password on "root".  Default is no password from console, and
	   disabled from network.  Make sure to edit "group" for any user groups,
	   and to put people into the wheel group if they need root access.
	d) Any local configuration change in: rc.conf, rc.local
	e) printcap, hosts.lpd	Get printers set up
	f) Tighten security:
		fbtab		Set security for X
		inetd.conf	Turn off extra stuff, add that which is really needed.
		rc.securelevel	Turn on Network Time Protocol.
	g) kerberosIV		Get kerberos configured.  Remember to get a srvtab.
	h) aliases		Local mail delivery (set postmaster, etc).  Run newaliases
	   after changes.
	i) bootptab		If this is a bootp server.
	j) ccd.conf		If using concatenated disks (striped, etc).
	k) exports		If this is an NFS server.
	m) NIS (old yellow pages), hosts.equiv, defaultdomain, etc.
	n) ifaliases for www, etc.
	o) daily, weekly, monthly.
	p) "amd" directory if using this package.
	q) rbootd if needed for remote booting (ethernet MAC address to IP translation).
	r) Any other files and directories in /etc.

   2) crontab -l.		Do you need anything else?
   3) After the first nights security run, change ownerships and permissions on things.
	Best bet is to have permissions as in the security list.




{% endraw %}
```

## Thread

+ Return to [October 1997](/archive/1997/10)

+ Return to "["J. Joseph Max Katz" <jkatz<span>@</span>cpio.org>](/author/j_joseph_max_katz_jkatz_at_cpio_org_)"
+ Return to "[Marshall Midden <m4<span>@</span>nts.umn.edu>](/author/marshall_midden_m4_at_nts_umn_edu_)"

+ 1997-10-15 (Wed, 15 Oct 1997 16:03:42 -0700 (PDT)) - Document on Customizing OpenBSD after install - _Marshall Midden \<m4@nts.umn.edu\>_
  + 1997-10-16 (Wed, 15 Oct 1997 20:02:27 -0700 (PDT)) - [Re: Document on Customizing OpenBSD after install](/archive/1997/10/0b6b77586c7fb289f26164c2593b16f7117253fddab0ccc52ba55ba18c011a07) - _"J. Joseph Max Katz" \<jkatz@cpio.org\>_

