---
layout: default
---

# 1997-01-30 - ad.doubleclick.net (fwd)

## Header Data

From: "Mark M." \<markm<span>@</span>voicenet.com\><br>
To: Cypherpunks \<cypherpunks@toad.com\><br>
Message Hash: 76cf3af4ad63496fed5f9110fae0d298c00093aab1eefc2d3edfccb4570d5cfc<br>
Message ID: \<Pine.LNX.3.95.970130172237.1585F-100000@purple.voicenet.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1997-01-30 22:23:34 UTC<br>
Raw Date: Thu, 30 Jan 1997 14:23:34 -0800 (PST)<br>

## Raw message

```
{% raw  %}From: "Mark M." <markm@voicenet.com>
Date: Thu, 30 Jan 1997 14:23:34 -0800 (PST)
To: Cypherpunks <cypherpunks@toad.com>
Subject: ad.doubleclick.net (fwd)
Message-ID: <Pine.LNX.3.95.970130172237.1585F-100000@purple.voicenet.com>
MIME-Version: 1.0
Content-Type: text/plain


Date: Thu, 23 Jan 1997 14:15:38 -0800
From: Caveh Frank Jalali <caveh@Eng.Sun.COM>
Subject: URL filtering, Re: ad.doubleclick.net (RISKS-18.78)

The obvious defense against hostile or undesirable web sites is to not visit
them in the first place.  This process can in fact be automated in
netscape's browser.  This saves bandwidth and your time!

The basic premise is that the browser may optionally execute a function on
every URL before it is accessed to determine whether a direct connection
should be made or a proxy should be used in the process.  This affords the
opportunity to [mis]direct the browser to fetch the document from an invalid
source.  this is a good approximation of not getting the document at all.

We sit behind a fire wall, so all WWW access has to funnel through a
proxy.  If I tell netscape to fetch an external document using a
direct connection, the connection attempt will fail, and the document
will not be accessed.  Netscape will put a broken image icon in its
place.

Here are the nuts and bolts to do it, but some assembly is required:
Under options/network preferences/proxies, select "automatic proxy
config" and tell it which file to use.  Call it something like
"file:///HOMEDIR/.netscape/proxy.pac", replacing HOMEDIR with your
home directory; the actual code is included below.
Next, go to options/general preferences/helpers and create an
application helper of type "application/x-ns-proxy-autoconfig" for
suffix "pac", handled by "navigator".
Install this java-script code to do the actual filtering.  call it
"file:///HOMEDIR/.netscape/proxy.pac", as mentioned before.

================
function FindProxyForURL(url, host) {
	if ( isResolvable(host) && ! shExpMatch(host, "[0-9]*") )
		return "DIRECT" ;
	else if (host == "advertising.quote.com")
		return "DIRECT" ;
	else if (host == "ad.doubleclick.net")
		return "DIRECT" ;
	else if (shExpMatch(url, "*:*/ads/*"))
		return "DIRECT" ;
	else
		return "PROXY webcache:8080; ";
}





{% endraw %}
```

## Thread

+ Return to [January 1997](/archive/1997/01)

+ Return to "["Mark M." <markm<span>@</span>voicenet.com>](/authors/mark_m__markm_at_voicenet_com_)"

+ 1997-01-30 (Thu, 30 Jan 1997 14:23:34 -0800 (PST)) - ad.doubleclick.net (fwd) - _"Mark M." \<markm@voicenet.com\>_

