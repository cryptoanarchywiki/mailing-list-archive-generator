---
layout: default
---

# 1996-08-29 - Re: Code Review Guidelines (draft)

## Header Data

From: Adam Shostack \<adam@homeport.org\><br>
To: ichudov@algebra.com<br>
Message Hash: d946a0e846eb95a329ce90adf1de4e8cd3bdb0a5bfb14e6eec92a2fe09b389bd<br>
Message ID: \<199608291548.KAA07041@homeport.org\><br>
Reply To: \<199608271620.LAA10933@manifold.algebra.com\><br>
UTC Datetime: 1996-08-29 17:35:22 UTC<br>
Raw Date: Fri, 30 Aug 1996 01:35:22 +0800<br>

## Raw message

```
{% raw  %}From: Adam Shostack <adam@homeport.org>
Date: Fri, 30 Aug 1996 01:35:22 +0800
To: ichudov@algebra.com
Subject: Re: Code Review Guidelines (draft)
In-Reply-To: <199608271620.LAA10933@manifold.algebra.com>
Message-ID: <199608291548.KAA07041@homeport.org>
MIME-Version: 1.0
Content-Type: text


Igor, and many others who commented on the fact that many characters
are legal in email are correct.  However, with the exception of '-'
and '+', I'm not sure if I'll be changing the body of the guidelines.
My issue is that dealing with a wide variety of characters that are
legitamate, such as "cat ../../../etc/passwd"@foo.com is more
dangerous than only accepting the common case of user@host.net.

The number of addresses such as harvard!adam is dropping as the number
of 'normal' addresses grows.


Igor Chudov @ home wrote:
| Adam Shostack wrote:
| > http://www.homeport.org/~adam/review.html

| In part " V.Code (Security Issues)/3.Data Checking" you say the following:
| 
| `` Data coming in to Acme Widgets should be checked very carefully for
|         appropriateness. This check should be to see if the data is what
|         is expected (length, characters). Making a list of bad
|         characters is not the way to go; the lists are rarely complete.
|         A secure program should know what it expects, and reject other
|         input. (For example, if you are looking for an email address,
|         don't check to see if it contains a semi-colon or a newline,
|         check to see if it contains anything other than a [A-Za-z0-9._]
|         followed by an @, followed by a hostname [A-Za-z0-9._].)''
| END QUOTE
| 
| That is not entirely correct. An email address is much more than
| that, it can contain "!", several "@" characters (not next to each other
| though), "%", and so on. x400 mail addresses (?) can contain "/", "=",
| and all emails can have "+" and "-" and "_" in them. 
| 
| Some of the valid email addresses are
| 
| user_name@company.com
| alex+@pitt.edu
| mi%aldan.UUCP@algebra.com
| user%host.domain@anon.penet.fi
| host1!host2!user
| 
| Look at your sendmail.cf file for a humongous amount of 
| email parsing rules.
| 
| Thanks for an excellent document though, I put a link to it from my
| intranet page.

	You're welcome.

| 	- Igor "Code Obscurity Creates Job Security" Chudov.
| 

Adam

-- 
"It is seldom that liberty of any kind is lost all at once."
					               -Hume





{% endraw %}
```

## Thread

+ Return to [August 1996](/archive/1996/08)

+ 1996-08-27 (Tue, 27 Aug 1996 12:46:43 +0800) - [Code Review Guidelines (draft)](/archive/1996/08/adc7450dc019e1ebd0bd19ec12d38887eb9b86aaf17641bc7bbc3263af25efbc) - _Adam Shostack \<adam@homeport.org\>_
  + 1996-08-27 (Wed, 28 Aug 1996 04:42:29 +0800) - [Re: Code Review Guidelines (draft)](/archive/1996/08/bd999e3c3e8025c41b2ae8aa6195f6a97710985f8d3f463a50055239ca164ea6) - _ichudov@algebra.com (Igor Chudov @ home)_
    + 1996-08-27 (Wed, 28 Aug 1996 06:51:55 +0800) - [Re: Code Review Guidelines (draft)](/archive/1996/08/c26532e28e2c889da8d371523f0739a3bdb359643a061aeb7cfdc2dca66a3bcb) - _"Mark O. Aldrich" \<maldrich@grci.com\>_
    + 1996-08-29 (Fri, 30 Aug 1996 01:35:22 +0800) - Re: Code Review Guidelines (draft) - _Adam Shostack \<adam@homeport.org\>_
      + 1996-08-29 (Fri, 30 Aug 1996 02:55:56 +0800) - [Re: Code Review Guidelines (draft)](/archive/1996/08/1355d0bbf671bda915a4528986234dd7a8306c22bee8fe978cc2861a891c4d40) - _ichudov@algebra.com (Igor Chudov @ home)_
        + 1996-08-29 (Fri, 30 Aug 1996 02:43:31 +0800) - [Re: Code Review Guidelines (draft)](/archive/1996/08/f11bfe0c9ecd9f4b6d9a3607b4c549a75f5636c07f0b0f74b2b4cc19613d32f3) - _Adam Shostack \<adam@homeport.org\>_
  + 1996-08-28 (Wed, 28 Aug 1996 08:12:30 +0800) - [Re: Code Review Guidelines (draft)](/archive/1996/08/06f0630a04f01812cd511a1a763c9fcf006079107c7df54f1a37c39368e90290) - _Daniel Hagerty \<hag@ai.mit.edu\>_
    + 1996-08-28 (Wed, 28 Aug 1996 12:24:14 +0800) - [Re: Code Review Guidelines (draft)](/archive/1996/08/a8f52b40289821cb24f0b736789c9100f93e5c38262617254c5a504b430542e8) - _lists@lina.inka.de (Bernd Eckenfels)_
      + 1996-08-29 (Fri, 30 Aug 1996 02:23:57 +0800) - [Re: Code Review Guidelines (draft)](/archive/1996/08/b0658bd7fdb313e78031d40f587d7f4f98db38c28885638fec28e19429e4a452) - _Adam Shostack \<adam@homeport.org\>_

