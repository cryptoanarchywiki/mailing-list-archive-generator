---
layout: default
---

# 1998-09-10 - RE: Spot The Fed

## Header Data

From: Matthew James Gering \<mgering<span>@</span>ecosystems.net\><br>
To: "Cypherpunks (E-mail)" \<cypherpunks@cyberpass.net\><br>
Message Hash: 57afea3dcd9f7abcbe6cc4c8c63e58ba3f643e393bb8fca3ddc651dbbae56ad7<br>
Message ID: \<33CCFE438B9DD01192E800A024C84A19284637@mossbay.chaffeyhomes.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1998-09-10 05:44:30 UTC<br>
Raw Date: Thu, 10 Sep 1998 13:44:30 +0800<br>

## Raw message

```
{% raw  %}From: Matthew James Gering <mgering@ecosystems.net>
Date: Thu, 10 Sep 1998 13:44:30 +0800
To: "Cypherpunks (E-mail)" <cypherpunks@cyberpass.net>
Subject: RE: Spot The Fed
Message-ID: <33CCFE438B9DD01192E800A024C84A19284637@mossbay.chaffeyhomes.com>
MIME-Version: 1.0
Content-Type: text/plain




Traceroute doesn't use DNS? Whatever.

And it's ICMP, Internet Control Management Protocol.

The original traceroute works by sending User Datagram Protocol (UDP)
datagrams (default 3) to an invalid port address of a remote host,
starting with a Time-To-Live (TTL) of 1 causing the first router in the
path to return an ICMP Time Exceeded Message (TEM), traceroute
increments the TTL by one (up the max hop count, default 30) and
resends, reaching the next router, until an ICMP Destination Unreachable
Message is returned indicating the unreachable port on the destination
host.

The IP addresses of the hops are determined by the return packet
headers, there is no hostname. Reverse DNS lookup is used to give you
the host names, which can be turned on or off in the traceroute options
(it's much faster if you turn it off).

Traceroute was a diagnostic kludge. RFC 1393 describes and ICMP-based
traceroute function, whereby traceroute sends an ICMP trace message (see
the RFC for details) but there is still no hostname on the return
packet, DNS is still used.

Certain ICMP messages are often disabled and/or certain ports blocked or
"shaped" by routers under thresholds to prevent common Denial-of-Service
(DoS) attacks.

	Matt



> -----Original Message-----
> From: Raymond D. Mereniuk [mailto:Raymond@fbn.bc.ca]

> Traceroute doesn't use DNS, it doesn't need to as it already has the 
> IP numbers.  DNS is a system which provides IP numbers when you 
> give it a domain name.  Reverse DNS provides a host name to an IP 
> address but Traceroute doesn't use it.
> 
> Traceroute works at the router level.  Traceroute is like Ping but 
> provides information on every hop including IP number and 
> assigned device name.  With Traceroute if a host name is not 
> received, when requested of course, it is because the equipment 
> was not assigned a host name or it is deliberately suppressed.  I 
> don't use Traceroute a lot but this is the first time I have 
> seen host names suppressed.  
> 
> A lot of routers have ICM suppressed and will not provide a device 
> name.  If an end user site wants to provide better security they will 
> turn off ICM packets.  At that point Traceroute doesn't work at all.




{% endraw %}
```

## Thread

+ Return to [September 1998](/archive/1998/09)

+ Return to "[Matthew James Gering <mgering<span>@</span>ecosystems.net>](/authors/matthew_james_gering_mgering_at_ecosystems_net_)"

+ 1998-09-10 (Thu, 10 Sep 1998 13:44:30 +0800) - RE: Spot The Fed - _Matthew James Gering \<mgering@ecosystems.net\>_

