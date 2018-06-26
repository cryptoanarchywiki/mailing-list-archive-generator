---
layout: default
---

# 1995-09-22 - Re: Another Netscape Bug (and possible security hole)

## Header Data

From: "Perry E. Metzger" \<perry<span>@</span>piermont.com\><br>
To: Ray Cromwell \<rjc@clark.net\><br>
Message Hash: 1a8d729dfda00dca3b63dcf28b5f679a1bfdb44928beafb085afef2a7e84ffd2<br>
Message ID: \<199509221224.IAA03734@frankenstein.piermont.com\><br>
Reply To: \<199509220612.CAA11441@clark.net\><br>
UTC Datetime: 1995-09-22 12:25:00 UTC<br>
Raw Date: Fri, 22 Sep 95 05:25:00 PDT<br>

## Raw message

```
{% raw  %}From: "Perry E. Metzger" <perry@piermont.com>
Date: Fri, 22 Sep 95 05:25:00 PDT
To: Ray Cromwell <rjc@clark.net>
Subject: Re: Another Netscape Bug (and possible security hole)
In-Reply-To: <199509220612.CAA11441@clark.net>
Message-ID: <199509221224.IAA03734@frankenstein.piermont.com>
MIME-Version: 1.0
Content-Type: text/plain



Ray;

This is evidence that, as I said, they have plenty of buffer overflow
bugs. So much for the protestations to the contrary.

My suspicion is that if you used a customized HTTPd that allowed you
to shove arbitrary data into your URL, you could get the victim's copy
of netscape to fandango on the stack and do nicely arbitrary things to
the victim -- like executing "cd ~/; rm -rf ."

A "Hack Netscape" T-Shirt for the first person (Ray, here is your
chance!) to find an exploit using this! Though your demo shouldn't do
anything bad. Does everyone think Ray should get a shirt no matter what?

Perry

Ray Cromwell writes:
> 
> I've found a Netscape bug which I suspect is a buffer overflow and
> may have the potential for serious damage. If it is an overflow bug,
> then it may be possible to infect every computer which accesses a web
> page with Netscape. To see the bug, create an html file containing
> the following:
> 
> <a href="http://foo.bar.foo[rest of giant URL elided]
> 
> On my BSDI2.0 machine running Netscape 1.1N, this causes a segmentation
> fault and subsequent coredump. GDB reports nothing useable (stripped
> executable)
> 
> As you can see, I just chose an extremely long domain name. I guessed
> that the authors of netscape probably thought something like "well,
> a buffer size of 256 characters is good enough to hold any domain"
> 
> It's definately the domain that's causing it, and not the length of
> the URL or the data after the domain name.
>  
> I also tried to overflow some netscape servers using similar techniques
> (and shell metacharacters in all sorts of URLs), to no avail. I suspect
> a similar attack may work against the Netscape Server if it is proxying.
> 
> 
> Does anyone have a disassembly of Netscape, or more specifically, 
> a disassembly of the URL parse and domain lookup routines? I'd be
> happy to collaborate and "Hack Netscape" ;-)
> 
> 
> Happy Hacking,
> -Ray
>  
> 
> 
> 
> 




{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ Return to "[David Lesher <wb8foz<span>@</span>nrk.com>](/author/david_lesher_wb8foz_at_nrk_com_)"
+ Return to "[Duncan Frissell <frissell<span>@</span>panix.com>](/author/duncan_frissell_frissell_at_panix_com_)"
+ Return to "[futplex<span>@</span>pseudonym.com (Futplex)](/author/futplex_at_pseudonym_com_futplex_)"
+ Return to "[heesen<span>@</span>zpr.uni-koeln.de (Rainer Heesen)](/author/heesen_at_zpr_unikoeln_de_rainer_heesen_)"
+ Return to "[jsw<span>@</span>neon.netscape.com (Jeff Weinstein)](/author/jsw_at_neon_netscape_com_jeff_weinstein_)"
+ Return to "[Laurent Demailly <dl<span>@</span>hplyot.obspm.fr>](/author/laurent_demailly_dl_at_hplyot_obspm_fr_)"
+ Return to "["Perry E. Metzger" <perry<span>@</span>piermont.com>](/author/perry_e_metzger_perry_at_piermont_com_)"
+ Return to "[Ray Cromwell <rjc<span>@</span>clark.net>](/author/ray_cromwell_rjc_at_clark_net_)"
+ Return to "[sameer <sameer<span>@</span>c2.org>](/author/sameer_sameer_at_c2_org_)"

+ 1995-09-22 (Thu, 21 Sep 95 23:12:30 PDT) - [Another Netscape Bug (and possible security hole)](/archive/1995/09/fadc044ccc0d051955b7d76793fb468b52e8641b6b922beda4f1970f882561ed) - _Ray Cromwell \<rjc@clark.net\>_
  + 1995-09-22 (Thu, 21 Sep 95 23:52:42 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/066ea4f92849d2c8c902eb038460e8171db235a2751096e6f70b304b30dd9742) - _futplex@pseudonym.com (Futplex)_
    + 1995-09-22 (Fri, 22 Sep 95 00:15:47 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/ea9e2da9e313fbe516bcb67e4f444fca93fd089a22a806c4f4c65463903f78ea) - _Ray Cromwell \<rjc@clark.net\>_
      + 1995-09-22 (Fri, 22 Sep 95 01:14:47 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/4945c2910ebeb4fa59aac38c6102b94c30b2ec32f1a7ad1373de28707bbcdf2e) - _futplex@pseudonym.com (Futplex)_
        + 1995-09-22 (Fri, 22 Sep 95 01:30:13 PDT) - [YET ANOTHER BAD NETSCAPE HOLE!](/archive/1995/09/fe2dd810320cbf1d499e020ccc2c77e38cd9ff7dd8f2353f707a1b234eff9bbd) - _Ray Cromwell \<rjc@clark.net\>_
          + 1995-09-22 (Fri, 22 Sep 95 01:37:09 PDT) - [Re: YET ANOTHER BAD NETSCAPE HOLE!](/archive/1995/09/a4069e3f493bfaf85ba0492c10cf603a2b38c35ee600f1d13b4fb8f0fcbebace) - _Ray Cromwell \<rjc@clark.net\>_
          + 1995-09-22 (Fri, 22 Sep 95 01:50:22 PDT) - [Re: YET ANOTHER BAD NETSCAPE HOLE!](/archive/1995/09/b4d325a8e175c758f57c440a97533629c9233d7f997fb87e8e692a4b107d8cb7) - _futplex@pseudonym.com (Futplex)_
            + 1995-09-22 (Fri, 22 Sep 95 02:46:54 PDT) - [Re: YET ANOTHER BAD NETSCAPE HOLE!](/archive/1995/09/22176ca1ffc4cebcf7917494baba0eb2ac0184be25053059a06749b4dac6278c) - _heesen@zpr.uni-koeln.de (Rainer Heesen)_
          + 1995-09-22 (Fri, 22 Sep 95 02:29:06 PDT) - [Re: YET ANOTHER BAD NETSCAPE HOLE!](/archive/1995/09/b4d4f1e47777bf910d00c3196b86586f3459bec85943d29cbe12ecd54f2b629e) - _jsw@neon.netscape.com (Jeff Weinstein)_
            + 1995-09-22 (Fri, 22 Sep 95 02:36:12 PDT) - [Re: YET ANOTHER BAD NETSCAPE HOLE!](/archive/1995/09/72effb2fb4f3b83d78bc8cbbd18d073be0667ebd67ee416875de7928bff77983) - _Ray Cromwell \<rjc@clark.net\>_
          + 1995-09-22 (Fri, 22 Sep 95 05:48:01 PDT) - [Re: YET ANOTHER BAD NETSCAPE HOLE!](/archive/1995/09/aa4433a6da2b7562a992accd38c713e1e175f3dad4ef7af86e36cb3f0ff2e2d8) - _"Perry E. Metzger" \<perry@piermont.com\>_
        + 1995-09-26 (Tue, 26 Sep 95 05:58:03 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/dbce76ba458ca96516591facb170f7fdb72a68f0261b4f24b43263e56b8ca192) - _David Lesher \<wb8foz@nrk.com\>_
      + 1995-09-22 (Fri, 22 Sep 95 05:36:15 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/872240a3b061d9229333e5b6d8a6c32fa7a8ad076601aa1186171b1424a9b8e7) - _"Perry E. Metzger" \<perry@piermont.com\>_
        + 1995-09-22 (Fri, 22 Sep 95 07:39:36 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/5eddf4fc6b190d0a1334bbf369a4823a45583a4d53b44db390fabf54d4e90410) - _sameer \<sameer@c2.org\>_
        + 1995-09-22 (Fri, 22 Sep 95 10:14:04 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/5855d81b2011edc86e0c20721abb6a93e86d39b6ce517276e3c55fa0fb985595) - _Ray Cromwell \<rjc@clark.net\>_
          + 1995-09-22 (Fri, 22 Sep 95 11:28:44 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/35bdaf8dee5e39c2c403e23a278a529f4396d63a5ccc7c243b5748c6679cf7f0) - _sameer \<sameer@c2.org\>_
        + 1995-09-25 (Mon, 25 Sep 95 13:47:57 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/8cabdd234ee6c9d3303eb16b76297a9278022dfcc8c208849f00d9ef4eaab420) - _Laurent Demailly \<dl@hplyot.obspm.fr\>_
          + 1995-09-26 (Tue, 26 Sep 95 05:02:10 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/26b8551af5412cca9922766dd4d75d1b471729bc7bfdea56c90adf2d74ab071f) - _Duncan Frissell \<frissell@panix.com\>_
  + 1995-09-22 (Fri, 22 Sep 95 00:34:29 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/35cac2a8a72f42eaa0e44adf33d1c39e827eab8b872191099cb391470594ce46) - _jsw@neon.netscape.com (Jeff Weinstein)_
  + 1995-09-22 (Fri, 22 Sep 95 03:15:46 PDT) - [Re: Another Netscape Bug (and possible security hole)](/archive/1995/09/6b45f63609687041fcfd430ec81fb69596b838d8e78ea552b5522b0e0fdcd478) - _Laurent Demailly \<dl@hplyot.obspm.fr\>_
  + 1995-09-22 (Fri, 22 Sep 95 05:25:00 PDT) - Re: Another Netscape Bug (and possible security hole) - _"Perry E. Metzger" \<perry@piermont.com\>_

