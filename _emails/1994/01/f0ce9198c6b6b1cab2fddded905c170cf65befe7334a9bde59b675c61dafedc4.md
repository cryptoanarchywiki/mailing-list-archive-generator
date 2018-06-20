---
layout: default
---

# 1994-01-20 - Re: faster code for neural network

## Header Data

From: Ron Davis \<rondavis@datawatch.com\><br>
To: cypherpunks@toad.com<br>
Message Hash: f0ce9198c6b6b1cab2fddded905c170cf65befe7334a9bde59b675c61dafedc4<br>
Message ID: \<9401200918.aa03559@gateway.datawatch.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-01-20 14:19:49 UTC<br>
Raw Date: Thu, 20 Jan 94 06:19:49 PST<br>

## Raw message

```
{% raw  %}From: Ron Davis <rondavis@datawatch.com>
Date: Thu, 20 Jan 94 06:19:49 PST
To: cypherpunks@toad.com
Subject: Re: faster code for neural network
Message-ID: <9401200918.aa03559@gateway.datawatch.com>
MIME-Version: 1.0
Content-Type: text/plain


>> Recently I received the code for a neural network. It is written in
>> standard ANSI-C. However, running it on the Mac gives me a lot of coffee
>> breaks ( it takes 10 min on a IIci, 3 hrs on an LC ). I was wondering if
>> anybody out there has experience with this and knows of ways to make the
>> code faster ( replacing ANSI routines with Mac-based routines.
>> 
>> If you are the woman or man with this experience mail me! I really need the
>> help ( it's all for my master's thesis ).
>
>You might want to get  a match coprocessor for the LC.  The ci has one,
>and that's probably your problem.  (I'm not sure if the LC can take one,
>though!)  If my memory still works after the two pints I just had, the LC
>has a 68020 without any FPU.  You might want to upgrade to an LC III and
>find out if it has an FPU.   I believe neural nets use floats, no?  If so
>you will most certainly need and FPU if you want decent speed.
>

The LC does lack a FPU, but you can get one on a card.  I'm not sure if
this would help though, because it would depend if your compilier would
generate FPU code.  I know you can with Think.  You also might need to take
into account which compiler you are using for this kind of program, there
seems to be a vairation in efficency between Mac Compilers.

As for using toolbox calls, using Apple's SANE library might help. I
haven't had much experience with it, but it would probably take advatage of
the FPU.

E-mail me if I can help anymore. (I'll run the program on my Q700 if you
just need a quick speed test.)
___________________________________________________________________________
"I want to know God's thoughts...the rest are details."
                                           -- Albert Einstein
_________________________________________
Ron Davis                                  rondavis@datawatch.com       
Datawatch, Research Triangle Park, NC      (919)549-0711





{% endraw %}
```

## Thread

+ Return to [January 1994](/archive/1994/01)

+ 1994-01-20 (Thu, 20 Jan 94 06:19:49 PST) - Re: faster code for neural network - _Ron Davis \<rondavis@datawatch.com\>_

