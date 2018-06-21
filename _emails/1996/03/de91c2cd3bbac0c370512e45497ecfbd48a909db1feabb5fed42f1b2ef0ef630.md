---
layout: default
---

# 1996-03-01 - Re: A brief comparison of email encryption protocols

## Header Data

From: Alex Strasheim \<cp@proust.suba.com\><br>
To: perry@piermont.com<br>
Message Hash: de91c2cd3bbac0c370512e45497ecfbd48a909db1feabb5fed42f1b2ef0ef630<br>
Message ID: \<199603010154.TAA05515@proust.suba.com\><br>
Reply To: \<199602292135.QAA18937@jekyll.piermont.com\><br>
UTC Datetime: 1996-03-01 06:20:26 UTC<br>
Raw Date: Fri, 1 Mar 1996 14:20:26 +0800<br>

## Raw message

```
{% raw  %}From: Alex Strasheim <cp@proust.suba.com>
Date: Fri, 1 Mar 1996 14:20:26 +0800
To: perry@piermont.com
Subject: Re: A brief comparison of email encryption protocols
In-Reply-To: <199602292135.QAA18937@jekyll.piermont.com>
Message-ID: <199603010154.TAA05515@proust.suba.com>
MIME-Version: 1.0
Content-Type: text


> In the end, we are probably going to need something in the way of key
> servers, which may (or may not) imply either a new type of URL or
> something other than a URL to do retrieval off of.

Sorry for the stupid questions, but I want to make sure I'm on the same 
page as the rest of you.  Correct me where I'm wrong --

The idea to have a distributed database (like DNS?) that allows you to
retrieve keys with query strings similar to urls.  So if you wanted to do
a secure telnet to host.foobar.com, you'd submit something like
"telnet://host.foobar.com" to the key server, and it would give you back a
key.  If you wanted to send mail to me, you'd submit something like 
"mailto://alex@suba.com".  Etc.

The key distribution system wouldn't address the problem of trust
directly, but the key you'd get back from the server would contain
information that you could use to verify it.  Suppose I get signed email 
from Perry.  The signature would contain something like 
"mailto://perrry@piermont.com" -- I could use that to get Perry's key to 
verify the signature.  Along with Perry's key I'd probably get a 
signature from some entity that vouches for his key, maybe a piermont.com 
key.  I could follow the chain up until I hit an entity I trust.


If this is correct, I have a question:

What's the advantage of using this url type system instead of "fully
qualified" certificates, ie., attaching all the keys and signatures to the
object?  Doesn't the give and take with the key servers more than wipe out
the advantage of the smaller data object?

Does the win come from solving the revocation problem?


Finally, does anyone know if anything's been happening with Matt's key
management project? 





{% endraw %}
```

## Thread

+ Return to [March 1996](/archive/1996/03)

+ 1996-03-01 (Fri, 1 Mar 1996 09:13:40 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/9ef28ac5ee762a5772e0e710f650fb29b00551c1d1988b6e0648fc118c9d0843) - _cme@cybercash.com (Carl Ellison)_
  + 1996-03-01 (Thu, 29 Feb 96 16:17:26 PST) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/c7d903b3862bd68f0b1a990c45cff6cd39c49f155430532431ec38de3a0ff945) - _Adam Shostack \<adam@homeport.org\>_
  + 1996-03-01 (Fri, 1 Mar 1996 09:41:48 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/f91d744f50de54b345b5b05bab7c18db1b2cccd8d8f2d558335c8a50632ca933) - _Derek Atkins \<warlord@MIT.EDU\>_
    + 1996-03-08 (Fri, 8 Mar 1996 09:58:49 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/e4b684cbde4bdfd6dd0caa1ed01cb5d817ff2748cc171947f4c8f01935800219) - _"Perry E. Metzger" \<perry@piermont.com\>_
      + 1996-03-08 (Fri, 8 Mar 1996 09:57:08 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/f2ede3405090538edaae804c9143c7ab353aee54dd4f5b8061e595d133caf2e7) - _Derek Atkins \<warlord@MIT.EDU\>_
    + 1996-03-09 (Sun, 10 Mar 1996 01:37:06 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/012e1072de8f6b5e7bfff8a66b88f36734e16aeca45bc4e2ae25e02b3cc44a40) - _Tatu Ylonen \<ylo@cs.hut.fi\>_
  + 1996-03-08 (Fri, 8 Mar 1996 10:04:04 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/a38714f5b50a17c3f1fbe9ef373a54ee73355ef49ec6e9abb1873782f87b6f5e) - _"Perry E. Metzger" \<perry@piermont.com\>_
    + 1996-03-01 (Fri, 1 Mar 1996 14:20:26 +0800) - Re: A brief comparison of email encryption protocols - _Alex Strasheim \<cp@proust.suba.com\>_
      + 1996-03-02 (Sat, 2 Mar 1996 08:05:38 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/d355cbddf429279c0caaa4179338e03486e54c46c20f1ecd9a1b5951c1974e01) - _"Perry E. Metzger" \<perry@piermont.com\>_
      + 1996-03-02 (Sat, 2 Mar 1996 14:22:25 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/4a8649cbbca120e0f5bf988499b6423dcf06e242d069119222fd1cea8c57bc9d) - _Adam Shostack \<adam@lighthouse.homeport.org\>_
    + 1996-03-02 (Sat, 2 Mar 1996 14:28:08 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/c6a7fdd7028ddacda15c94c33c89d80654b45d89cb4438243630f28faf82450e) - _Adam Shostack \<adam@lighthouse.homeport.org\>_
      + 1996-03-01 (Fri, 1 Mar 96 08:06:47 PST) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/1d04b514be562ec5cd82002292f3c0f5f4a5c6d1bf13f0ba65fd97ff2a5f51f8) - _Eric Murray \<ericm@lne.com\>_
        + 1996-03-05 (Tue, 5 Mar 1996 19:48:46 +0800) - [Re: A brief comparison of email encryption protocols](/archive/1996/03/d7e7d4337a55aae695d05d2c72c280760335921bf1556ba0e35e1a0e77136d06) - _Adam Shostack \<adam@lighthouse.homeport.org\>_
        + 1996-03-09 (Sun, 10 Mar 1996 01:38:28 +0800) - [Re: key cert. distrib. and management (Was: A brief comparison of email encryption protocols)](/archive/1996/03/79c686439e74363716babad24d6f79aef898314e73b16d81baee714d3d85ba84) - _lmccarth@cs.umass.edu_

