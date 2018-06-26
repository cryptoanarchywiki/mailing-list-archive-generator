---
layout: default
---

# 1998-01-13 - load balancing web proxy and server networks

## Header Data

From: Adam Back \<aba<span>@</span>dcs.ex.ac.uk\><br>
To: eternity@internexus.net<br>
Message Hash: 5c9d86e70edee2aafc25d75b499eb3b9f00e90db680beeac29ccccbb4ab6da8f<br>
Message ID: \<199801132146.VAA00420@server.eternity.org\><br>
Reply To: _N/A_<br>
UTC Datetime: 1998-01-13 23:31:18 UTC<br>
Raw Date: Wed, 14 Jan 1998 07:31:18 +0800<br>

## Raw message

```
{% raw  %}From: Adam Back <aba@dcs.ex.ac.uk>
Date: Wed, 14 Jan 1998 07:31:18 +0800
To: eternity@internexus.net
Subject: load balancing web proxy and server networks
Message-ID: <199801132146.VAA00420@server.eternity.org>
MIME-Version: 1.0
Content-Type: text/plain




We might also think about adding hot spot avoidance to distributed web
hosting mechanisms.  A distributed web space which distributed itself
to meet demand would be useful.  (An example of hot spots being
perhaps Dan Farmer's web site after he released Satan ... he switched
the web server off to stop his T1 being saturated, until the deluge
subsided).

An automatic load balancing distributed web server would be a kind of
next generation web proxy cacheing and mirroring scheme, dynamically
replicating and cacheing data to meet demand.  Robustness could be
improved also by the redundancy introduced.

Those browsing documents would pay for their web accesses at the
service rate they desired.  A market in web data would then give web
proxies / mirroring agents an economic incentive to automatically
replicate and migrate data.

Web caches already have some protection from various laws.


One other idea for an eternity service host we could leach off was
suggested to me by Ian Brown <I.Brown@cs.ucl.ac.uk>.  His suggestion
was that it would be nice if we could con proxy caches into cacheing
eternity web space for us.

One way to do this for example would be to actually host our own web
pages, but to configure our web server to only serve to a list of web
proxies -- anybody else would get access denied.  The .htaccess
mechanism would be sufficient for this purpose.

Adam





{% endraw %}
```

## Thread

+ Return to [January 1998](/archive/1998/01)

+ Return to "[Adam Back <aba<span>@</span>dcs.ex.ac.uk>](/author/adam_back_aba_at_dcs_ex_ac_uk_)"

+ 1998-01-13 (Wed, 14 Jan 1998 07:31:18 +0800) - load balancing web proxy and server networks - _Adam Back \<aba@dcs.ex.ac.uk\>_

