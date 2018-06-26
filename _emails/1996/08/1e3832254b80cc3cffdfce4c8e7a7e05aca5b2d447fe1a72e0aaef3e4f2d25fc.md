---
layout: default
---

# 1996-08-05 - Integrating PGP 3.0 Library with INN

## Header Data

From: ichudov<span>@</span>galaxy.galstar.com (Igor Chudov)<br>
To: ggr@usenix.org<br>
Message Hash: 1e3832254b80cc3cffdfce4c8e7a7e05aca5b2d447fe1a72e0aaef3e4f2d25fc<br>
Message ID: \<199608051829.NAA19030@galaxy.galstar.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-08-05 21:46:10 UTC<br>
Raw Date: Tue, 6 Aug 1996 05:46:10 +0800<br>

## Raw message

```
{% raw  %}From: ichudov@galaxy.galstar.com (Igor Chudov)
Date: Tue, 6 Aug 1996 05:46:10 +0800
To: ggr@usenix.org
Subject: Integrating PGP 3.0 Library with INN
Message-ID: <199608051829.NAA19030@galaxy.galstar.com>
MIME-Version: 1.0
Content-Type: text


Hi,

Has anyone thought of integrating PGP 3.0 library with INN? 

I was thinking along the lines of having PGPMoose support built
right into INN: if an arriving article is posted to a moderated
newsgroup for which a PGP key is available in the INN's keyring,
INN verifies existence and correctness of a PGP signature.

An article that fails this verification will be dropped. 

Same thing can be used for authenticating newgroup and rmgroup
messages, in the spirit of true freedom on usenet -- anyone would
be sent _their own_ newgroups and rmgroups but no one will
be impersonated.

For those not familar with PGP Moose, it is a program that was written
by Greg Rose. It is used for signing approvals on usenet articles. It
takes message body, several important header fields, signs them with
PGP and places the signatures in the headers, in order not to clobber the
text.

If moderators choose short enough keys (512 bits for example), this
verification will not take any significant amount of CPU time.


igor




{% endraw %}
```

## Thread

+ Return to [August 1996](/archive/1996/08)

+ Return to "[Adam Shostack <adam<span>@</span>homeport.org>](/author/adam_shostack_adam_at_homeport_org_)"
+ Return to "[Alan Barrett <apb<span>@</span>iafrica.com>](/author/alan_barrett_apb_at_iafrica_com_)"
+ Return to "[dlv<span>@</span>bwalk.dm.com (Dr.Dimitri Vulis KOTM)](/author/dlv_at_bwalk_dm_com_dr_dimitri_vulis_kotm_)"
+ Return to "[ichudov<span>@</span>galaxy.galstar.com (Igor Chudov)](/author/ichudov_at_galaxy_galstar_com_igor_chudov_)"

+ 1996-08-05 (Tue, 6 Aug 1996 05:46:10 +0800) - Integrating PGP 3.0 Library with INN - _ichudov@galaxy.galstar.com (Igor Chudov)_
  + 1996-08-05 (Tue, 6 Aug 1996 07:22:42 +0800) - [Re: Integrating PGP 3.0 Library with INN](/archive/1996/08/7232c30946d5ce2f03c0a8c087f2e434d602ab7cf2cce6425417d9bfcc2d2265) - _Adam Shostack \<adam@homeport.org\>_
    + 1996-08-06 (Tue, 6 Aug 1996 14:38:46 +0800) - [Re: Integrating PGP 3.0 Library with INN](/archive/1996/08/a75ab56c68657ece2bb0e23ab358cb85f14bbd1e22cc8567f870134d7b78ec08) - _dlv@bwalk.dm.com (Dr.Dimitri Vulis KOTM)_
  + 1996-08-06 (Wed, 7 Aug 1996 06:59:35 +0800) - [Re: Integrating PGP 3.0 Library with INN](/archive/1996/08/28ceb5885f35b065c86593d4bf48625eb53084b67949f8b8abf746a6fc017d15) - _Alan Barrett \<apb@iafrica.com\>_

