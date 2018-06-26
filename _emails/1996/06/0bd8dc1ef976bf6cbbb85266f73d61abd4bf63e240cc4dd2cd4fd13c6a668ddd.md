---
layout: default
---

# 1996-06-16 - Re: Fuseable Links - no guarantees??

## Header Data

From: kooltek<span>@</span>iol.ie (Hack Watch News)<br>
To: cypherpunks@toad.com<br>
Message Hash: 0bd8dc1ef976bf6cbbb85266f73d61abd4bf63e240cc4dd2cd4fd13c6a668ddd<br>
Message ID: \<199606152107.WAA28424@GPO.iol.ie\><br>
Reply To: _N/A_<br>
UTC Datetime: 1996-06-16 01:50:49 UTC<br>
Raw Date: Sun, 16 Jun 1996 09:50:49 +0800<br>

## Raw message

```
{% raw  %}From: kooltek@iol.ie (Hack Watch News)
Date: Sun, 16 Jun 1996 09:50:49 +0800
To: cypherpunks@toad.com
Subject: Re: Fuseable Links - no guarantees??
Message-ID: <199606152107.WAA28424@GPO.iol.ie>
MIME-Version: 1.0
Content-Type: text/plain


>At 11:44 PM 6/14/96 -0400, Warren wrote:
>>I have never paid much attention to the protection of firmware or the
>>technical issues revolving around such schemes...was wondering:
>>
>>I recently saw an add for a UK based group that says they can take a PIC
>>OTP micro and read the prom (for a fee, of course) - How the heck is this
>>done?? I have my suspicion that they (somehow) magically peel off the
>>ceramic coating (without destroying the chewy center), get a circuit mask
>>and 'micro probe' the I/O of the IC...they then download the secret recipe
>>to the afore mentioned 'chewy center'.

The advert was probably for a device/program called PICBUSTER. This is
basically a technique of popping the PIC16C84 microcontroller. The chip is
an EEPROM micro. There are a few ways of popping the chip but the simplest
is to ensure that there is set the supply voltage to the programming voltage
less about 0.7 Volts. This is generally done with the aid of a diode such as
the 1N4148. Then the fuses are reset. For normal programming there should be
at least 5 Volts differential. The smaller differential seems to only allow
the protection to be popped. It is not a fusible link as such.

If you want to read the details they are on
http://www.iol.ie/~kooltek/picbust.html

>>
>>Is this close to accurate?? How is it 'done' ???
>
>
>While I have never come even close to needing to attempt this kind of thing, 
>long ago it occurred to me that if the "no read" bit was stored in a 
>programmable bit, and if the location of that bit was known or could be 
>identified, you could expose that particular bit through a tiny mask hole 
>and cause the part to be readable again.  Locating that bit (assuming 
>there's just one) would be relatively simple:  Take a test part, program it, 
>read-lock it, and then expose it to a VERY slowly sliding mask with UV 
>behind.  Do this for both axes, to find the bit's location on the chip.

Apparently the protection fuse in the EPROM versions of the microcontrollers
are fairly readily identifiable. Most of the OTP microcontrollers are
essentially EPROM types without the quartz glass window. 

The commonest procedure for popping these is to first remove the coating and
then to measure accurately where the protection fuse is. Then, with another
that is to be popped, a small hole is drilled over the fuse area. The
drilling operation stops before reaching the silicon die. Then some strong
acid, either Sulphuric or Nitric is dropped in to disolve the coating. Then
a UV lamp is shone on the fuse to reset it.

The latter techique for popping chips is by far the most dangerous. It
requires proper acid handling procedures and good ventilation. 

Another technique is to fool the microncontroller into switching from
internal to external EPROM and then back. This hack generally works on the
8051, 8751, 8052 and 8752 microcontrollers.

I was coincidentally just finishing a section on popping chips for a book
that I am working on :-)

Regards...jmcc
(John McCormac)
********************************************
John McCormac            * Hack Watch News
jmcc@hackwatch.com       * 22 Viewmount, 
Voice&Fax: +353-51-73640 * Waterford,
BBS: +353-51-50143       * Ireland
********************************************

-----BEGIN PGP PUBLIC KEY BLOCK-----
Version: 2.6

mQCNAzAYPNsAAAEEAPGTHaNyitUTNAwF8BU6mF5PcbLQXdeuHf3xT6UOL+/Od+z+
ZOCAx8Ka9LJBjuQYw8hlqvTV5kceLlrP2HPqmk7YPOw1fQWlpTJof+ZMCxEVd1Qz
TRet2vS/kiRQRYvKOaxoJhqIzUr1g3ovBnIdpKeo4KKULz9XKuxCgZsuLKkVAAUX
tCJKb2huIE1jQ29ybWFjIDxqbWNjQGhhY2t3YXRjaC5jb20+tBJqbWNjQGhhY2t3
YXRjaC5jb20=
=sTfy
-----END PGP PUBLIC KEY BLOCK-----





{% endraw %}
```

## Thread

+ Return to [June 1996](/archive/1996/06)

+ Return to "[kooltek<span>@</span>iol.ie (Hack Watch News)](/author/kooltek_at_iol_ie_hack_watch_news_)"

+ 1996-06-16 (Sun, 16 Jun 1996 09:50:49 +0800) - Re: Fuseable Links - no guarantees?? - _kooltek@iol.ie (Hack Watch News)_

