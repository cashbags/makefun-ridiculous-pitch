# Design — Ridiculous at First Glance, Real by the Second

## The pitch

> Executives pay convents $99 a month per inbox to answer their unanswered emails, because a reply signed by a nun gets answered faster than any assistant's.

155 characters, one sentence.

## How it was chosen

Ten pitches were drafted, each in a lane with no visible entry in the live
field of 720 submissions. Each was judged pairwise against the brief's five
criteria in their published order; the nun-email pitch beat all nine rivals.
The full slate and every pairwise verdict are in CANDIDATES.md.

## Why the lane is empty

The field is flooded with potholes (48), funerals (49), crows (46), goats
(38) and grandmothers (36). Nothing visible touches convents, nuns, email,
or unanswered mail — the dullest corner of office life, which is why the
joke lands: the strangest worker doing the most ordinary job.

## Criterion-by-criterion case

1. Bizarre yet real: nuns on corporate email is absurd on its face, and the
   sentence still names a paying customer, a price, and a return.
2. Never heard before: no visible entry uses this premise, and it is not a
   familiar business with an adjective bolted on.
3. Logic holds: an executive buys replies, not handling. A nun's signature
   is a credible signal that a message deserves an answer, so the $99 buys
   response rate, which one closed deal repays many times over.
4. Turn: laugh at nuns doing email, then nod — of course that email gets
   answered. One sentence, 155 of 200 characters.
5. Concrete: convents, executives, inboxes, $99 a month — a thing sold and
   a buyer, named in the sentence.

## The program

`main.py` holds the pitch as one constant, checks the 1–200 character gate
before writing, and writes exactly those bytes to `/output/entry.txt` with
no trailing newline. No clock, no randomness, no network, stdlib only, so
two runs are byte-identical by construction (verified by running it twice).
