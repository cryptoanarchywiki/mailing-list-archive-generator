---
layout: default
---

# 1993-06-04 - Re: Software infrastructure

## Header Data

From: J. Michael Diehl \<mdiehl@triton.unm.edu\><br>
To: nobody@shell.portal.com<br>
Message Hash: 805b16be6accccd0a4fdcfff41a800ca3dba14ae2a8dfdcd6a109793c87b974f<br>
Message ID: \<9306040452.AA13658@triton.unm.edu\><br>
Reply To: \<9306040011.AA22327@jobe.shell.portal.com\><br>
UTC Datetime: 1993-06-04 04:53:22 UTC<br>
Raw Date: Thu, 3 Jun 93 21:53:22 PDT<br>

## Raw message

```
{% raw  %}From: J. Michael Diehl <mdiehl@triton.unm.edu>
Date: Thu, 3 Jun 93 21:53:22 PDT
To: nobody@shell.portal.com
Subject: Re: Software infrastructure
In-Reply-To: <9306040011.AA22327@jobe.shell.portal.com>
Message-ID: <9306040452.AA13658@triton.unm.edu>
MIME-Version: 1.0
Content-Type: text/plain


According to nobody@shell.portal.com:
> 
> It would be helpful for me to hear more about how people read and send
> mail on their home computers, in some detail.  If Mike Diehl got
> enough responses to his survey that would be good to hear about, too.

I've gotten a bunch!  I'm storing the messages in a file which will later be 
edited.  Then I'll tally everything up.  Expect results on the list monday.  Of
course this means that if you haven't replied to my poll, you need to do so by
saturday night, mountain time.

Well, now I will describe how I send/receive mail on my system, the killer
8086-8 from Hell! ;^)  I've been hyping my setup on this list for about a month.
But since I've partially implimented a system like what we have been discussing,
I'll give more details.

First, my system configuration:
MACHINE: AT&T 6300 PC 
HARDWARE: 640K, CGA, 1-360K fd, 1-20M hd.
OS: PMS-DOS 3.1 and 4DOS 4.02
COMM PROGRAM: Telix 3.15

As you can see, I am developing for the low-end computer......  ;^)

My email system is composed of (basicly) 2 files, a telix script, and a 4dos
batch file.  

The telix script, at the moment, assumes it is already logged into my unix 
account.  Then it does a 'frm' command and finds out how many NEW messages are
in; it would actually be easier to simply dload all of my messages, but this is
a bit more usefull.  Anyway, it dloads them one at a time onto my pc using 
zmodem.  Once on my machine, the script extracts From: and Subject: information
from the message.  Then it finds a unique filename to give the new message.
This information is then stored in a form usable by the batch file, later.  
After it has done all this, it quits elm, and does some housekeeping.  At this
point, the communications program is finished and the mail is on my pc ready to
read.  Under an automatic implimentation (for, say a pay-as-you-go system) this
can be done without any human intervention.

After the messages have been collected, I, of course, want to read them.  To do
this, I run the mail.bat program.  I am then presented with a menu allowing me 
to Create, Encrypt, Send, Read, Delete mail.  Create, Encrypt, and Delete are 
trivial and don't lend much to this discussion. 

Read presents a menu of messages from the data file created by the telix script.
At the moment, when a user selects a message to read, I use pgp to view it even
if it is not encrypted.  That can be fixed later.

To send a message, you first have to have a file containing the message, duh.
The user is asked for the name of this file, the address of the recipient, and
a subject to use.  This is information is then stored in a form usable by a
third telix script.  Ok, I lied, there are 3 files needed by my system. ;^)

The actuall sending process is simple.  The telix script reads the message 
information and starts elm, supplying the address and subject when asked.  Then
when it gets into vi, it ascii uploads the message directly into vi.  This may
seem kludgy, but it is rather portable since almost every online service lets
you enter a message into an editor.  

Overall, the system works pretty well.  I've still got a few bugs, mostly speed-
related.  But there is room for a lot of improvement.  Here is what I would like
to impliment.

I'd like to have "encryption detection" which would allow my system to use the
appropriate decryption software for message reading.  If a message isn't coded,
it should use list.com.

I'd also like to expand "encryption detection" to recognize several types of 
encryption, pgp, pem, ripem, des, my-bitchin-crypto, etc.  The telix script
could tag the message as it s dloaded.

I'd like to be able to use the system on many online services.  The telix script
could check the phone directory to see which system is it on.  Then, when any
system-specific stuff has to be done, such as starting the mail program on the
host, a special function can be called to do that function on that host.  The
ascii up/down loading is fairly constant, and the local file manipulation 
doesn't depend on the host.

At the moment, I am working on a Reply function.  I know how I'm going to do it,
I just haven't done it yet.  More later.

Well, if you have followed my this far, you either crazy or interested. ;^)  It 
puzzles me why we are contemplating writing our own comm package when so many 
good ones are out there that can be made to serve our purposes.  I'm open to
comments.....  Fire away!

+-----------------------+-----------------------------+---------+
| J. Michael Diehl ;-)  | I thought I was wrong once. | PGP KEY |
| mdiehl@triton.unm.edu |   But, I was mistaken.      |available|
| mike.diehl@fido.org   |                             | Ask Me! |
| (505) 299-2282        +-----------------------------+---------+
|                                                               |
+------"I'm just looking for the opportunity to be -------------+
|            Politically Incorrect!"   <Me>                     |
+-----If codes are outlawed, only criminals wil have codes.-----+
+----Is Big Brother in your phone?  If you don't know, ask me---+



{% endraw %}
```

## Thread

+ Return to [June 1993](/archive/1993/06)

+ 1993-06-04 (Thu, 3 Jun 93 17:17:36 PDT) - [Software infrastructure](/archive/1993/06/329d4e53d135c12df3e179f9a90a146b5c9094bb11fda06139b3ebe308e2f331) - _nobody@shell.portal.com_
  + 1993-06-04 (Thu, 3 Jun 93 21:53:22 PDT) - Re: Software infrastructure - _J. Michael Diehl \<mdiehl@triton.unm.edu\>_
    + 1993-06-04 (Thu, 3 Jun 93 22:25:56 PDT) - [Software infrastructure](/archive/1993/06/69be2689408493cb766c07437c31f6a88738c4fed8a1f631d68d43d1816ed5d9) - _Eric Hughes \<hughes@soda.berkeley.edu\>_
      + 1993-06-05 (Fri, 4 Jun 93 17:36:11 PDT) - [Re: Software infrastructure](/archive/1993/06/94f9dfcb3d269e43adcba8be01d173f708fcaa2b4bd7b4729b11f9a7672a879f) - _J. Michael Diehl \<mdiehl@triton.unm.edu\>_
    + 1993-06-04 (Fri, 4 Jun 93 10:21:12 PDT) - [Re: Software infrastructure](/archive/1993/06/969e5974b04bd0f0bdc738672c0252118ca7063d5004eb262bf828895ff34579) - _Johan Helsingius \<julf@penet.FI\>_
      + 1993-06-04 (Fri, 4 Jun 93 10:50:04 PDT) - [Software infrastructure](/archive/1993/06/368af7957c3531b27d7beda8eae9447b6ac61fcb23df8a1502a0e0abd936c033) - _Eric Hughes \<hughes@soda.berkeley.edu\>_
        + 1993-06-05 (Sat, 5 Jun 93 00:06:42 PDT) - [Re: Software infrastructure](/archive/1993/06/8a8368f02929d5ba37ff2ea1f745f81265cdfcaacae90debcbce4fc0d1927a22) - _Johan Helsingius \<julf@penet.FI\>_

