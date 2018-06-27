---
layout: default
---

# 1993-04-08 - MATH: Zero Knowledge Proofs

## Header Data

From: tcmay<span>@</span>netcom.com (Timothy C. May)<br>
To: Extropians@gnu.ai.mit.edu<br>
Message Hash: aea3af0ffdf57e6d229150bfca3faffdbbb3739774b1d25ee08bcf37c41b2aec<br>
Message ID: \<9304080431.AA26255@netcom.netcom.com\><br>
Reply To: _N/A_<br>
UTC Datetime: 1993-04-08 04:33:22 UTC<br>
Raw Date: Wed, 7 Apr 93 21:33:22 PDT<br>

## Raw message

```
{% raw  %}From: tcmay@netcom.com (Timothy C. May)
Date: Wed, 7 Apr 93 21:33:22 PDT
To: Extropians@gnu.ai.mit.edu
Subject: MATH: Zero Knowledge Proofs
Message-ID: <9304080431.AA26255@netcom.netcom.com>
MIME-Version: 1.0
Content-Type: text/plain


[Since this should also be of interest to the Cypherpunks list, which Ray
is/was subscribed to, I am posting this essay to that list.]

Ray Cromwell writes:

>   Could someone explain zero knowledge proofs and give me an example. I
>have taken number theory and abstract algebra so feel free to use equations.
>
>(I know that zero knowledge proofs are a way of certifying something without
>revealing the information you are certifying, but I want to know how they
>work mathematically)

Zero knowledge interactive proof systems ("ZKIPS") are sometimes called
"minimum disclosure proofs" (with some subtle differences) and are exciting
and mysterious (at first) methods that lie at the heart of modern
cryptology. Here's a simple explanation. Too bad we don't have a
blackboard!

ALICE AND BOB (some people call them Peggy the Prover and Vic the Verifier)

Alice wishes to prove to Bob that she knows some item of knowledge without
actually giving Bob any of that knowledge.

Let us first imagine that Alice claims she knows a "Hamiltonian cycle" on a
particular graph. (For a given set of nodes and arcs linking some of those
nodes, a Hamiltonian cycle is one which passes through each node once and
only once. You might want to draw some graphs on a sheet of paper and try
to find a Hamiltonian cycle for the graphs, to get a feel for the problem.)


The particular graph may be "registered" somewhere with Alice's claim that
she--and only she, for reasons I'll discuss at the end--knows a Hamiltonian
cycle for the graph. In a sense, this is her "proof of identity."

To make this example concrete, Alice is using this piece of knowledge as
her *password* to get into some system. She presents a map of 50  cities
and some set of highways interconnecting them and says "I am who I say I am
if and only if I know a Hamiltonian cycle for this graph."

The conventional (non zero knowledge) way to convey this knowledge is for
Alice to simply *show* the Hamiltonian cycle to Bob. This is how passwords
are currently handled. Bob, and anybody else who is spying on the exchange,
then knows the "secret," which isn't a secret anymore. (Anybody who saw the
exchange, including Sysadmin Bob, could then impersonate her.)

ENTER ZERO KNOWLEDGE

Alice, instead of showing Bob the Hamiltonian cycle, takes the cities and
covers them with something, say, coins. (On a computer, this is all done in
software, using the cryptographic protocol called "bit commitment.")

Alice scrambles the position of the cities (covered by coins) so as not to
allow positional cues. (Most of the 50 cities should have about the same
number, ideally exactly the same number, of links to other cities, to
ensure that some cities are not "marked" by having some unique number of
links. A detail.) Needless to say, she scrambles the cities out of sight of
Bob, so he can't figure out which cities are which. However, once she's
done with the scrambling, she displays the cities in such a way that she
can't *later change*..i.e., she "commits" to the values, using well-known
cryptographic methods for this. (If this sounds mysterious, read up on it.
It's how "mental poker" and other crypto protocols are handled.)

Bob sees 50 cities with links to other cities, but he doesn't have any way
of knowing which of the covered cities are which. Nor, I should add, are
the links labelled in any way--it wouldn't do to have some links
permanently labelled "Route 66" or "Highway 101"!

She says to Bob: "Pick one choice. Either you can see a Hamiltonian cycle
for this set of covered cities and links, or you can see the cities
uncovered." In other words, "Alice cuts, Bob chooses."

Bob tosses a coin or chooses randomly somehow and says: "Show me the cities."

Alice uncovers all the cities and Bob examines the graph. He sees that
Akron is indeed connected to Boise, to Chicago, to Denver, not to Erie, and
so on. In short, he confirms that Alice has shown him the original graph.
No substitution of another graph was made.

Bob, who is suspicious that this person is really who she claims to be, 
says to Alice: "Ok, big deal! So you anticipated I was going to ask you to
show me the cities. Anybody could have gotten Alice's publicly registered
graph and just shown it to me. You had a 50-50 chance of guessing which
choice I'd make."

Alice smugly says to him: "Fine, let's do it again." She scrambles the
cities (which are covered) and displays the graph to Bob...50 covered
cities and various links between them. She tells Bob to choose again.

This time Bob says: "Show me the Hamiltonian cycle."

Without uncovering the cities (which would give the secret away, of
course), Alice connects the cities together in a legal Hamiltonian cycle.

Bob says, "OK, so this time you figured I was going to ask you the opposite
of what I did last time and you just substituted some other graph that you
happened to know the Hamiltonian cycle of. I have no guarantee the graphs
are really the same."

Alice, who knows this is just the beginning, says: "Let's do the next round."

...and so it goes....

After 30 rounds, Alice has either produced a legal Hamiltonian cycle or a
graph that is the same as (isomorphic to...same cities linked to same other
cities) the registered graph in each and every one of the rounds.

There are two possibilities:

1. She's an imposter and has guessed correctly *each time* which choice Bob
will make, thus allowing her to substitute either another graph altogether
(for when Bob wants to see the Hamiltonian cycle) or just the original
graph (for when Bob asks to see the cities uncovered to confirm it's the
real graph). Remember, if Alice guesses wrong even once, she's caught
red-handed.

2. She really is who she claims to be and she really does know a
Hamiltonian cycle of the specified graph.

The odds of #1 being true drop rapidly as the number of rounds are
increased, and after 30 rounds, are only 1 in 2^30, or 1 in a billion. Bob
choose to believe that Alice knows the solution.

Alice has conveyed to Bob proof that she is in possession of some knowledge
without actually revealing any knowledge at all! The proof is
"probabilistic."

This is the essence of a zero knowledge proof. There's more to it than just
this example, of course, but this is the basic idea.


SOME DETAILS

1. Could someone else discover the Hamiltonian cycle of Alice's graph? 

Exhaustive search is the only way to guarantee a solution will be
found--the Hamiltonian cycle problem is a famous "NP-complete"
combinatorial problem. This is intractable for reasonable numbers of nodes.
50 nodes is intractable. 

2. If finding a Hamiltonian cycle is intractable, how the hell did Alice
ever find one?

She didn't *have* to find one! She started with 50 cities, quickly
connected them so that the path went through each city only once and then
wrote this path down as her "secret" solution. Then she went back and added
the other randomly chosen interconnects to make the complete graph. For
this graph, she obviously knows a Hamiltonian cycle, *by construction*.

3. Can Bob reconstruct what the Hamilonian cycle must be by asking for
enough rounds to be done?

Not generally. Read the papers for details on this, which gets deeply into
under what circumstance partial knowledge of the solution gives away the
complete solution.

4. Are there other problems that can be used in this same way?

Yes, there are many forms. I find the Hamiltonian cycle explanation quite
easy to explain to people. (Though usually I can draw pictures, which helps
a lot.)

5. How general is the "zero knowledge interactive proof" approach?

Anything provable in formal logic is provable in zero knowledge, saith the
mathematicians and crypto gurus. Check out the various "Crypto Conference"
Proceedings.

Hope this helps.

-Tim May


--
Timothy C. May         | Crypto Anarchy: encryption, digital money,  
tcmay@netcom.com       | anonymous networks, digital pseudonyms, zero
408-688-5409           | knowledge, reputations, information markets, 
W.A.S.T.E.: Aptos, CA  | black markets, collapse of governments.
Higher Power: 2^756839 | Public Key: MailSafe and PGP available.





{% endraw %}
```

## Thread

+ Return to [April 1993](/archive/1993/04)

+ Return to "[rjc<span>@</span>gnu.ai.mit.edu](/authors/rjc_at_gnu_ai_mit_edu)"
+ Return to "[tcmay<span>@</span>netcom.com (Timothy C. May)](/authors/tcmay_at_netcom_com_timothy_c_may_)"

+ 1993-04-08 (Wed, 7 Apr 93 21:33:22 PDT) - MATH: Zero Knowledge Proofs - _tcmay@netcom.com (Timothy C. May)_
  + 1993-04-08 (Wed, 7 Apr 93 22:59:54 PDT) - [Re: MATH: Zero Knowledge Proofs](/archive/1993/04/7e05f638c6846053c96fe9ae41cf567f2117a2d07cd77b27e96df489ade54062) - _rjc@gnu.ai.mit.edu_

