---
layout: default
---

# 1995-07-14 - Re: Ssh security hole?

## Header Data

From: "Rev. Ben" \<samman<span>@</span>CS.YALE.EDU\><br>
To: Tatu Ylonen \<ylo@cs.hut.fi\><br>
Message Hash: 42b00f21c2c9b0fa0f2601afec5c3e6fe56c3d7b4efe5ec0e60aa849fe1bdac1<br>
Message ID: \<Pine.A32.3.91.950714094431.11806J-100000@JAGUAR.ZOO.CS.YALE.EDU\><br>
Reply To: \<199507132303.CAA18383@shadows.cs.hut.fi\><br>
UTC Datetime: 1995-07-14 13:51:42 UTC<br>
Raw Date: Fri, 14 Jul 95 06:51:42 PDT<br>

## Raw message

```
{% raw  %}From: "Rev. Ben" <samman@CS.YALE.EDU>
Date: Fri, 14 Jul 95 06:51:42 PDT
To: Tatu Ylonen <ylo@cs.hut.fi>
Subject: Re: Ssh security hole?
In-Reply-To: <199507132303.CAA18383@shadows.cs.hut.fi>
Message-ID: <Pine.A32.3.91.950714094431.11806J-100000@JAGUAR.ZOO.CS.YALE.EDU>
MIME-Version: 1.0
Content-Type: text/plain


On Fri, 14 Jul 1995, Tatu Ylonen wrote:

> I think you are right in your analysis.  There is indeed a problem
> with RSA authentication.  Basically what this means is that if you log
> into a corrupt host, that host can at the same time log into another
> host with your account (by fooling you to answer to the request)
> provided that you use the same RSA identity for both hosts.

Bruce Schnier calls this the GrandMaster Problem in the Applied Crypto 
section on Zero Knowledge Authentication.

This can be skewed by requiring synchroneous transmissions within a very 
small synchronized time window.


Ben.
____
Ben Samman..............................................samman@cs.yale.edu
I have learned silence from the talkative, toleration from the intolerant,
and kindness from the unkind; yet, strange, I am ungrateful to those 
teachers.-- K. Gibran. SUPPORT THE PHIL ZIMMERMANN LEGAL DEFENSE FUND!
For information Email: zldf@clark.net       http://www.netresponse.com/zldf  

Original message follows:
_______________________________________________________________
> A workaround is to use a different identity for each host you use.
> The default identity can be specified on a per-host basis in the
> configuration file, or by -i options.
> 
> And, yes, I think the same problem might occur with client host
> authentication.  Though, there you would still have to do IP-spoofing,
> DNS spoofing or similar to get through (breaking RSA based host client
> effectively reduces RhostsRSAAuthentication to conventional .rhosts
> authentication).
> 
> The protocol will need to be changed somewhat because of this.  I'll
> think about it tomorrow and let you say you opinion about it.
> 
> Thanks!
> 
>     Tatu Ylonen <ylo@cs.hut.fi>
> 
> Date: Thu, 13 Jul 1995 13:08:15 -0700
> From: David Mazieres <mazieres@pa.dec.com>
> To: ssh-bugs@cs.hut.fi
> Cc: rtm@eecs.harvard.edu, dm@eecs.harvard.edu, tbl@eecs.harvard.edu
> Subject: Ssh security hole?
> 
> I believe there is a serious problem with the RSA authentication
> scheeme used in ssh, but then again I could be misreading the proposed
> RFC.  Is the following really the case?
> 
> As I understand the protocol, here is what happens during SSH_AUTH_RSA
> authentication.
> 
> Suppose the holder of SKu, is allowed access to account U on machine B
> (which holds SKb).  Both PKu and PKb are widely known.  In addition,
> machine B has a session key, PKs, which changes every hour.  When U on
> machine A wants to log into machine B, here's what I think happens
> based on my reading of the RFC:
> 
> A -> B: A
> 
> B -> A: (PKb, PKs, COOKIE)
> 	[A flags an error if PKb is not the stored value.]
> 
> A -> B: (COOKIE, {{Kab}_PKs}_PKb)
> A -> B: {U}_Kab
> A -> B: {PKu}_Kab
> 	[B aborts if SKu is not allowed access to account U.]
> 
> B -> A: {{N}_PKu}_Kab
> 
> A -> B: {{N}_MD5}_Kab (*)
> 	[B aborts if the MD5 hash is invalid.]
> 
> B -> A: access to acount U with all data encrypted by Kab.
> 
> The problem is, suppose U actually wanted to log into machine C, which
> was maintained by an untrusted person.  The person maintaining C could
> initiate a connection to B the minute U tried to log into C.  When
> given a challenge {{N}_PKu}_Kbc, C could simply give this to A as the
> challenge to respond to, and then forward the response to B.
> 
> To fix the problem, A must at the very least include B in the
> response line marked (*).  I have reason to believe (after having just
> seen a lecture on authentication), that you might even need to include
> more.  A safe bet might be (but then again I am no expert):
> 
> A -> B: {(N, A, B, Kab)}_MD5
> 
> I think similar problems arise for the other authentication methods.
> 
> Other than that, though, I am really impressed by by ssh.  It's easy
> to install and easy to use.  In fact, it is even more convenient to
> use than standard rsh, because the X forwarding happens
> automatically.
> 
> Thanks for such a great package!
> 
> David
> 




{% endraw %}
```

## Thread

+ Return to [July 1995](/archive/1995/07)

+ Return to "["Perry E. Metzger" <perry<span>@</span>imsi.com>](/authors/perry_e_metzger_perry_at_imsi_com_)"
+ Return to "["Rev. Ben" <samman<span>@</span>CS.YALE.EDU>](/authors/rev_ben_samman_at_cs_yale_edu_)"
+ Return to "[Tatu Ylonen <ylo<span>@</span>cs.hut.fi>](/authors/tatu_ylonen_ylo_at_cs_hut_fi_)"

+ _Unknown thread root_
  + 1995-07-13 (Thu, 13 Jul 95 16:03:36 PDT) - [Re: Ssh security hole?](/archive/1995/07/a3ed2ebb0728b2813d3930d24245e2ebb30897a3b468aaa3afc2d06aa8fcf8ca) - _Tatu Ylonen \<ylo@cs.hut.fi\>_
    + 1995-07-14 (Thu, 13 Jul 95 19:04:34 PDT) - [Re: Ssh security hole?](/archive/1995/07/dc5c0bfd5df36b58b1d963f58232bde89ab49a5b17b0e544f7a57c1e049ffac1) - _"Perry E. Metzger" \<perry@imsi.com\>_
    + 1995-07-14 (Fri, 14 Jul 95 06:51:42 PDT) - Re: Ssh security hole? - _"Rev. Ben" \<samman@CS.YALE.EDU\>_

