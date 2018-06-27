---
layout: default
---

# 1997-09-28 - Re: Remailer Attack

## Header Data

From: "Robert A. Costner" \<pooh<span>@</span>efga.org\><br>
To: cypherpunks@cyberpass.net<br>
Message Hash: 92fcdcb0700149d0a5d45a4efffe4edceaa0e7d0830dbfa7f34cef5d410456fb<br>
Message ID: \<3.0.3.32.19970927215256.032fa804@mail.atl.bellsouth.net\><br>
Reply To: \<5b2ff18d32f6e69b9daafc8470b65133@anon.efga.org\><br>
UTC Datetime: 1997-09-28 02:10:40 UTC<br>
Raw Date: Sun, 28 Sep 1997 10:10:40 +0800<br>

## Raw message

```
{% raw  %}From: "Robert A. Costner" <pooh@efga.org>
Date: Sun, 28 Sep 1997 10:10:40 +0800
To: cypherpunks@cyberpass.net
Subject: Re: Remailer Attack
In-Reply-To: <5b2ff18d32f6e69b9daafc8470b65133@anon.efga.org>
Message-ID: <3.0.3.32.19970927215256.032fa804@mail.atl.bellsouth.net>
MIME-Version: 1.0
Content-Type: text/plain



At 08:03 PM 9/27/97 -0400, Anonymous (Monty Cantsin) wrote:
>One more question: When redneck is down, do other remailers discard
>their mail if they cannot connect to it?
...
>According to Raph, redneck has an uptime of 99.83%.  By my
>understanding, this means for every 1000 messages handled, redneck
>loses 17.

For a variety of reasons, mail is never "lost" to Redneck because of
downtime.  Only if the Redneck remailer is unreachable for a period of say
five days (it really depends on the sender's ISP) will a message get lost.
Then it will be attempted to be returned to the sender, by the Sender's
ISP's machine, not redneck.  In a case where Redneck is too busy too often,
or for some other reason, the sender's ISP's equipment will resend the
message to Redneck dozens or hundreds of times until the message goes
through.  The downtime statistic is more an indication of when email has to
be sent more than once to get to Redneck.  Apparently this is 17 out of
1,000 messages on the average.  To be honest, I don't really know how the
stats program works, I'm just assuming this is what is being checked.

>For some reason, we are accustomed to the
>idea that remailers should lose messages.

I'm not sure what you mean here.  A properly run remailer doesn't lose
messages.  There may be criteria that triggers a remailer to discard a
message, but a message never gets lost.

Did I open up a can of worms by saying that?  Policies will vary from
remailer to remailer.  Some items that might get discarded (or might not)
would be things such as 

  Mail from cyberpromo.com
  A 300MB email bomb
  6,000 identical messages to the same address
  A message to a particular newsgroup
  Mail to someone who has requested to be blocked

Remailers support free speech, but some mild restraints are placed to aid
in preventing abuse.  If you are talking about setting up a remailer as a
business then as a business there would be policies of what did or did not
go through.

You asked earlier which remailers charge for services.  I'm really not
sure.  Check www.cyberpass.com.  I believe they offer anonymous accounts
and accept Ecash.  


  -- Robert Costner                  Phone: (770) 512-8746
     Electronic Frontiers Georgia    mailto:pooh@efga.org  
     http://www.efga.org/            run PGP 5.0 for my public key





{% endraw %}
```

## Thread

+ Return to [September 1997](/archive/1997/09)

+ Return to "[Anonymous <anon<span>@</span>anon.efga.org>](/authors/anonymous_anon_at_anon_efga_org_)"
+ Return to "["Robert A. Costner" <pooh<span>@</span>efga.org>](/authors/robert_a_costner_pooh_at_efga_org_)"

+ 1997-09-28 (Sun, 28 Sep 1997 08:03:30 +0800) - [Re: Remailer Attack](/archive/1997/09/cfb5c29d3aac12715d8930c86567b5f1bcded57a740e3e0eafb89772333923a1) - _Anonymous \<anon@anon.efga.org\>_
  + 1997-09-28 (Sun, 28 Sep 1997 10:10:40 +0800) - Re: Remailer Attack - _"Robert A. Costner" \<pooh@efga.org\>_

