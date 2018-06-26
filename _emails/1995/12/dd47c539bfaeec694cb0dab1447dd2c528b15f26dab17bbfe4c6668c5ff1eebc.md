---
layout: default
---

# 1995-12-02 - Filtering Net Commercials

## Header Data

From: Jeff Simmons \<jsimmons<span>@</span>goblin.punk.net\><br>
To: cypherpunks@toad.com<br>
Message Hash: dd47c539bfaeec694cb0dab1447dd2c528b15f26dab17bbfe4c6668c5ff1eebc<br>
Message ID: \<199512020237.SAA03409@goblin.punk.net\><br>
Reply To: _N/A_<br>
UTC Datetime: 1995-12-02 03:08:23 UTC<br>
Raw Date: Sat, 2 Dec 1995 11:08:23 +0800<br>

## Raw message

```
{% raw  %}From: Jeff Simmons <jsimmons@goblin.punk.net>
Date: Sat, 2 Dec 1995 11:08:23 +0800
To: cypherpunks@toad.com
Subject: Filtering Net Commercials
Message-ID: <199512020237.SAA03409@goblin.punk.net>
MIME-Version: 1.0
Content-Type: text/plain


On December 1, Timothy C. May wrote:

> One patch I'd pay money to have is one which intercept the "commercials"
> Netscape blasts out at us and replace them with something else (maybe
> nothing, maybe a "quote for the day," maybe something from a
> user-selectable file of items).
>
> I understand that Netscape is collecting money for these "commercials," and
> that they control what is sent out. So, any such patch to intercept/remove
> these commercials would have to be done locally. Can this be done?

This is from a post to cypherpunks back in September.  Given the current
situation, maybe a re-posting is in order.  (If not, flames to my address
please, the list has enough to worry about.)  I just checked, it's still
at the ucsb.edu site.

- - - Begin forwarded message - - -

On the subject of HTTP proxies, 

[SEVERAL FWD'S DELETED, ENTERTAINING SUBJECTS RETAINED]

Subject: The agents/advertising arms race heats up
Subject: OH YEAH BABY, FILTER ME HARDER

>From: Axel Boldt <boldt@math.ucsb.edu>
>Newsgroups: comp.infosystems.www.announce
>Subject: SOFTWARE: Filtering ads out of popular web sites
>Organization: Univ of California at Santa Barbara, Dept of Mathematics
>Approved: www-announce@boutell.com
>Message-ID: <44ercn$nhl@holly.aa.net>

Several popular web sites have recently turned to putting advertising
gifs on their pages. NoShit is a tool that filters these out so that
you don't see them - in fact, you don't even download them in the
first place, thus saving time, money and brain capacity.

NoShit is implemented as a set of patches against Cern httpd to turn
it into a "filtering proxy server". This means that the proxy
maintains a list of URL templates together with corresponding filter
scripts. When a document is requested form the proxy that matches one
of the templates, then the page is piped through the corresponding
script before being presented to the client. This works together with
caching, if desired.

The idea is to run your own personalized NoShit proxy server and point
your browser to it. The proxy does the filtering; the browser doesn't
even know about it. This scheme works with every browser.

I have written a ready-to-use library of filter scripts for a couple
of well known, ad-infected sites, including Yahoo, Lycos, Netscape,
HotWired, CNN, Infoseek and NandO Times. You can change these or add
your own very easily.

Locations:
            <URL:http://math-www.uni-paderborn.de/~axel/NoShit/>
                (Germany)
    
            <URL:http://emile.math.ucsb.edu:8000/~boldt/NoShit/>
                (California)

Enjoy,
  Axel

- - - End forwarded message - - -

-- 
Jeff Simmons                           jsimmons@goblin.punk.net




{% endraw %}
```

## Thread

+ Return to [December 1995](/archive/1995/12)

+ Return to "[Jeff Simmons <jsimmons<span>@</span>goblin.punk.net>](/author/jeff_simmons_jsimmons_at_goblin_punk_net_)"

+ 1995-12-02 (Sat, 2 Dec 1995 11:08:23 +0800) - Filtering Net Commercials - _Jeff Simmons \<jsimmons@goblin.punk.net\>_

