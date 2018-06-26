---
layout: default
---

# 1995-08-30 - Re: SSL trouble

## Header Data

From: keelings<span>@</span>wu1.wl.aecl.ca (S. Keeling)<br>
To: cypherpunks@toad.com<br>
Message Hash: 91edca332bbc1a07f49117aaeecdb2eab7b13df08442b3aab113fecb9b51b46d<br>
Message ID: \<9508291415.AA02629@wu1.wl.aecl.ca\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-08-30 15:13:54 UTC<br>
Raw Date: Wed, 30 Aug 95 08:13:54 PDT<br>

## Raw message

```
{% raw  %}From: keelings@wu1.wl.aecl.ca (S. Keeling)
Date: Wed, 30 Aug 95 08:13:54 PDT
To: cypherpunks@toad.com
Subject: Re: SSL trouble
Message-ID: <9508291415.AA02629@wu1.wl.aecl.ca>
MIME-Version: 1.0
Content-Type: text/plain


Incoming from Daniel R. Oelke:
> 
[presumably piete brooks?]:
> > >PS3: I'd like to get the raw date in brloop (a sh script). In perl I'd just
> > >     use "time", and I can't see a way to get "date +" to yield the raw time.
> > >     I could use "date=`perl -e 'print time'`" but that seems OTT, and perl
> > >     may not be on teh users PATH. Any suggestions ?
> >
[anonymous?]
> > "date '+%s'" does it under BSDI, but I'm not sure how portable it is.
>  
> This is what I got from SunOS 4.1.x
>  
>         $ date +%s
>         date: bad format character - s

	On Ultrix, I get:

$_ date '+%s'
s
$_

and on OSF/1:

$_ date '+%s'
%s
$_

	XMan (OSF/1) says:

		"To display the date and time in a specified format, enter:

		date +"%r %d %h %y (%a)"	[note the `+' outside the ""]

which gives me:

		08:58:39 AM 29 Aug 95 (Tue)

FWIW ...


-- 

 "Remember, obsolescence (Win95) isn't an accident;  it's an art form!" 
   keelings@wu1.wl.aecl.ca       s. keeling,   aecl - whiteshell labs



{% endraw %}
```

## Thread

+ Return to [August 1995](/archive/1995/08)

+ Return to "[keelings<span>@</span>wu1.wl.aecl.ca (S. Keeling)](/author/keelings_at_wu1_wl_aecl_ca_s_keeling_)"

+ 1995-08-30 (Wed, 30 Aug 95 08:13:54 PDT) - Re: SSL trouble - _keelings@wu1.wl.aecl.ca (S. Keeling)_

