---
layout: default
---

# 1996-04-13 - Re: No matter where you go, there they are.

## Header Data

From: jim bell \<jimbell<span>@</span>pacifier.com\><br>
To: "Powers Glenn" \<cypherpunks@toad.com<br>
Message Hash: 88bcfe9bac8eeb9433fe7d4302a7d32ec2acb1e8fcc74b6bab55d2a950a341eb<br>
Message ID: \<m0u7aOu-0008y4C@pacifier.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-04-13 15:13:31 UTC<br>
Raw Date: Sat, 13 Apr 1996 23:13:31 +0800<br>

## Raw message

```
{% raw  %}From: jim bell <jimbell@pacifier.com>
Date: Sat, 13 Apr 1996 23:13:31 +0800
To: "Powers Glenn" <cypherpunks@toad.com
Subject: Re: No matter where you go, there they are.
Message-ID: <m0u7aOu-0008y4C@pacifier.com>
MIME-Version: 1.0
Content-Type: text/plain


At 07:48 PM 4/11/96 GMT+01DST, Powers Glenn wrote:
>- It's called "S/A" (Selective Availability) which is the NWO term for adding 
>- errors that "authorized" users can remove. (Not to be confused with A/S, or 
>- anti-spoofing)   It was originally intended to be turned on in wartime to 
>- deny the enemy accurate fixes, but during the Gulf War military GPS 
>- receivers were so scarce that the soldiers had to use commercial products, 
>- so the S/A actually was turned OFF then!
>- 
>- Since then, pressure has been building to turn off S/A, since its 
usefulness 
>- is nearly zero.  Even so, the amplitude of S/A errors are only a little 
>- larger than natural errors caused by satellite timing errors, atmospheric 
>- propagation variations, etc.  The result is that DGPS is useful, which is 
>- (more or less) a fixed antenna and GPS system which knows where it is, and 
>- subtracts where it "seems" to be by GPS every second, and broadcasts the 
>- resulting error data on some terrestrial system to receivers locally.  The 
>- result is errors down to the 1-meter level and even lower.  That system 
>- compensates for both natural errors and S/A, so the whole purpose of having 
>- S/A is negated.  Eventually S/A will probably be turned off permanently, 
but 
>- even then we'll want to continue to use DGPS systems.
>
>    Close, but not quite:
>S/A is an ADJUSTABLE variable, not on/off. 

Huh?  You sound like you're trying to correct me, but you're not.  I'm 
already aware that the magnitude of S/A is adjustable; nothing I've said 
above contradicts this.

>it can reduce accuracy to 10 meters or 100 meters or whatever. 

For ordinary C/A code (the kind civilians are allowed to use) it can't 
"reduce accuracy to 10 meters."  The minimal error in C/A mode is based on 
atmospheric propagation and other errors.  Adjusting S/A down or off can 
eliminate the ADDED error, not reduce it below C/A's normal minimum RMS value.

>It's a DoD term, not NWO term.

I was being a bit facetious.  Nevertheless, my implication was correct:  The 
term is "selective availability" and it was specifically chosen to sound 
"positive" rather than "negative."  (I can't tell you exactly which issue of 
GPS World magazine mentioned this, but I've read every copy since it was 
started a few years ago.  It was probably in this magazine.  It would have 
been more accurate, I suppose, to call this "Newspeak.")

>    The "this is where you really are" percision location (forgot 
>the designation off hand) is ENCRYPTED (yes, there is crypto 
>revelance here...) in the data stream from the satellites.

It's called "PPS," for "Precise positioning Service."  Check the most recent 
issue of GPS World for an article on making that even more accurate.  
Nevertheless, even PPS is only accurate to about +/- 2 meters; DGPS is 
easily accurate to 1 meter, and I've seen ads that talk about 0.15 meter 
accuracy with differential GPS in C/A mode.

> The difference S/A makes is on the order of magnitude, therefore not 
>"useless." 

That depends on what you compare it to.  If you compare it to 
non-differential, C/A code signal, it turns +/- 25 meter (approx, of course) 
errors to upwards of +/- 100 meter errors, although as I understand it S/A 
is normally toned down to about +/- 50 meters.  BTW, I don't doubt that DoD 
has the technical ability to increase S/A even beyond +/- 100 meters, but 
that would be a pointless exercise.  It would also strongly piss off the 
average civilian GPS user, and since by far the largest number of GPS users 
are now civilian (and this number is growing rapidly) the DoD knows which 
side of its bread is buttered.

And using DGPS, the effect of S/A is essentially nil, since both it and most 
"natural" (unintentional) errors are cancelled out.  

So, what part of "useless" do you not understand?  

Please note that I didn't say it had no effect, merely that it was 
"useless."  As in, no militarily significant effect.    If you still 
disagree, please formulate a plausible (and, ideally, a PROBABLE) scenario 
under which the presence of S/A achieves a military benefit based on a 
rational view of whichever "enemy" you choose.  Since DGPS receivers are 
available for well under $1000, you're going to have to hypothesize a 
poverty-stricken enemy indeed. 

>It should be pointed out that different regions of the 
>earth can have different degrees of accuracy based on the S/A system.
>    I doubt S/A will ever be turned off, but this is my opinion.

Just a couple of days ago, I saw a note HERE reporting that Clinton had 
backed down (his normal behavior, interestingly!) and had decided to turn 
off S/A.  I haven't seen any confirmation of this claim, but then I haven't 
looked either.  If that report was correct, your opinion is already wrong.

I am fully aware that it could later be turned back on, if there was a 
genuine reason to do so.  This would be in line with the original intent 
behind S/A, to turn it on only when there was some real reasons to do so.  
Why they did not adopt this planned mode years ago, I don't know.  

>I know Jim's opinion. Discussion of this point is pointless.

In other words, "Don't confuse me with the facts."

>    DGPS transmission are made from a multiple single points, which 
>(to the best of my knowledge) are not networked.
>    glenn

That's only partially true.  There is nothing to prevent the world-wide 
distribution of a data stream which represents the complete differential 
correction data for GPS, broadcast from multiple locations  by FM 
subcarrier, idle cell-phone site, HF, pager channels, or 
other.   In fact, it has been argued that it should be transmitted, in the 
band of the GPS signals(so that a separate differential antenna is not 
required), from satellites, with the receivers built into GPS units, so that 
it would be available to everyone no matter where he is.  The attraction of 
this system, from a government/military standpoint, is that it would tend to 
foster dependance on this correction system by the average GPS user, and 
would tend to deter development of DGPS stations independent of the 
government.  That means that the government would actually be able to keep 
the "S/A advantage":  When it wants accuracies to be degraded, they will be. 
 Its current policy, however, practically guarantees that DGPS stations will 
be broadcasting in every major population center within just a few years.

Isn't it a good thing that government is so (CDA alert!) fucking stupid?

Jim "He only talks about one subject" Bell
jimbell@pacifier.com






{% endraw %}
```

## Thread

+ Return to [April 1996](/archive/1996/04)

+ Return to "[jim bell <jimbell<span>@</span>pacifier.com>](/authors/jim_bell_jimbell_at_pacifier_com_)"

+ 1996-04-13 (Sat, 13 Apr 1996 23:13:31 +0800) - Re: No matter where you go, there they are. - _jim bell \<jimbell@pacifier.com\>_

