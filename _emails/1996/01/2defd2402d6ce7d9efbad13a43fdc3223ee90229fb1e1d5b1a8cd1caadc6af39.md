---
layout: default
---

# 1996-01-27 - [NOISY] Printing Microsoft's CryptoAPI .ps

## Header Data

From: Rich Graves \<llurch@networking.stanford.edu\><br>
To: Louis Freeh \<cypherpunks@toad.com\><br>
Message Hash: 2defd2402d6ce7d9efbad13a43fdc3223ee90229fb1e1d5b1a8cd1caadc6af39<br>
Message ID: \<Pine.ULT.3.91.960126125847.19154L-100000@Networking.Stanford.EDU\><br>
Reply To: \<2.2.32.19960126184329.002dbed0@isdn.net\><br>
UTC Datetime: 1996-01-27 00:41:43 UTC<br>
Raw Date: Sat, 27 Jan 1996 08:41:43 +0800<br>

## Raw message

```
{% raw  %}From: Rich Graves <llurch@networking.stanford.edu>
Date: Sat, 27 Jan 1996 08:41:43 +0800
To: Louis Freeh <cypherpunks@toad.com>
Subject: [NOISY] Printing Microsoft's CryptoAPI .ps
In-Reply-To: <2.2.32.19960126184329.002dbed0@isdn.net>
Message-ID: <Pine.ULT.3.91.960126125847.19154L-100000@Networking.Stanford.EDU>
MIME-Version: 1.0
Content-Type: text/plain


The problems futplex et al were having are the result of a known
incompatibility between Windows [95] and many print spoolers. You can fix
it like so: 

Date: Thu, 14 Dec 1995 17:41:02 -0800 (PST)
From: Rich Graves <llurch@networking.Stanford.EDU>
To: win95netbugs@lists.Stanford.EDU
Subject: Fix for PostScript printer "PJL" Error (printing PostScript code rather than image)

Shamelessly lifted from the discussion forum on NetWork 
World's Web site, http://nwfusion.com/

-rich
 owner-win95netbugs@lists.stanford.edu
 ftp://ftp.stanford.edu/pub/mailing-lists/win95netbugs/
 gopher://quixote.stanford.edu/1m/win95netbugs
 http://www-leland.stanford.edu/~llurch/win95netbugs/faq.html

>From ohara on Wed Nov 1 12:14:40 1995

I have a problem when printing to postscript printers spooled from unix 
hosts. I am running Win95 and FTP Software's
Interdrive 95 (for the lpr client).

The problem is that the printer spits out pages of postscript code 
rather than the page the code represents. This
happens only when I print over the network. If I plug directly into the 
printer, everything works fine.

It seems that Microsoft improved the pscript.drv to also send "PJL" code 
to printers. Thus, the actual postscript is
surrounded by PJL. Redirect a postscript printer to a file and take a look.

Unfortunately, this causes the spooler on the unix host to identify the 
print job as a plain ascii file, rather than a
postscript file. Other than manually editting every print job and 
copying it to the printer port, is there a way to
eliminate the PJL and get my networked printers working again?

-Bob


>From ohara on Thu Nov 2 11:23:54 1995

I have figured out how to excise the offending PJL commands from the 
postcript output stream. Every printer that is
added to Win 95 puts a unique file into the windows system directory. In 
my case the file is ibm4039p.spd. This file
seems to be a control file for pscript.drv as well as the customization 
of the properties dialog for the printer. 

In my case there are several lines that include the word "PJL": 

*Protocols: PJL TBCP

and

*JCLBegin: "<1B>%-12345X@PJL JOB<0A>"
*JCLToPSInterpreter: "@PJL ENTER LANGUAGE = Postscript <0A>"
*JCLEnd: "<1B>%-12345X@PJL EOJ <0A><1B>%-12345X"

When I deleted these lines from the .spd file and restarted Win95, the 
problem was gone. -Bob
===========================================================================
Sent through the win9netbugs list. To unsubscribe, send an email message to
majordomo@lists.stanford.edu with "unsubscribe win95netbugs" in the *body*.
Note spelling. URL for FAQ and further info is in each message's X-headers.




{% endraw %}
```

## Thread

+ Return to [January 1996](/archive/1996/01)

+ 1996-01-26 (Sat, 27 Jan 1996 05:20:53 +0800) - [Re: Microsoft's CryptoAPI - thoughts?](/archive/1996/01/4740409e9f94d9e8e221f5b046ee3fd5cdbbdf09ab84dab8b6c9f8682a47cd19) - _Lou Zirko \<lzirko@isdn.net\>_
  + 1996-01-27 (Sat, 27 Jan 1996 08:41:43 +0800) - [NOISY] Printing Microsoft's CryptoAPI .ps - _Rich Graves \<llurch@networking.stanford.edu\>_

