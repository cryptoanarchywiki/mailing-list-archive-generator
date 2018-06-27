---
layout: default
---

# 1996-02-23 - Re: Patient medical files on Net

## Header Data

From: juggy<span>@</span>cerc.wvu.edu (V. "Juggy" Jagannathan)<br>
To: adam@lighthouse.homeport.org (Adam Shostack)<br>
Message Hash: a4ab7d2f4a7e28ad31fb4ec0bfb3d28da895b0e1c763a775deeda0a4c5df1e3c<br>
Message ID: \<9602221611.AA13184@cerc.wvu.edu\><br>
Reply To: \<199602211521.KAA06043@homeport.org\><br>
UTC Datetime: 1996-02-23 20:51:05 UTC<br>
Raw Date: Sat, 24 Feb 1996 04:51:05 +0800<br>

## Raw message

```
{% raw  %}From: juggy@cerc.wvu.edu (V. "Juggy" Jagannathan)
Date: Sat, 24 Feb 1996 04:51:05 +0800
To: adam@lighthouse.homeport.org (Adam Shostack)
Subject: Re: Patient medical files on Net
In-Reply-To: <199602211521.KAA06043@homeport.org>
Message-ID: <9602221611.AA13184@cerc.wvu.edu>
MIME-Version: 1.0
Content-Type: text/plain




Dear all:

We are pleased with the national attention the ARTEMIS project of the
Concurrent Engineering Research Center(CERC) sponsored by NLM has
attracted. On February 20, there was an article in
the Wall Street Journal calling ARTEMIS an "audacious experiment" by a
rural physician in West Virginia, Dr. Bruce Merkin, M.D. This was
followed by an ABC Evening News story with Peter Jennings (Feb 21,
Wednesday) which declared Dr. Merkin is "the future."

While we  are most happy to receive this attention, we are also
concerned that some people may erroneously draw the conclusion that we
are jeopardizing patient confidentiality by "putting their records on
the Web." We are both  extremely security conscious and thouroughly
familiar with all the available security technologies. We have taken a
number of steps to ensure that our experiment will not be compromized:

1. The patient records are on the INTRAnet which is secured with a
firewall and we continously monitor and evaluate the efficacy of this
protection.

2. Standard UNIX network security mechanisms with all the known security
holes addressed and verified with programs such as "Satan"

3. Multiple levels of access controls, role-based access controls,
user-id based access controls - implemented using Oracle DB mechanisms

4. Audit trails as a separate CORBA-service to track all transactions
and accesses to any patient information

We can add additional layers such as classification of sensitivity of
information, stripping patient identifying information etc as our core
infrastructure is based on CORBA.  We have and continue to experiment
with a number of security technologies. We have in our research
testbed prototypes of systems using Kerberos, PGP, MOSS, and RSA-based
public-key server technologies. We are currently investigating
commercial security technologies and technologies that can securely
bridge World Wide Web and distributed object technologies and CORBA
standards promoted by OMG. Until a satisfactory implementation of
security and a market acceptance of the mechanisms using these
emerging and potent technologies are in place, confidential patient
information will NOT be put in the "Internet".


Sincerely

Ramana Reddy, CERC
V. "Juggy" Jannathan, CERC 
Bruce Merkin, Valley Health Systems Inc.

Co-Principal Investigators

------------------------------------------------------------------
            Ramana Reddy (Also known as Y. V. Reddy) 
            Director
            Concurrent Engineering Research Center
            West Virginia University
            Morgantown, WV 26506
       e-mail: rar@cerc.wvu.edu
-------------------------------------------------------------------








{% endraw %}
```

## Thread

+ Return to [February 1996](/archive/1996/02)

+ Return to "[Adam Shostack <adam<span>@</span>lighthouse.homeport.org>](/authors/adam_shostack_adam_at_lighthouse_homeport_org_)"
+ Return to "[juggy<span>@</span>cerc.wvu.edu (V. "Juggy" Jagannathan)](/authors/juggy_at_cerc_wvu_edu_v_juggy_jagannathan_)"
+ Return to "["Martin Diehl" <mdiehl<span>@</span>dttus.com>](/authors/martin_diehl_mdiehl_at_dttus_com_)"

+ 1996-02-21 (Wed, 21 Feb 1996 12:55:34 +0800) - [Patient medical files on Net](/archive/1996/02/cc7ffa79b284460fcdab1c4452d87e61b9cd7d381d11d7ffd3a257f9ea7f76c6) - _"Martin Diehl" \<mdiehl@dttus.com\>_
  + 1996-02-21 (Thu, 22 Feb 1996 00:38:24 +0800) - [Re: Patient medical files on Net](/archive/1996/02/554444fcbc286d2d9e54d44de3c0dc5a4056ba24d4c6bcad748fdb1a889a2379) - _Adam Shostack \<adam@lighthouse.homeport.org\>_
    + 1996-02-23 (Sat, 24 Feb 1996 04:51:05 +0800) - Re: Patient medical files on Net - _juggy@cerc.wvu.edu (V. "Juggy" Jagannathan)_

