---
layout: default
---

# 1994-02-04 - Remailer FAQ. Details.

## Header Data

From: catalyst-remailer<span>@</span>netcom.com<br>
To: cypherpunks@toad.com<br>
Message Hash: ee9f9afc1aa23cc0c05d1ebcf5d0b9eac84e2b4e4cc737077bccb5a833d6c72a<br>
Message ID: \<199402040732.XAA02211@mail.netcom.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1994-02-04 07:34:53 UTC<br>
Raw Date: Thu, 3 Feb 94 23:34:53 PST<br>

## Raw message

```
{% raw  %}From: catalyst-remailer@netcom.com
Date: Thu, 3 Feb 94 23:34:53 PST
To: cypherpunks@toad.com
Subject: Remailer FAQ. Details.
Message-ID: <199402040732.XAA02211@mail.netcom.com>
MIME-Version: 1.0
Content-Type: text/plain


I hope I can get a bit more attention to this, now that it has become more
sophisticated. Please code warriers, take a break and let the human race
know what the existing remailers are all about. I know exactly why they
don't have enough traffic; knowledge about them is still insider
knowledge. A list of remailer addresses and year-old partial info from a
request made my Tim May was all I could find. Specs needed.

I will send this to Gary Edstrom for the PGP FAQ if I don't have to spend
the rest of my life compiling it. Mail info to qwerty@netcom.com. I'm
interested in hearing from users as well as operators. 

-Nik (Xenon)

Xenon's Full Disclosure Remailer List.

Remailer  Fast?  OpLog SysLog Subj Batch RD NL CPU Phys PGP BitB ?what else?
--------- ------ ----- ------ ---- ----- -- -- --- ---- --- ---- -----------
bsu-cs    +      ?      ?/?    +    ?    ?   ?  ?   ?   23a  ?
catalyst  +      N?    SM/MQ   -    -    ?   -  PA  M   23a  -
choas     +      ?      ?/?    +    ?    ?   ?  ?   ?   -    -
cicada    ++     ?      ?/?    -    -    -   -  ?   ?   -    -
dis.org   -      ?      ?/?    -    ?    ?   ?  ?   ?   23a  ?
extropia  ?      ?      ?/?    +    ?    ?   ?  Pr? ?   23a  ?
jarthur   +/--   St    SM/MQ?  -    ?    ?   ?  Un  ?   23a  -
menudo    --     ?      ?/?    -    t1   ?   ?  ?   ?   -    ?
merde     -/--   ?      ?/?    -    ?    ?   ?  ?   ?   -    ?
penet.fi  --     St     ?/?    -    t?   24  +  Pr  H   -    -
pmantis   ++     ?      ?/?    -    ?    -   -  ?   ?   -    -
qwerty    +      C     SM/MQ   -    -    -   -  PA  M   23a  +
rosebud   ++/-   ?      ?/?    -    -    -   ?  ?   ?   23a  ?
remba       ?    ?      ?/?    ?    ?    ?   ?  ?   ?   23a  ?
shell     ++/+/- St     ?/?    -    ?    ?   ?  ?   ?   23a  -
soda      ++/-   St+?   ?/?    -    ?    ?   ?  ?   ?   -

Subj: Strips Subject header?
NL: Non-linear remailing? 123->231.
RD: Random delay added (max, in hours)?
Batch: Batched remailing? t2 means twice daily. n5 means after 5 messages.
CPU: Pr = private. PA = account on public access machine. Un = university.
Phys: Physical security of the CPU, especially at night. H/M/L.
BitB: BitBucket feature?

Fast?:
++ <5 min
+   5-10 min.
-  ~10-30 min delay
--  Pinging isn't practical due to long delays, but may be more secure.
+/- Sometimes +, sometimes -
Normal internet mail delays are common, and are not equivalent in the two
directions between any two remailers. Mail still gets through.

OpLog:
F: Full copies of all mail is archived. My large volume mailing should
   help put a stop to this.
St: Stats logs of when mail was remailed.
St+: Stats logs of when and where mail was remailed.
St-: Simple counter.
N: Operator keeps no logs.

SysLog:
SM: sendmail logs of when and where mail was exchanged. Root access.
MQ: mailqueue accessible by anyone on the site. Could make logs.

bsu-cs    nowhere@bsu-cs.bsu.edu
catalyst  catalyst@netcom.com
chaos     remailer@chaos.bsu.edu
cicada    hh@cicada.berkeley.edu
dis.org   remailer@dis.org
extropia  remail@extropia.wimsey.com
jarthur   ebrandt@jarthur.claremont.edu
menudo    nobody@Menudo.UH.EDU
merde     remailer@merde.dis.org
penet.fi  anon.penet.fi
pmantis   hh@pmantis.berkeley.edu
qwerty    qwerty@netcom.com
rosebud   elee7h5@rosebud.ee.uh.edu
shell     hfinney@shell.portal.com
soda      hh@soda.berkeley.edu

Discontinued remailers still on some lists out there:

phantom@mead.u.washington.edu
remail@tamaix.tamu.edu
sameer@netcom.com (spelling?)
sameer@berkeley.edu (spelling?)
cdodhner@indirect.com
remailer@entropy.linet.org??
00x@uclink.berkeley.edu?
remail@tamaix.tamu.edu?
remailer@entropy.linet.org?

Background on each remailer:

bsu-cs:
Run by Chael Hall.
Machine: ??
Problems policy: ?? Contact ??
Software: ??
Security: ??
Comments:
History: ??

catalyst:
Run by Scott Collins.
Machine: personal dial-up account on Netcom.
Problems policy: Outgoing address blocking, with proof of ID.
         Contact catalyst@netcom.com.
Software: Customized Hal's ?
Security: Netcom keeps sendmail logs, which root@netcom.com can read.
          Any Netcom user could also compile his own sendmail logs, by
          constantly logging mail as it arrives and leaves.
Comments:
History: ??

chaos:
Run by ??
Machine: ??
Problems policy: ?? Contact ??
Software: ??
Security:
Comments: Finger remailer.help@chaos.bsu.edu for info using any remailer. ??
          gopher chaos.bsu.edu for a collection of info about Cypherpunks.
Comments:
History: ??

cicada:
Run by Eric Hollander.
Machine: ???
Problems policy: ?? Contact ??
Software: ??
Security: Tread lightly. Being "phased out".

dis.org:
Run by ??
Machine: ??
Problems policy: ?? Contact ??
Software: ??
Security: ??
Comments:
History: ??

extropia:
Run by ??
Machine: ??
Problems policy: ??  Contact ??
Software: ??
Security: ??
Comments: Only accepts PGP remailing. ::/Encrypted:PGP header is optional.
          Privately owned, in Canada.
History: ??

jarthur:
Run by Eli Brandt.
Machine: Sequent Symmetry.
Problems policy: Destination blocking is available w/ sufficient ID.
                 Contact ebrandt@jarthur.claremont.edu.
Software: the usual, tweaked for MMDF. Hal's?
Security: jarthur keeps sendmail logs.
Comments:
History: Set up late '92.  PGP added mid-'93.

menudo:
Run by ??
Maching: ??
Problems policy: ?? Contact ??
Software: ??
Security: Stores messages and sends them at midnight??
Comments:
History: ??

merde:
Run by ??
Maching: ??
Problems policy: ?? Contact ??
Software: ??
Security: ??
Comments:
History: ??

penet.fi:
Run by Julf (last name?)
Machine: ?? Operator owned.
Problems policy: Account revokation. Contact ??@anon.penet.fi.
Software: custom.
Security:
Comments: By far the most popular remailer, dwarfing in a day what the
          entire Cypherpunk remailers combined carry in a month. Supports
          easy return addresses as well as non-anonymous mailing to
          someone's anonymous address (na1234... instead of an1234...).
          Your real address is kept on Julf's hard disk, but is fairly safe
          there, especially if you do not abuse your anonymity to harass
          someone. On a bad day your mail and especially Usenet posts may
          be delayed up to two days. Very reliable though. Sends error
          messages back to you for failed mail. Limited to 48K mail.
History: ??

pmantis:
Run by Eric Hollander.
Machine: ??
Problems policy: ?? Contact ??
Software: ??
Security: Tread lightly. Being "phased out".
Comments:
History: ??

qwerty:
Run by Xenon.
Machine: dial-up account on Netcom.
Problems policy: "What problems?". Contact qwerty@netcom.com.
Software: Hal's remailer.
Security: Netcom keeps sendmail logs, which root@netcom.com can read.
          Any Netcom user could also compile his own sendmail logs, by
          constantly logging mil as it arrives and leaves.
Comments: You must use na1234@anon.penet.fi not an1234@anon.penet.fi.
          Finger qwerty@netcom.com for a blurb on the remailer and updates
          on its software.
          Request-Remailing-To: /dev/null is a bit bucket.
          whitehouse.gov gets blocked and fully logged.
History: Up 2/94. Set up by Xenon who needed more remailers to use to send
         PGP info to people with, since anon.penet.fi was overloaded.

rembe:
Run by ?
Machine: ??
Problems policy: ?? Contact ??
Software: ??
Security: ??
Comments: ??
History: ??

rosebud:
Run by Karl Barrus.
Machine: ??
Problems policy: ?? Contact ??
Software: ??
Security: ??
Comments:
History: ??

shell:
Run by Hal Finney.
Machine: ??
Problems policy: ?? Contact ??
Software: Hal's Remailer.
Security: ??
Comments: whitehouse.gov blocked and fully logged.
          hal@alumni.caltech.edu forwards all mail to shell.
History: ??

soda:
Run by Eric Hollander.
Run by: ??
Machine: ??
Problems policy: ?? Blocking of addresses. Mail sent to problem causer.
                 Contact ??
Software: custom. ??
Security: ??
Comments:
History: ??

Remailer Public Keys:
(I've got these...)




{% endraw %}
```

## Thread

+ Return to [February 1994](/archive/1994/02)

+ Return to "[catalyst-remailer<span>@</span>netcom.com](/author/catalystremailer_at_netcom_com)"

+ 1994-02-04 (Thu, 3 Feb 94 23:34:53 PST) - Remailer FAQ. Details. - _catalyst-remailer@netcom.com_

