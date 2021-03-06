---
layout: default
---

# 1993-08-23 - Attacks on remailers

## Header Data

From: hfinney<span>@</span>shell.portal.com<br>
To: cypherpunks@toad.com<br>
Message Hash: 0ae5783f74eebc67fa21daf0c77c11ed629ca8c7fd517c3aa0cdc8c2becc408f<br>
Message ID: \<9308230602.AA25533@jobe.shell.portal.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-08-23 17:36:21 UTC<br>
Raw Date: Mon, 23 Aug 93 10:36:21 PDT<br>

## Raw message

```
{% raw  %}From: hfinney@shell.portal.com
Date: Mon, 23 Aug 93 10:36:21 PDT
To: cypherpunks@toad.com
Subject: Attacks on remailers
Message-ID: <9308230602.AA25533@jobe.shell.portal.com>
MIME-Version: 1.0
Content-Type: text/plain


Chaum, in his first paper on "Mixes" (anonymous remailers) described
protocols which were designed to resist several attacks.  (See the
February, 1981, Communications of the ACM, p. 84.)  These can
be understood by considering a series of attacks of increasing sophis-
tication, with corresponding responses.

Our opponent has as his goal to track a message through a chain of
remailers.

Attack 1: Just intercept the message from the sender, and look at the
commands of the form:
::
Request-Remailing-To: first-remailer
::
Request-Remailing-To: second-remailer
::
Request-Remailing-To: final-destination

The final command shows where the message is finally going to go.

Response: Encrypt the messages.  Use "nesting", so that all that is
visible as each message leaves a remailer is the destination of the
next remailer.

Attack 2: Look at the mail logs on the system running the remailer to
see which message goes out from the remailer account shortly after each
message comes in.

Response: Run the remailer on a machine which does not keep mail logs,
or on a machine to which you can deny the attackers access.

Attack 3: Monitor the messages in real time as they flow into and out of
each remailer machine, again looking for the message which comes out
just after each incoming message.

Response: Batch up many messages which arrive over a period of time,
only sending them out at regular intervals or when a certain number have
accumulated.  Send them out in random order.  Alternatively, delay each
message by a random amount of time before the message goes out.  (This
response will also deal with the previous attack.)

Attack 4: Look at distinguishing features of the messages which are
preserved by the remailers, such as subject line or message size, to
match up incoming and outgoing messages within each batch.

Response: Do not retain any header fields through remailers, not even
subject.  Use an encryption mode in which messages are rounded up to
some standard size so that all messages appear to be the same size.

Attack 5: Record an incoming message to the remailer, and insert a copy
of it into the incoming message stream, so that the batch will have two
identical messages.  Look for two identical outgoing messages.  Remove
one.  This is the match to that incoming message.

Response: Check for duplicate incoming messages in the remailer, and
remove all but one copy of each duplicate.

Attack 6: Insert a duplicate message multiple times in separate batches.
Observe the outgoing batches and look for a pattern of destinations
which are correlated with those batches in which the incoming message
is inserted.

Response: Check for messages which have been duplicated from earlier
batches and remove them.  Include time/date stamps on incoming messages
with a time limit so that they are no good after a certain number of
days; this way the check for duplicates only has to go back that many
days.

Attack 7: Look at all messages coming out of the first remailer, and
follow them into their 2nd remailers; take all messages from those and
follow them on, and so on.  This will eventually lead to a number of
destinations, one of which must have been the destination of the original
message.  Over a period of time, look for correlations between destinations
and sources.

Response: Use large remailer chains of popular remailers.  With enough
mixing at each stage of the chain, the number of possible destinations
will become astronomically large, making correlations statistically
impossible.

Attack 8: Correlate messages being sent from person A with messages being
received a certain time later by person B.  Even without the ability to
track messages through the remailers this can show a communication pattern.

Response: Send dummy messages at regular intervals, which bounce through
the remailer network and then die.  When you have a real message to send,
replace one of the dummies with this.  The sender's traffic pattern is
then constant and no information can be gained from it.

Attack 9: Bribe or coerce one or more remailer operators into revealing
their keys, or into decrypting the desired messages.  Alternatively, run
many remailers, pretending to be dedicated to privacy, while secretly
gathering information on the messages.

Response: Use many remailers in a variety of geographical locations, so
that it is unlikely that all of them can be corrupted in this way.

These are all the attacks I can remember being implicitly considered in
Chaum's paper.  Other people who have ideas for attacks should mention
them so we can think of responses.

Chaum also discusses anonymous return addresses.  We have a simple form
of these enabled in our encrypting remailers.  The idea is to encrypt
a series of remailing requests for the path the message will follow,
with the last request directing the message to the user whose anonymous
address this is.

Some more attacks are possible in this case:

Attack 1A: Look at the message content as it passes through each remailer,
to correlate incoming and outgoing messages.

Response: Encrypt the message at each stage to prevent this matching.  This
raises the problem of how to determine the encryption key in such a way
that the final user can decrypt the message.  Chaum suggested including the
encryption key in the anonymous address (a different key at each stage
of the chain), so that the user can decrypt the message.  Eric Messick
has proposed letting the remailer choose the key, with a protocol for the
user to communicate again with the remailer to get the message decrypted.

Attack 1B: Send two different messages to the same return address with
different contents, and look for duplicate address blocks in the outgoing
batches.

Response: Apply some randomization to the address blocks at each stage so
that messages to the same address don't look identical.  (Chaum did not
give this solution, as he viewed the next attack as being essentially
unanswerable.)

Attack 1C: Send many addresses to the anonymous address, and look for a
destination which receives that many messages in a correlated fashion.

Response: Chaum's response is that the remailer must not accept more than
one message with a given anonymous return address, just as it must not
accept more than one copy of a message in the regular case.  This implies
that anonymous return addresses must be use-once to be truly secure.

This conclusion is uncomfortable, as the requirement that an address be
use-once will severely impair its usability.  But this attack appears
hard to avoid.

There is always the possibility of giving up on anonymous addresses in
the Chaumian sense, and instead using other ideas which have been
suggested here, such as posting to newsgroups, or message broadcast
pools.  All of these ideas have the problem that they expose everyone
in some group to all of the messages intended for every group member,
hence the number of messages will scale as the square of the number of
group members.  This will quickly become unmanageable for large groups,
therefore providing only a limited amount of anonymity.

It's also worth noting that our remailers are vulnerable to almost all
of these attacks; at best we are safe against two or three of them.

Hal Finney
hfinney@shell.portal.com




{% endraw %}
```

## Thread

+ Return to [August 1993](/archive/1993/08)

+ Return to "[cme<span>@</span>ellisun.sw.stratus.com (Carl Ellison)](/authors/cme_at_ellisun_sw_stratus_com_carl_ellison_)"
+ Return to "[hfinney<span>@</span>shell.portal.com](/authors/hfinney_at_shell_portal_com)"

+ 1993-08-23 (Mon, 23 Aug 93 10:36:21 PDT) - Attacks on remailers - _hfinney@shell.portal.com_
  + 1993-08-23 (Mon, 23 Aug 93 14:51:39 PDT) - [Re: Attacks on remailers](/archive/1993/08/067661ade8d388ab8e2a464ebe2ad342ee3e93c744e28c9249e377160eeb13f9) - _cme@ellisun.sw.stratus.com (Carl Ellison)_
  + 1993-08-23 (Mon, 23 Aug 93 15:01:39 PDT) - [Re: Attacks on remailers](/archive/1993/08/1af1806df231a804857c91f2782df8ba0b404652403c82a22f542c539e15ce1d) - _cme@ellisun.sw.stratus.com (Carl Ellison)_

