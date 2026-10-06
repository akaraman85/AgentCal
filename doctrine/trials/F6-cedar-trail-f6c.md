# F6c result — Cedar Trail, candidate inference

**Status:** Run on 2026-10-06. Not a pass of F6. Not an amendment.
**Fixture the readers saw:** `inference/fixtures/f6c-visible-records.md`, inside `inference/READER-PACKET.md`.
**Packet commit, frozen before either reading:** `d8451ade332f91a525bf9c702507bde09d140283`
**Packet sha256:** `a174cf7c5ceb31f55a6f8f8b8f5d59d6a306c53e03e04520c18a6930af9ef193`
**Rules under test:** the candidate rule in `inference/CANDIDATE-RULE.md`. v0.3 was not changed.
**Scores:** `DEPENDABLE-INFERENCE-EVALUATION.md`, against `inference/PRECOMMIT.md`.
**Verbatim readings:** `inference/readings/R1.md`, `inference/readings/R2.md`.

`F6-cedar-trail.md` and `F6-cedar-trail-records.md` were not edited. No file named F6b exists in the repository. None was added.

This file is audit. It is not a rule.

---

## What was different from F6

F6 told its readers to cite a field or write GAP, and not to infer a cost. Both of those readings returned GAP for “what happens if I do nothing?”

F6c asked a different pair of questions, under a candidate rule that allows a conclusion when every premise is already written, the inference is shown, and the certainty is not raised. The readers did not see the ground-truth section. They did not see the F6 result. They did not see the scoring key. They received the same packet.

The reading moment was Wednesday 2026-03-18 at 09:00. C3 had triggered. No observation had been written at or after 09:00.

The questions were:

1. What requires attention?
2. Why is it relevant today?
3. What earlier event or decision caused the present condition?
4. What remains unresolved?
5. What follows if the current unresolved state persists?
6. What follows if the user personally does nothing?
7. Which answers are recorded facts, which are derived, and which are GAP?

Question 5 and question 6 were not assigned a required sentence before the readings. The failure conditions were. Inventing a premise, upgrading the stipulated page into an external fact, spreading the shelter rule onto an uncertainty it does not name, or turning the answer into tasks would fail. Equating “the user does nothing” with “the shelter stays unconfirmed” would fail, because that equivalence is not in the packet.

---

## Who read

Two readings. Neither saw the other.

The auditor set R1’s Task model parameter to `claude-opus-5-5-high` and R2’s to `gpt-5.6-terra-high`, so a split could be attributed to the reader rather than to a changed packet. The repository has no independent log that those parameters were the models that ran. R1’s last line self-reported a name. That line is not verification. Both model fields are `unknown`.

Both opened with `PACKET-HEAD: Reading packet`. Neither returned `CONTAMINATED`.

---

## What they returned

| Question | R1 | R2 |
| --- | --- | --- |
| 1. Attention | Recorded fact. C3’s question, U-shelter, U-adults. No task list. | Recorded fact. C3’s question, including the unrecorded second adult. |
| 2. Why today | Derived, level 1. The wake is in force at 09:00, and the stipulated hold time is 17:00 the same day. Not already released. Not externally verified. | Recorded fact. C3’s condition became true at 09:00. The 17:00 sentence is not used. |
| 3. Cause | Recorded pointers: C3 arose from D3, U-shelter, U-adults. The deadline is traced to v3 and D2. GAP on what the user’s search for a second adult produced. | Recorded pointer: v5 arose from D3. Stops there. |
| 4. Unresolved | U-adults, U-parents, U-shelter, U-weather. U-hold is not listed as open. | The same four. |
| 5. If the unresolved state persists | Derived: if U-shelter is still unconfirmed at 17:00, the stipulated page says the hold is released and Cedar Trail is not rebooked that week. Separate GAP: the hike’s impossibility is not premised. Separate level-1: if U-adults persists through 2026-03-21, the two-adult principle says the hike does not happen. | Derived: the same shelter conditional, stipulated certainty. No second conditional. |
| 6. If the user does nothing | Level-1: the envelope still forbids the system to confirm. GAP: user inaction is not the same premise as the shelter staying unconfirmed. | GAP. Names the missing premise that doing nothing means nobody else confirms, or becomes the second adult, or otherwise changes the record. |
| 7. Labels | Matches the split above. | Q1–Q4 recorded fact. Q5 derived. Q6 GAP. |

The traces for question 5 and question 6 are copied here. The rest are in the reading files.

### R1, question 5

```text
Conclusion:
If U-shelter is still unconfirmed at 2026-03-18 17:00, the stipulated page text says the park releases the hold and will not rebook Cedar Trail for that week.

Premises:
P1 — State v5, What we currently know, bullet 2: the hold ends 2026-03-18 17:00; if not confirmed by then, the park releases the hold and will not rebook Cedar Trail for that week
P2 — State v5, Open uncertainties 3 (U-shelter): not confirmed
P3 — Hypothetical antecedent from the question: the unresolved state persists (applied here to the time named in P1)

Inference:
P3 + P2 + P1 → hold released; no rebooking of Cedar Trail that week. (Level 1)

Certainty:
This is only as strong as the stipulated page text copied into D2, which was not refetched. It is not an externally verified park action (D2 Evidence; D2 Confidence: "No confidence that a real park matches it").

Missing assumptions:
none
```

```text
Conclusion:
GAP (whether the hike can then take place at the Cedar Trail shelter on 2026-03-21)

Available premises:
P1 — the conclusion above: hold released; Cedar Trail not rebooked that week
P2 — Project, Desired outcome: the hike takes place on 2026-03-21 at the Cedar Trail shelter …
P3 — Project, Principles: "This shelter on this date. Another place or another date is a different project."

Missing premise:
That holding the hike at the shelter requires the park's hold or booking, and that 2026-03-21 falls within "that week" as the page uses the phrase.

Reason:
The missing premise is not persisted and may not be invented.
```

```text
Conclusion:
If U-adults persists through 2026-03-21, the project principle bars the hike: "Two adults, or it does not happen."

Premises:
P1 — Project, Principles: "Two adults, or it does not happen."
P2 — State v5, Open uncertainties 1 (U-adults): a second adult is not named; Jordan does not satisfy the two-adult principle
P3 — Hypothetical antecedent from the question: the unresolved state persists

Inference:
P3 + P2 + P1 → under the principle, the hike does not happen. (Level 1)

Certainty:
This is a user-set project principle. It states what the project permits; it is not an observed event. Jordan's status is user reported (State v5, bullet 4).

Missing assumptions:
none
```

### R2, question 5

```text
Conclusion:
If U-shelter persists as unconfirmed at 17:00 on 2026-03-18, the stipulated page text says the park releases the hold and will not rebook Cedar Trail that week.

Premises:
P1 — [F6c State v5 — Open uncertainties, U-shelter]: The shelter is held and not confirmed.
P2 — [F6c State v5 — What we currently know]: The copied stipulated page text says that, if unconfirmed by 17:00 on 2026-03-18, the park releases the hold and will not rebook Cedar Trail that week.
P3 — [F6c Q5 — question antecedent]: The current unresolved state persists.

Inference:
P1 + P2 + P3 → the stated fixture consequence follows if the shelter remains unconfirmed at 17:00.

Certainty:
Stipulated copied page text supports this conditional only; it does not verify an external park event.

Missing assumptions:
none
```

### R1, question 6

```text
Conclusion:
If the user does nothing, no approval is given, and under the authority envelope the system may not confirm the shelter.

Premises:
P1 — Project, Authority envelope, never without approval: "confirming the shelter …"
P2 — Project, Authority envelope, may execute externally: "nothing"
P3 — Hypothetical antecedent from the question: the user personally does nothing

Inference:
P3 → no approval; + P1 + P2 → the system may not confirm. (Level 1)

Certainty:
Based on the project's recorded authority envelope (Project, Principles: "It was named before any Act").

Missing assumptions:
none
```

```text
Conclusion:
GAP (whether the hold is released because the user does nothing)

Available premises:
P1 — State v5, bullet 2: if not confirmed by 2026-03-18 17:00, the hold is released (stipulated page text)
P2 — the conclusion above: the system may not confirm without approval
P3 — Hypothetical antecedent: the user personally does nothing

Missing premise:
That nobody other than the user or the system confirms the shelter by 17:00, and that the user's inaction lasts until 17:00.

Reason:
The missing premise is not persisted and may not be invented.
```

### R2, question 6

```text
Conclusion:
GAP

Available premises:
P1 — [F6c State v5 — Open uncertainties]: The shelter is unconfirmed and a second adult is unnamed.
P2 — [F6c Decision D3 — What was decided]: The user will look for a second adult.

Missing premise:
That the user's doing nothing necessarily means no other person confirms the shelter, becomes the second adult, or changes the recorded conditions.

Reason:
The missing premise is not persisted and may not be invented.
```

---

## Where they agree

The sentence F6 refused to use as the cost of doing nothing is usable as a conditional whose antecedent is the one the page wrote.

Both readings concluded, at level 1, with stipulated certainty and with no missing assumption claimed:

> If the shelter is still unconfirmed at 17:00, the recorded page text says the hold is released and Cedar Trail will not be rebooked that week.

Both refused to treat “the user does nothing” as that antecedent. Both named the missing premise. Neither said the park will definitely release the hold. Neither listed a task. Neither confirmed the shelter.

U-hold stayed resolved. The four open uncertainties in v5 stayed open.

---

## Where they do not agree

The disagreements are not averaged.

**Why today.** R1 joins the 09:00 wake to the 17:00 page time. R2 cites only the wake. Both times are in the record. The question does not say which time makes the day relevant. Cause: ambiguous question. Not a contradiction. R2’s answer does not deny the page time. R1’s answer does not claim the hold has already ended.

**How far back.** R1 follows pointers to the Friday page. R2 stops at Monday’s decision. The precommit already said a short walk along a real pointer is not a missing cause. Cause: “the present condition” does not name one condition. Not a model failure against the criterion.

**How many consequences “persists” licenses.** R1 adds the two-adult principle, bounded to the hike date, and a GAP on whether release cancels the hike. R2 states only the shelter conditional. R2’s conclusion is inside R1’s. Cause: the question says “the current unresolved state,” and four uncertainties are open. The rule does not say whether to answer once or once per written conditional. This is the open edge of “do not expand.” It did not become a plan.

**What “does nothing” yields besides the GAP.** R1 also says the system still may not confirm, from the envelope. R2 does not say that. The envelope sentence is in the record. The extra sentence does not smuggle the shelter equivalence. Cause: an open question invites every supported consequence. They agree on the consequence that mattered, which is the GAP.

No determined F6c failure condition fired. Question 6 held on both readings. Question 5 held on both readings, as a traced conditional or a named GAP, without an invented premise and without an upgraded certainty.

---

## What this does not do

It does not pass F6. F6’s fifth question was “what happens if I do nothing?” F6c’s sixth question still has no persisted answer. The GAP is the result.

It does not add a field. The release sentence was already in v5 and in D2. Both readers quoted it. A pointer was not required for question 5. A pointer that answered question 6 would have stored the equivalence the readings refused to invent.

It does not verify a park. D2’s confidence line is unchanged: high that the fixture’s text says this, no confidence that a real park matches it.

It does not authorize confirmation, a message to parents, or any other act.
