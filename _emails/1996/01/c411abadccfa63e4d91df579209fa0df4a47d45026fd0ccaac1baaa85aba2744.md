---
layout: default
---

# 1996-01-01 - Re: Australian "calculatorcard"

## Header Data

From: attila \<attila@primenet.com\><br>
To: amp \<Alan.Pugh@internetMCI.COM\><br>
Message Hash: c411abadccfa63e4d91df579209fa0df4a47d45026fd0ccaac1baaa85aba2744<br>
Message ID: \<Pine.BSD.3.91.960101093049.3196B-100000@usr5.primenet.com\><br>
Reply To: \<01HZH81Y0DKI95P3WV@MAIL-CLUSTER.PCY.MCI.NET\><br>
UTC Datetime: 1996-01-01 10:01:40 UTC<br>
Raw Date: Mon, 1 Jan 1996 18:01:40 +0800<br>

## Raw message

```
{% raw  %}From: attila <attila@primenet.com>
Date: Mon, 1 Jan 1996 18:01:40 +0800
To: amp <Alan.Pugh@internetMCI.COM>
Subject: Re: Australian "calculatorcard"
In-Reply-To: <01HZH81Y0DKI95P3WV@MAIL-CLUSTER.PCY.MCI.NET>
Message-ID: <Pine.BSD.3.91.960101093049.3196B-100000@usr5.primenet.com>
MIME-Version: 1.0
Content-Type: text/plain


On Mon, 1 Jan 1996, amp wrote:

> DS> I'd think you could have the server safely accept # N, N-60 sec, and
> DS> N+60 seconds; and adjust the server's idea of your card's clock speed
> DS> from that.
> 
> DS> What new risk would that create?
> 
> i would figure the server would give a minute or so for slippage.
> basically the risk is that it would give someone 3 minutes to do a
> brute force attack rather than one. if you have decent security on
> the server side, i.e., disallow the card for 5 minutes or more after 3
> or so failed attempts, brute attacks would be minimized. however, if
> the actual window for a single code is 3 minutes, that increases your
> chance of hitting it as 3 separate numbers would be valid for a given
> card at any given time.
> 

    START <attila>

	Bank wire systems over the SWIFT private wire are time synched
    much closer than a minute although I have never been given more of
    an answer than that.

	given that you have a tolerable high speed link, and are not
    dealing with an overloaded concentrator at the telco -> carrier
    inferface or an overloaded server, I believe you can solve most
    of the windowing problem by:

	1.  client sends number and time to server
	2.  server send what it thinks as time to client
	3.  client can place a delta on servers time for local time
	4.  enter PIN, etc. and you are working with a much narrower
	    window.

	the security risk does not appear to increase from the 
    exchange times and entering the PIN and letting the normal
    progression go forward once v. just monitoring a series of
    successive verifications trying to effect a pattern in the
    hash.

	Secure-ID seems to be a one-time time-based single use
    pad; to me, using a time exchange initiator has the advantage
    of a smaller window, and fewer problems with client machines
    running on strange times which require sloppier time windows.

    END <attila>





{% endraw %}
```

## Thread

+ Return to [January 1996](/archive/1996/01)

+ 1996-01-01 (Mon, 1 Jan 1996 14:57:23 +0800) - [Re: Australian "calculatorcard"](/archive/1996/01/b5ce56d430c520dbe7acac5423b1862529af57e554a8d8be1c651ac426af88a4) - _amp \<Alan.Pugh@internetMCI.COM\>_
  + 1996-01-01 (Mon, 1 Jan 1996 18:01:40 +0800) - Re: Australian "calculatorcard" - _attila \<attila@primenet.com\>_

