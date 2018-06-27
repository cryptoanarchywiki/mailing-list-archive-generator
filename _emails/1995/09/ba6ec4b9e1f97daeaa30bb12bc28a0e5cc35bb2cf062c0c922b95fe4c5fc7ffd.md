---
layout: default
---

# 1995-09-22 - Re: netscape bug

## Header Data

From: Ray Cromwell \<rjc<span>@</span>clark.net\><br>
To: perry@piermont.com<br>
Message Hash: ba6ec4b9e1f97daeaa30bb12bc28a0e5cc35bb2cf062c0c922b95fe4c5fc7ffd<br>
Message ID: \<199509220511.BAA00235@clark.net\><br>
Reply To: \<199509220443.AAA02254@frankenstein.piermont.com\><br>
UTC Datetime: 1995-09-22 05:12:06 UTC<br>
Raw Date: Thu, 21 Sep 95 22:12:06 PDT<br>

## Raw message

```
{% raw  %}From: Ray Cromwell <rjc@clark.net>
Date: Thu, 21 Sep 95 22:12:06 PDT
To: perry@piermont.com
Subject: Re: netscape bug
In-Reply-To: <199509220443.AAA02254@frankenstein.piermont.com>
Message-ID: <199509220511.BAA00235@clark.net>
MIME-Version: 1.0
Content-Type: text/plain



  Maybe I'm missing something here, but I don't see it. While it is easy
to use the "overwrite buffer and stomp on stack" method to execute code
for programs written as so


void foo(char* inputdata)
{
  char blah[X];
  write_to_buffer_without_knowing_length(inputdata, blah);
}

How would you do it for a program rewritten as

void foo(char* intputdata)
{
  char* blah;
  blah=PMalloc(X);
  write_to_buffer_without_knowing_length(inputdata, blah);
}

Where PMalloc acts like malloc, but from a separate heap. Two
other conditions further hold. All variables in this separate heap
are viewed as "tainted" since they came from user input, and can not
be used as arguments to system(), popen(), fopen(), etc.

Given this, I don't see how it is possible to cause code to be executed.
For one thing, you can't modify the stack. Secondly, since buffers
can't be used as arguments for i/o calls, overwriting nearby buffers like
char *program_path = "auxillary_program" to "/bin/csh" won't do you any
good. (note: a pointer variable should never point to data on the stack
anyway. I'm glad Java eliminated stack data. Pointers to stack data 
are the source of numerous bugs in C. There is a minor performance gain
to having the compiler generate the stack allocation rather than
call malloc(), but it's not worth it. Stack data has the benefit that
it is automatically deallocated upon function return. My answer is
to simply use C++ to achieve this with dynamically allocated resources)


I for one, never use scanf(), gets(), or anything that doesn't know the
size of the destination storage. It's plain stupid. I was tutoring
a student today who had allocated a 20-byte buffer on the stack and
used scanf to ask for a filename. Sheesh.

One thing that should set off alarm bells immediately whenever your
coding is a fixed size buffer justified with the idea "no one could
ever use more than Y resources." Yeah, no one could ever use more
than 11 character file names. 640K ram. 32-bit IP address space. etc, etc.
If not for security, then for simple future flexability.


-Ray



   







{% endraw %}
```

## Thread

+ Return to [September 1995](/archive/1995/09)

+ Return to "[Bill Sommerfeld <sommerfeld<span>@</span>orchard.medford.ma.us>](/authors/bill_sommerfeld_sommerfeld_at_orchard_medford_ma_us_)"
+ Return to "["Perry E. Metzger" <perry<span>@</span>piermont.com>](/authors/perry_e_metzger_perry_at_piermont_com_)"
+ Return to "[Ray Cromwell <rjc<span>@</span>clark.net>](/authors/ray_cromwell_rjc_at_clark_net_)"
+ Return to "[tomw<span>@</span>orac.engr.sgi.com (Tom Weinstein)](/authors/tomw_at_orac_engr_sgi_com_tom_weinstein_)"

+ 1995-09-21 (Thu, 21 Sep 95 15:42:57 PDT) - [netscape bug](/archive/1995/09/00901adc03d841f0d4b1ec0673fc4b565a1092ec5c55586fae9c70f111579add) - _tomw@orac.engr.sgi.com (Tom Weinstein)_
  + 1995-09-22 (Thu, 21 Sep 95 19:19:20 PDT) - [Re: netscape bug](/archive/1995/09/63e0894d5a7d810db321a44494165677bd6b3bacc741bbe6e792ceca8a518b94) - _Bill Sommerfeld \<sommerfeld@orchard.medford.ma.us\>_
  + 1995-09-22 (Thu, 21 Sep 95 21:43:51 PDT) - [Re: netscape bug](/archive/1995/09/e37b3c2972118f59e43bb71523957ef6b41ee5c498f11f2d6355570b260cc1dc) - _"Perry E. Metzger" \<perry@piermont.com\>_
    + 1995-09-22 (Thu, 21 Sep 95 22:12:06 PDT) - Re: netscape bug - _Ray Cromwell \<rjc@clark.net\>_
  + 1995-09-22 (Thu, 21 Sep 95 22:33:41 PDT) - [Re: netscape bug](/archive/1995/09/570ef46268d7d21db91a7f627d84938a371192b146e71962f1007c03380da6e0) - _tomw@orac.engr.sgi.com (Tom Weinstein)_
    + 1995-09-22 (Thu, 21 Sep 95 22:38:08 PDT) - [Re: netscape bug](/archive/1995/09/26a40e540ab3e2c72ffd360d25eb274dcf40e02663df751386fe4d84001b2057) - _"Perry E. Metzger" \<perry@piermont.com\>_

