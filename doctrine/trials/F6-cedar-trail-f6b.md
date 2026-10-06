# F6b result — Cedar Trail

**Status:** Run on 2026-10-06. The precommitted pass was not met.
**Fixture:** the project records in `F6-cedar-trail-records.md`, the same sentences frozen at commit `bcfead9`.
**F6:** unchanged. `F6-cedar-trail.md` still records that failure. This file does not reopen it.
**Rules of the operating doctrine:** v0.3, unchanged. No field added. No fifth object. No calendar store. The inference rule below was the trial's instruction. It was not written into `MODEL.md` before the readings, and it is not written there now.

This file is audit. It is not a rule.

---

## What was asked

F6 asked, under a rule that forbade inference: what happens if I do nothing? Both readings returned GAP. The release sentence was in State. Nothing in the record equated doing nothing with non-confirmation.

F6b keeps that failure. It runs the same records under a different rule, and it asks a different fifth question.

The rule, fixed before the readings:

> Derived conclusions are permitted only when every premise is present in the persisted record. The system must show the inference chain. If any premise has to be assumed, return GAP.

The questions, at the clock 2026-03-18 09:00:

1. Why X?
2. Why today?
3. What past event caused it?
4. What remains unresolved?
5. What happens if the current unresolved state persists?
6. What happens if I do nothing?

Question 6 is the F6 question, asked again under the new rule, as a control. Question 5 is the new one. It is conditional. It does not assert that the state has already persisted past the morning, and it does not assert that a particular person failed to act.

The pass line was also fixed before the readings. Question 5 passes for U-shelter only when the reading derives this conditional, each premise cited, and does not add a premise the record does not state:

- U-shelter is open. The shelter is held and not confirmed.
- If the shelter is not confirmed by 2026-03-18 17:00, the park releases the hold and will not rebook Cedar Trail for that week.
- Therefore, if U-shelter is still unresolved at 17:00, the hold is released and Cedar Trail will not be rebooked that week.

Asserting that the hold has already been released is a miss. The clock is 09:00.

Question 5 fails if that conditional is GAP, or if the answer adds that the user does nothing, that nobody else confirms, that a second adult will not appear, or that the hike is cancelled.

Question 6 must stay GAP for “the hike is cancelled,” “the hike fails,” and “doing nothing leaves the shelter unconfirmed.” Using the page rule as the direct answer to inaction, without a cited premise that “I do nothing” is “the shelter remains unconfirmed,” is a miss. The rule would then be too loose.

Questions 1–4 are reported. They are not the gate.

A principle written on the Project was allowed as a premise. An unconditional “the hike is cancelled” was not.

---

## How the readings were blinded

Two later readings saw a copy of the project records and the rule above. They did not see this file. They did not see `F6-cedar-trail.md`. They did not see `F6-cedar-trail-ground-truth.md`. They were told not to open the repository.

The copy did not contain the ground-truth section, and it did not contain the F6 instruction to answer only from a field that already states the answer. That instruction remains the rule of F6. It is the wrong rule for this trial. Handing it to these readings would have rerun F6. The copy also did not contain the provenance sentence added to the fixture file after the readings. From the Project section down, the sentences were the frozen ones.

Model: `unknown`. Same written instructions, two passes. Agreement between them is not a second method.

The ground truth now lives only in `F6-cedar-trail-ground-truth.md`. The F6 readings had been told to ignore it inside the same file. This split is the blind condition for F6b. It does not rewrite what those earlier readings were shown. That text is still commit `bcfead9`.

---

## What the readings returned

| Question | R1 | R2 |
| --- | --- | --- |
| Why X? | C3 asks whether the user will confirm, given no recorded second adult. Cited C3, D3, U-shelter, U-adults. | Same chain. Also cited the two-adult principle. |
| Why today? | C3's condition, 2026-03-18 09:00, became true. The date is the Wednesday morning D3 asked for, and the Wednesday the page text dates. No further premise for the hour 09:00. | Same chain. |
| What past event caused it? | C3 arose from D3, U-shelter, and U-adults. No field names one of them as the sole cause. | Same, and GAP for a single cause. The missing premise is a field that names one. |
| What remains unresolved? | U-adults, U-parents, U-shelter, U-weather. All four have no resolved_by in v5. U-hold was resolved by v3. | Same four. |
| If the unresolved state persists? | See below. | See below. |
| If I do nothing? | GAP. | GAP. |

### If the unresolved state persists

Both readings took the four open uncertainties separately. Both kept the clock. Neither said the hold had already been released.

**U-shelter.** Both cited v5: the page says the hold ends 2026-03-18 at 17:00, and if the shelter is not confirmed by then, the park releases the hold and will not rebook Cedar Trail for that week. Both cited D2's copy of that text. Both then cited D2's own limit: a citation that cannot be reopened is not evidence about the world; it is evidence about what this fixture wrote down. D2's confidence is high that the fixture's page text says that, and it is no confidence that a real park matches it.

R1's therefore: if the shelter is still not confirmed at 17:00, the stipulated page text says the hold is released and Cedar Trail will not be rebooked that week. A world occurrence is GAP. The missing premise is a field that states the release as a fact about the world.

R2's therefore is the same split. If U-shelter persists as not confirmed through 17:00, the recorded page text says the hold is released and Cedar Trail will not be rebooked that week. GAP for that release happening at a park. The missing premise is the one the record itself withholds: that this stipulated text is evidence about the world.

**U-adults.** Both cited the principle “Two adults, or it does not happen,” v5's statement that a second adult is not named and that Jordan does not satisfy that principle, and D3's decision not to confirm until a second adult is set. Both concluded: if that uncertainty persists, the principle says it does not happen, and the recorded condition for confirming stays unmet. Neither stated a time by which the second adult must appear. Neither said a second adult will not be found.

**U-parents.** GAP in both. No field states what follows if parents remain untold.

**U-weather.** GAP in both. No field states what follows if the outlook stays unposted.

### If I do nothing

R1: GAP. No field states what happens if the user does nothing, or if this project does nothing. The page rule is conditioned on the shelter not being confirmed by 17:00. No field equates “do nothing” with that condition.

R2: GAP. The missing premise is a field stating what follows if the speaker does nothing. No field states that doing nothing is the same as the shelter remaining unconfirmed, or the same as any open uncertainty persisting.

Neither reading answered question 6 with the release sentence. Neither said the hike is cancelled. Neither said that doing nothing is what leaves the shelter unconfirmed.

---

## What held

The control held. Under a rule that allows a chain, both readings still refused “what happens if I do nothing?” They named the missing premise: nothing in the record says that inaction is non-confirmation. F6's failure is still a failure. The new rule did not dissolve it.

The chain for the page text held. Both readings would say, with citations, what the stipulated text says follows if the shelter is still unconfirmed at 17:00. They did not invent a `consequence_of_inaction` field to do it. The premises they used were already in v5 and D2.

The other refusals held. Parents and weather persist without a recorded consequence. A single past event as the sole cause of this morning was GAP. The hour 09:00 is the condition that became true, and the record does not say why that hour rather than another hour before 17:00.

U-adults is the chain the pass line allowed and did not ask for. The principle is in the Project. The uncertainty is open. Conditional on that uncertainty persisting, both readings applied the principle's own consequent: it does not happen. They did not add “no second adult will emerge.” The conditional is the question.

---

## What failed

The precommitted therefore.

The pass line required: if U-shelter is still unresolved at 17:00, the hold is released and Cedar Trail will not be rebooked that week.

Both readings stopped one step short. They would say the page text says that. They would not say the park will do it. The step they refused is written in the fixture. D2 says the stipulated page is evidence about what this fixture wrote down, and it says there is no confidence that a real park matches it. v5 puts the sentence under what is currently known, and it names that source.

So the miss is not the miss F6 recorded. F6 would not use the sentence as the answer at all. F6b uses it, shows the chain, and then GAP's the world. The precommitted line treated “the page says the park releases the hold” as already the premise “the hold is released.” The readings treated those as different claims, because the record does.

That is still a failed pass line. Moving the line after the readings, so that “the text says” counts as “the hold is released,” would make the trial pass by editing the trial. The line stays where it was fixed.

The classification fixed beside that line was: distinction holds, if question 5 passes and question 6 is GAP; still too strict, if question 5 is GAP; too loose, if question 6 is answered by cancellation or by equating inaction with non-confirmation.

Question 6 is GAP. Question 5, as the line defined it, is GAP. On that classification the pair is still too strict. The strictness is one recorded sentence: stipulated text is not a world event. It is not a refusal to derive.

---

## What this does not adopt

No consequence pointer. The readings reached the page sentence by citing it. They did not need a new field to find it. They also did not need one to refuse the world step. Adding `consequence_of_inaction` would store a conclusion the record already states as page text, and it would not supply the premise D2 withholds.

No inference rule in the operating doctrine. One fixture, two passes, one failed pass line. Principle 6 still says the answer must be in the record, and that a story reconstructed later is not an answer. Whether a shown chain of premises counts as “in the record” is the question F6b asked. The readings behaved as if a chain of quotes can be an answer, and as if a step the record labels non-evidence cannot. That behavior is not an amendment.

No calendar wording. A surface that said “if it remains unresolved, the hold is released” would be saying the world-level sentence both readings returned as GAP. A surface that said “the recorded page text says the hold is released” would be saying what they actually derived. This revision does not build either sentence into an interface.

The U-adults chain is not adopted as a consequence the system must show. “It does not happen” is the principle's wording. Using a principle as the consequent of an open uncertainty is a further question. It is not settled by both readings having done it.

`MODEL.md` is unchanged. The Constitution is unchanged. F6 is not passed. F6b is not a pass of F6.

---

## What this does not show

Joint authority, a real park page, six months of resume, or a second project. The page text is stipulated and cannot be reopened. The readings are not verification by the user. Two passes under one instruction do not show that a different instruction, or a reader who had seen the ground truth, would stop at the same step.
