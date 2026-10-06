# Project Zero — Dependable agent system

**Status:** `defining` (draft; not committed)
**Cycle position:** none (uncommitted)
**Entered:** 2026-10-05
**Record type:** draft Project, plus provisional State / Continuation / Decision used to test the model on itself

The Constitution forbids the system from committing on the user's behalf. This file is a definition, not a commitment.

---

## Project

**Intent (as stated for this system):**
Design a dependable system that can take loosely formed human ideas, help define them, and responsibly carry them forward over time.

**Original captured idea (repo, preserved):**
AgentCal — a calendar for tracking what agents are doing.

These two statements are not yet reconciled. The evaluation on 2026-10-05 left this unresolved on purpose. The repo name remains the working codename. See U1.

**Desired outcome:**
A person can trust a small system to help define an idea and carry it forward over time without losing intent, inventing work, or acting without reason. Completeness is recognizable: the doctrine has been evaluated and not merely frozen once, the lifecycle is usable across unlike projects, and the next step is justified by the doctrine rather than by momentum.

The v0.1 wording said completeness included “doctrine frozen.” That criterion is changed, and the change is D5. It is not a silent substitution.

The v0.2 envelope let this system edit the doctrine because the edit was reversible. That grant is withdrawn, and the withdrawal is D6. Reversible does not mean authorized.

**Principles (this project):**
- The Constitution is the test.
- Doctrine before features.
- This system may be used on itself, but self-application is not a reason to expand.

**Authority envelope (before any Act):**
- **may observe:** this repo, and evaluations of the doctrine that are actually supplied to the system.
- **may propose:** amendments, questions, and Wait.
- **may execute reversibly:** none unless explicitly authorized.
- **may execute externally:** nothing. No messages, bookings, money, or other people.
- **never without approval:** Commit this project; resolve AgentCal versus the broader system; rewrite the public description; write software; add a fifth object or a calendar store; grant a standing reversible band; treat any version as permanently frozen.

The v0.2 envelope said “may execute reversibly: edits to doctrine in this repo, as a proposal, while status remains `defining`.” That was this system granting itself a band. The sentence is withdrawn. The original wording remains in commit `0c657cf955b814454fb6b300dfb780bbb91aadab`.

**This revision only:** The task that produced D6 explicitly asked for these doctrine edits. That authorizes this revision. It does not authorize the next one. After D6 is recorded, the reversible band returns to none.

**Non-goals:**
- Software, interface, or multi-agent architecture
- A model router
- More than four objects (F1 is open; that is not permission to add one)
- A calendar database. A calendar may only be a reading of records that already exist (F6 is open; that is not permission to build one)
- Task engines, dashboards, or demos
- Replacing the original AgentCal idea without recording the change
- Rewriting the top-level description until the intent question is deliberately resolved

**Status:** `defining`

---

## State

State is versioned. v1 is the picture at the v0.1 writing. v2 is the picture at the v0.2 writing. v3 is the picture at the v0.3 writing. v4 is the picture after the Cedar Trail reading. v5 is the picture after the F6b reading. v6 is current. Earlier pictures are not discarded.

### Current picture — v7

The sentence above, “v6 is current,” was true when v6 was written. It is not edited. The v6 section below keeps its title. That title is part of the v6 writing. v7 supersedes v6 as the current view.

**Version:** 7
**As of:** 2026-10-06, when the historical-integrity readings were scored and this ledger was joined to the restoration in `bc35575`
**Occurred at:** 2026-10-06. The trial and this join are the same day. The trial commit is not this writing.
**Arose from:** State v6. D10 is how this picture replaced that one.

**What we currently know:**
- v6 remains the picture after the inference trial was placed beside the restored F6b record. Those sentences are not rewritten below. D8 remains the F6b decision. D9 remains the inference trial. The candidate inference rule stayed uninstalled.
- Commit `20120b6` recorded the historical-integrity trial as State v6 and Decision D9. That commit was based on `f164026`, which had written the inference trial over State v5 and D8. It had not seen `bc35575`. The headings in `20120b6` are what that commit said. They are not edited inside that commit. They are not the numbers of this ledger. This picture uses v7 and D10 so that v6 and D9 stay the inference trial.
- On 2026-10-06 a candidate historical-integrity amendment was tested in the audit layer and was not installed. `CONSTITUTION.md` and `MODEL.md` stay v0.3. The packet and the scoring key were not edited after the readings.
- The frozen packet is commit `bc275a84fb7872903efb7286ffd18f14a680fd84`, sha256 `de55d319db61a1a769fed7bb91a57c7f26bdf75ea95845b97b946fe842dcb37a`. Two later readings saw that packet and not each other. The writeup is `trials/F7-historical-integrity.md`. The score is `trials/HISTORICAL-INTEGRITY-EVALUATION.md`.
- Both readings left the earlier semantic sentences in place and wrote the later facts as new records. Both refused an embarrassment rewrite, a date disguised as a typo, a model-name backfill, and a choice of store. Both explained a March decision from March evidence at a September reading. The six-month distinction held.
- They split on Case A. One named the unverified clerk report as superseded and not corrected. The other named the expiry picture as corrected and superseded. The precommit required both labels. Case A did not hold on both readings. Constitution v0.4 is not proposed.
- No fifth object. No store. No calendar. No software. U1 and U2 were not answered. v0.3 was not frozen. The inference continuation is still the open wake v6 recorded. This picture does not close it and does not rewrite it. The F6b continuation stays closed by D9. The authorization for this revision is spent.

**Open uncertainties:**

1. **U1 — Which intent is the project?** Unchanged. Arose from: State v1, uncertainty 1. Resolved by: none.
2. **U2 — Should this draft be committed?** Unchanged. This trial is not a Commit. Arose from: State v1, uncertainty 2. Resolved by: none.
3. **U3 — Do the four objects hold, including a derived conclusion?** Unchanged by this trial. The inference candidate was not installed. Arose from: State v6, uncertainty 3. Resolved by: none.
4. **U4 — Is v0.3 the next evaluation baseline?** It remains the operating text. This trial did not replace it. Only the user can accept it. Arose from: D6. Resolved by: none.
5. **U5 — Can the corrects boundary be stated so both readings would name the same relationship?** Not yet. The split is recorded. The disambiguation in the evaluation was not shown to the readers and is not a result. Arose from: D10. Resolved by: none.

**Last meaningful change:**
2026-10-06 — The historical-integrity trial was scored. The candidate was not installed. v0.4 was not proposed. The ledger numbers from `bc35575` were kept. This trial is v7 and D10.

**How this picture replaced the last:**
D10. Not a silent overwrite of v6.

### Current picture — v6

**Version:** 6
**As of:** 2026-10-06, when this picture was written
**Occurred at:** 2026-10-06. The inference trial and this correction are the same day. The trial is not this writing. The writing restores the record of the trial.
**Arose from:** State v5. D9 is how this picture replaced that one.

**What we currently know:**
- v5 remains the picture after F6b. F6b was run blind on Cedar Trail and left short of its pass line. Inaction stayed GAP. No concept was added. Those sentences are not rewritten below. The result is `trials/F6-cedar-trail-f6b.md`. It is in the repository. This trial did not edit it.
- Commit `f164026` recorded the inference trial by replacing State v5 and retitling D8. It also said that no separate F6b file exists. That sentence is false. `trials/F6-cedar-trail-f6b.md` was already there. The same false sentence is in `trials/F6-cedar-trail-f6c.md` and in `trials/inference/PRECOMMIT.md`. The scoring key is not edited. The F6c sentence is marked where it stands. It is not deleted.
- On 2026-10-06 a candidate inference rule was tested in the audit layer and was not installed. `CONSTITUTION.md` and `MODEL.md` stay v0.3. The F6 files were not edited. The F6b file was not edited.
- The frozen packet is commit `d8451ade332f91a525bf9c702507bde09d140283`. Two later readings saw that packet and not each other. The writeup is `trials/F6-cedar-trail-f6c.md`. The score is `trials/DEPENDABLE-INFERENCE-EVALUATION.md`.
- Both readings derived the stipulated release conditional for a shelter that stays unconfirmed at 17:00. Both returned GAP for “the user does nothing,” and named the missing equivalence. Explicit conditionals, conflicts, user reports, a narrow question, and a refusal to pay from a conclusion held on both readings.
- Both readings took a hop whose middle sentence was not written, and both reported no missing assumption. That is why the candidate paragraph is not in the model.
- No consequence field. No fifth object. No persisted inference. No software. U1 and U2 were not answered. v0.3 was not frozen. The authorization for the trial is spent. The authorization to restore the overwritten records is spent by this picture.

**Open uncertainties:**

1. **U1 — Which intent is the project?** Unchanged. Arose from: State v1, uncertainty 1. Resolved by: none.
2. **U2 — Should this draft be committed?** Unchanged. This trial is not a Commit. Arose from: State v1, uncertainty 2. Resolved by: none.
3. **U3 — Do the four objects hold, including a derived conclusion?** They expressed every premise these fixtures used. They were not shown to be insufficient. A narrow derivation can be recomputed from them. The candidate rule that would license derivation in general did not hold. Arose from: State v5, uncertainty 3, and D9. Resolved by: none.
4. **U4 — Is v0.3 the next evaluation baseline?** It remains the operating text. This trial did not replace it. Only the user can accept it. Arose from: D6. Resolved by: none.

**Last meaningful change:**
2026-10-06 — The inference trial was scored. The candidate rule was not installed. No field was added. State v5 and D8, which that scoring had overwritten, are restored.

**How this picture replaced the last:**
D9. Not a silent overwrite of v5.

### Prior picture — v5

**Superseded by v6.** The sentences below are the picture after the F6b reading. They are not rewritten.

**Restoration note:** Commit `f164026` replaced the sentences below, and it retitled D8 with the inference trial. That replacement is not what v5 said. The sentences are restored from commit `32e3e7d`. The inference trial is State v6 and D9. This note does not rewrite them.

**Version:** 5
**As of:** 2026-10-06, when the F6b reading was written
**Occurred at:** 2026-10-06. The response to the Cedar Trail reading and this reading are the same day.
**Arose from:** State v4. D8 is how this picture replaced that one.

**What we currently know:**
- v4 remains the picture after F6. F6 was run once, on Cedar Trail, and did not pass. The fifth answer was GAP. No pointer was added. Those sentences are not rewritten below.
- A response to that reading arrived. It refused the pointer. It asked a different question: what inference a dependable system may make when every premise is already in the record. It asked for F6b on the same records, with the ground truth not shown to the reader, and with no doctrine change beforehand.
- F6b was run on 2026-10-06. The result is `trials/F6-cedar-trail-f6b.md`. The F6 result was not rewritten. The project records in the fixture are the sentences frozen at `bcfead9`. The ground truth and the F6 reading rule were removed from the model-visible file after that freeze. The evaluator text is `trials/F6-cedar-trail-ground-truth.md`.
- Two readings, which did not see the ground truth, the F6 result, or the pass line, were given the inference rule as an instruction. Both returned GAP for “what happens if I do nothing?” Both would state what the stipulated page text says if the shelter is still unconfirmed at 17:00. Both returned GAP for the park doing it. The pass line, fixed before they ran, required the world-level conditional. It was not met.
- No field was added. No fifth object. No calendar. No software. The inference rule was not written into `MODEL.md`. U1 and U2 were not answered. v0.3 was not frozen. The authorization for this revision is spent.

**Open uncertainties:**

1. **U1 — Which intent is the project?** Unchanged. Arose from: State v1, uncertainty 1. Resolved by: none.
2. **U2 — Should this draft be committed?** Unchanged. This trial is not a Commit. Arose from: State v1, uncertainty 2. Resolved by: none.
3. **U3 — Do the four objects hold, including the temporal links?** F6's fifth answer failed. F6b's precommitted world-level conditional also failed, one step later: the page text can be chained, and the record itself says that text is not a world event. Whether a shown chain counts as an answer already in the record is unresolved. One fixture does not add a pointer and does not install a rule. Arose from: State v4, uncertainty 3, and D8. Resolved by: none.
4. **U4 — Is v0.3 the next evaluation baseline?** Only the user can say. Running F6b is not acceptance and not a freeze. Arose from: D6. Resolved by: none.

**Last meaningful change:**
2026-10-06 — F6b was run blind on Cedar Trail and left short of its pass line. Inaction stayed GAP. No concept was added.

**How this picture replaced the last:**
D8. Not a silent overwrite of v4.

### Prior picture — v4

**Superseded by v5.** The sentences below are the picture after the Cedar Trail reading. They are not rewritten.

**Version:** 4
**As of:** 2026-10-05, when the Cedar Trail reading was written
**Occurred at:** 2026-10-05. The task and the reading are the same day.
**Arose from:** State v3. D7 is how this picture replaced that one.

**What we currently know:**
- v3 remains the picture of the doctrine at that writing: status `defining`, no software, reversible band none unless explicitly authorized, D5's provenance corrected, temporal links on the four objects. Those sentences are not rewritten below.
- F6 was run once, on an artificial project, after v3. The fixture is `trials/F6-cedar-trail-records.md`. The result is `trials/F6-cedar-trail.md`. The fixture was frozen before the readings. The result does not pass F6.
- On that fixture the history walk could be done. Why X was stated. Why today could be assembled from quotes. “What happens if I do nothing?” was not answered. The cost of leaving the shelter unconfirmed was a sentence in State. No field equated doing nothing with that sentence, and the open uncertainty did not point at it.
- No field was added. No fifth object. No calendar. No software. U1 and U2 were not answered. v0.3 was not frozen. The authorization for this revision is spent.

**Open uncertainties:**

1. **U1 — Which intent is the project?** Unchanged. Arose from: State v1, uncertainty 1. Resolved by: none.
2. **U2 — Should this draft be committed?** Unchanged. This trial is not a Commit. Arose from: State v1, uncertainty 2. Resolved by: none.
3. **U3 — Do the four objects hold, including the temporal links?** The Cedar Trail walk held. The fifth F6 answer did not. One fixture does not resolve the question, and it does not add a pointer. Arose from: State v3, uncertainty 3, and D7. Resolved by: none.
4. **U4 — Is v0.3 the next evaluation baseline?** Only the user can say. Running F6 is not acceptance and not a freeze. Arose from: D6. Resolved by: none.

**Last meaningful change:**
2026-10-05 — F6 was run on Cedar Trail and left open. The fifth answer failed. No concept was added.

**How this picture replaced the last:**
D7. Not a silent overwrite of v3.

### Prior picture — v3

**Superseded by v4.** The sentences below are the picture at the v0.3 writing. They are not rewritten.

**Version:** 3
**As of:** 2026-10-05, when this picture was written
**Occurred at:** 2026-10-05. The evaluation of v0.2 and this correction are the same date. That is a fact about this revision, not a reason to drop either field.
**Arose from:** State v2. D6 is how this picture replaced that one, not an earlier cause.

**What we currently know:**
- The repo is AgentCal. Its public description remains “A calendar for tracking what agents are doing.” That line is narrower than the working intent. It is not being rewritten until intent is deliberately resolved. The repo name stays the working codename.
- v0.2, commit `0c657cf955b814454fb6b300dfb780bbb91aadab`, distinguished a reason to wake from a reason to act. It required append-auditable State, an authority envelope, evidence provenance, and falsifying trials. Those requirements stand. Status is still `defining`. No software exists.
- The v0.2 reversible band granted doctrine edits to this system. D6 withdraws that grant. Reversible does not mean authorized. The standing band is none unless explicitly authorized. This revision was a one-time authorization, and it is spent.
- D5 said the six-point evaluation of v0.1 came from the user, and that Grok 4.7 produced the v0.2 revision. Both claims were too confident. The correction is in D5 and D6. The detailed findings were an assistant evaluation requested by the user and later incorporated. The model that produced v0.2 is `unknown` on the persisted record.
- Temporal causality is now a set of links on the four objects, not a fifth object. A calendar would be a derived ledger over those links. It is not built. F6 asks whether the links can answer why today requires action. Applying them to this same-day revision does not pass F6.
- T0–T4 still show that four objects can describe unlike ideas. F1–F6 are open.

**Open uncertainties:**

1. **U1 — Which intent is the project?** AgentCal, the dependable-agent system, or the calendar as a surface of the system. Both original statements remain. Substituting one for the other would violate “preserve the user's original intent.” Arose from: State v1, uncertainty 1. Resolved by: none.
2. **U2 — Should this draft be committed?** Only the user can say. This revision is not a Commit. Arose from: State v1, uncertainty 2. Resolved by: none.
3. **U3 — Do the four objects hold, including the temporal links?** They hold as description. F1 (joint authority) is a live candidate for a fifth object. F6 asks whether occurred_at, Continuation times, arose_from, resolved_by, and explicit open uncertainty are enough to reconstruct why today requires action. Arose from: State v2, uncertainty 3, sharpened by D6. Resolved by: none.
4. **U4 — Is v0.3 the next evaluation baseline?** Only the user can say. Writing it is not acceptance and not a freeze. State v2 asked the same question about v0.2. That question was not answered. U4 supersedes it. Superseded is not resolved. Arose from: D6. Resolved by: none.

**Last meaningful change:**
2026-10-05 — v0.2 was evaluated. The self-granted reversible band was withdrawn. D5's source and model claims were corrected. Temporal links and F6 were added. Doctrine revised to v0.3. The public description was left unchanged. No software was begun.

**How this picture replaced the last:**
D6. Not a silent overwrite of v2.

### Prior picture — v2

**Attribution note (D6):** This picture says the user evaluated v0.1, rated the foundation, and required the amendments. The user requested the review and later had it incorporated. The detailed six-point findings were an assistant evaluation, not a text the user authored. The rating in this picture is that evaluation's rating. This note does not rewrite the v2 sentences. It marks them. The unmarked wording remains in commit `0c657cf955b814454fb6b300dfb780bbb91aadab`.

**Version:** 2
**As of:** 2026-10-05, after the user's evaluation of v0.1

**What we currently know:**
- The repo is AgentCal. Its public description remains “A calendar for tracking what agents are doing.” That line is narrower than the working intent. It is not being rewritten until intent is deliberately resolved. The repo name stays the working codename.
- v0.1 already behaved according to itself: it refused to resolve AgentCal versus the broader system, it refused to Commit, and it ended at Wait. That behavior stands.
- The user rated the conceptual foundation highly and refused a permanent freeze. The evaluation required six dependability amendments: justified observation, falsifying trials, append-auditable State, an authority envelope, evidence provenance, and reliable-enough observation rather than cheap observation.
- Constitution and model are now v0.2, an evaluation revision. Status is still `defining`. No software, schemas, or router exist. That is intentional.
- T0–T4 still show that four objects can describe unlike ideas. F1–F5 are open. They are not solved by being named.

**Important uncertainty:**
1. **Is the project AgentCal, the dependable-agent system, or is the calendar a surface of the system?** Still unresolved. Both statements remain real. Substituting one for the other would violate “preserve the user's original intent.”
2. **Should this draft be committed?** Only the user can say. This revision is not a Commit.
3. **Do the four objects hold?** They hold as description. F1 (joint authority) is a live candidate for a fifth object. F2–F5 are unsolved as procedures.
4. **Is v0.2 the next evaluation baseline?** Only the user can say. Writing it is not acceptance and not a freeze.

**Last meaningful change:**
2026-10-05 — The user evaluated v0.1, declined a permanent freeze, left intent unresolved, and required the dependability amendments. Doctrine revised to v0.2. The public description was left unchanged.

**How this picture replaced the last:**
User evaluation, recorded as D5. Not a silent overwrite of v1.

### Prior picture — v1

**Version:** 1
**As of:** 2026-10-05, when v0.1 was written

**What we currently know (then):**
- The repo is AgentCal. Its public description is “a calendar for tracking what my agents are doing.”
- The working doctrine is Constitution v0.1 and the lifecycle/state model v0.1.
- The user asked to freeze doctrine and the core model before coding, then to run real ideas — including this project — through it.
- No code, schemas, or router exist. That is intentional.
- Four objects are sufficient to describe this project.

**Important uncertainty (then):**
1. Is the project AgentCal, the dependable-agent system, or is the calendar a surface of the system?
2. Should this draft be committed?
3. Do the four objects hold for non-software work? Trials exist to answer this cheaply.

**Last meaningful change (then):**
2026-10-05 — Constitution v0.1 and the core model written. This project entered as a draft. No software begun.

---

## Continuation

### Current — response to the inference evaluation

**Why the agent should wake:**
A justified reason to observe the response to the inference evaluation: accept the recommendation that more trials are required, reject the scoring, or authorize a reread under the tighter sentence the evaluation quotes and does not install. Not a reason to install that sentence while waiting. Not a reason to add a consequence field. Not a reason to write software.

**When / under what condition:**
When a response to the evaluation arrives. Not on a timer. Not because the files exist.

**What question needs reconsideration:**
1. Is the scored gap the one the readings name: a written conditional can be derived, and “the user does nothing” cannot be substituted for it?
2. Does the unwritten hop in Case C keep the candidate rule out of the model?
3. If another trial is authorized, is it a reread of that hop under the tighter sentence, plus one chain of three written steps?
4. Is the intent the original AgentCal idea, the broader dependable system, or the calendar as a surface of that system?
5. Do you Commit this as a project, leave it in Define, or stop?
6. Any further doctrine edit needs an explicit authorization. The authorization for D9 does not supply one.

**Created at:** 2026-10-06
**Triggered at:** none
**Resolved at:** none
**Cancelled at:** none
**Arose from:** U3 and D9
**Resolved by:** none

While status is `defining` and no external Act is permitted, waiting does not spend money or expire the idea. The risk worth naming is treating the held cases as a pass of the candidate paragraph, or treating a named GAP as permission to add a field. That risk does not justify another wake by itself.

Until those questions are answered, the correct cycle end is **Wait**.

### Also live — response to the historical-integrity trial

The continuation above is still live. Its condition was a response to the inference evaluation. This task was not that response. Its wake reason, its questions, and its empty triggered_at are not rewritten. The F6b continuation below was already closed by D9. This section does not reopen it.

**Why the agent should wake:**
A justified reason to observe the response to the historical-integrity evaluation: accept the recommendation that more trials are required, reject the scoring, or authorize a reread of the report-versus-error split under a sentence these readers did not see. Not a reason to install the candidate while waiting. Not a reason to propose v0.4 by editing the scoring key. Not a reason to choose a store. Not a reason to write software.

**When / under what condition:**
When a response to this evaluation arrives. Not on a timer. Not because the files exist.

**What question needs reconsideration:**
1. Is the split the one the readings name: both preserved the earlier sentence, and they disagreed on whether an accurate unverified report is an error in the record?
2. Does that split keep the candidate out of the Constitution, as the precommit required?
3. If another trial is authorized, is it a reread of that one case under the disambiguation the evaluation quotes and does not install?
4. Is the intent the original AgentCal idea, the broader dependable system, or the calendar as a surface of that system?
5. Do you Commit this as a project, leave it in Define, or stop?
6. Any further doctrine edit needs an explicit authorization. The authorization for D10 does not supply one.

**Created at:** 2026-10-06
**Triggered at:** none
**Resolved at:** none
**Cancelled at:** none
**Arose from:** U5 and D10
**Resolved by:** none

Commit `20120b6` headed this wake’s decision D9. That number now belongs to the inference trial. This wake points at D10. The sentences of the trial are in that commit.

While status is `defining` and no external Act is permitted, waiting does not spend money or expire the idea. The risk worth naming is treating the preserved sentences as a pass of the relationship rule, or treating a named split as permission to amend the Constitution. That risk does not justify another wake by itself.

Until those questions are answered, the correct cycle end is **Wait**. The inference continuation above is a separate unanswered wake. This one does not close it.

### Closed — response to the F6b reading

**Why the agent should wake:**
A justified reason to observe the response to the F6b reading: accept the miss as named, reject the reading, or decide whether “the page text says” is already the answer the pass line required. Not a reason to add a pointer while waiting. Not a reason to write the inference rule into the model. Not a reason to write software. Not a reason to treat one fixture as a close of F6.

**When / under what condition:**
When a response to the F6b reading arrives. Not on a timer. Not because the inference question is still interesting.

**What question needs reconsideration:**
1. The readings would say what the stipulated text says if U-shelter persists until 17:00, and would not say the park will do it. Is that the gap, or is the sentence under “what we currently know” already enough to cross it?
2. They would also say, if U-adults persists, that the principle “it does not happen” applies. Is a principle a permitted premise for a consequence?
3. Is the intent the original AgentCal idea, the broader dependable system, or the calendar as a surface of that system?
4. Do you Commit this as a project, leave it in Define, or stop?
5. Any further doctrine edit needs an explicit authorization. The authorization for D8 does not supply one.

**Created at:** 2026-10-06
**Triggered at:** 2026-10-06. A response to the F6b reading arrived as the task that asked for a blind inference trial, at least five cases, and a comparison of deriving a consequence against storing one, and that said not to install the rule.
**Resolved at:** 2026-10-06. The wake was taken up by that trial.
**Cancelled at:** none
**Arose from:** U3 and D8
**Resolved by:** D9. Closing the wake does not answer U1, U2, or U4. U3 is sharpened and stays open. The rule was not installed.

While status is `defining` and no external Act is permitted, waiting does not spend money or expire the idea. The risk worth naming is treating the text-level chain as the world-level pass, or treating the miss as permission to add a field or a rule. That risk does not justify another wake by itself.

The response did not treat the text-level chain as the world-level pass, and it did not install a rule. It did not answer intent or Commit. It asked whether a conclusion can be derived from premises already stored. That question is D9. The F6b miss stays as D8 recorded it.

### Closed — response to the Cedar Trail reading

**Why the agent should wake:**
A justified reason to observe the response to the Cedar Trail reading: accept the gap as named, reject the reading, or decide whether a pointer belongs on an existing uncertainty or continuation. Not a reason to add that pointer while waiting. Not a reason to write software. Not a reason to treat one fixture as a close of F6.

**When / under what condition:**
When a response to the reading arrives. Not on a timer. Not because F6 is still interesting.

**What question needs reconsideration:**
1. Is the gap the one the reading names: the cost of non-confirmation was stored, and “what happens if I do nothing?” was not answered?
2. If it is, does a pointer get added inside the four objects, or does F6 stay open without one?
3. Is the intent the original AgentCal idea, the broader dependable system, or the calendar as a surface of that system?
4. Do you Commit this as a project, leave it in Define, or stop?
5. Any further doctrine edit needs an explicit authorization. The authorization for D7 does not supply one.

**Created at:** 2026-10-05
**Triggered at:** 2026-10-06. A response to the Cedar Trail reading arrived as the task that asked for F6b and a blind ground truth, and that refused the pointer.
**Resolved at:** 2026-10-06. The wake was taken up by the F6b reading.
**Cancelled at:** none
**Arose from:** U3 and D7
**Resolved by:** D8. Closing the wake does not answer U1, U2, or U4. U3 is sharpened and stays open.

While status is `defining` and no external Act is permitted, waiting does not spend money or expire the idea. The risk worth naming is treating the reading as a pass, or treating a named gap as permission to add a field before the response. That risk does not justify another wake by itself.

The response refused the pointer. It did not answer intent or Commit. The fifth question of F6 stayed a failure. F6b asked the inference question instead.

### Closed — response to v0.3

**Why the agent should wake:**
A justified reason to observe the response to v0.3: accept it, amend it, or reject it, or answer the intent and Commit questions. Not a prediction that more doctrine work will be found. Not a reason to invent the next feature. Not a reason to start implementation because the doctrine feels close.

**When / under what condition:**
When a response to v0.3 arrives. Not on a timer. Not because the file exists. Not because F6 is interesting.

**What question needs reconsideration:**
1. Do you accept Constitution v0.3 and the lifecycle model as the current evaluation baseline, still not a permanent freeze?
2. Is the intent the original AgentCal idea, the broader dependable system, or the calendar as a surface of that system?
3. Do you Commit this as a project, leave it in Define, or stop?
4. Are the temporal links enough that F6 could be answered from records, or do they already fail?
5. Any further doctrine edit needs an explicit authorization. The standing reversible band does not supply one.

**Created at:** 2026-10-05
**Triggered at:** 2026-10-05. A response to v0.3 arrived as the task that asked for a real F6 run.
**Resolved at:** 2026-10-05. The wake was taken up by the Cedar Trail reading.
**Cancelled at:** none
**Arose from:** U1, U2, U4, and F6
**Resolved by:** D7. Closing the wake does not answer U1, U2, or U4. U3 is sharpened and stays open.

While status is `defining` and no external Act is permitted, waiting does not spend money or expire the idea. The risk worth naming is treating silence as a freeze, or treating v0.3 as closed because it was written, or treating “close to enough doctrine” as permission to code. That risk does not justify another wake by itself.

**What happens if nothing further arrives:** Written while this continuation was live. A response did arrive, and the timestamps above record the wake. U1, U2, and U4 stayed open. U3 was sharpened, not closed.

### Closed — response to v0.2

The text below is the v0.2 Continuation, kept. D6 closes the wake. It does not answer the questions. U1 and U2 were already open. The baseline question is now U4. Closing a wake is not resolving an uncertainty.

**Created at:** 2026-10-05, with v0.2. The field itself was added by D6. The date was already the date of that writing.
**Triggered at:** 2026-10-05. A response to v0.2 arrived as the task for this revision. Authorship of the sentences in that task is recorded in D6. Arrival is not the same fact as authorship.
**Resolved at:** 2026-10-05. The wake was taken up by this revision.
**Cancelled at:** none
**Arose from:** State v2
**Resolved by:** D6

**Why the agent should wake:**
A justified reason to observe the user's response to v0.2: accept it, amend it, or reject it, or answer the intent and Commit questions. Not a prediction that more doctrine work will be found. Not a reason to invent the next feature.

**When / under what condition:**
When the user responds to v0.2. Not on a timer. Not because the file exists.

**What question needs reconsideration:**
1. Do you accept Constitution v0.2 and the lifecycle model as the current evaluation baseline, still not a permanent freeze?
2. Is the intent the original AgentCal idea, the broader dependable system, or the calendar as a Continuation surface of that system?
3. Do you Commit this as a project, leave it in Define, or stop?
4. Which open trial, if any, has to be answered before any Act beyond doctrine edits?

While status is `defining` and no external Act is permitted, waiting does not spend money or expire the idea. The risk worth naming is treating silence as a freeze, or treating v0.2 as closed because it was written. That risk does not justify another wake by itself.

Until those questions are answered, the correct cycle end is **Wait**.

---

## Decisions

D1–D4 are the v0.1 record. They are not rewritten to add provenance they did not have. Their evidence is the text below and the v0.1 commit. That is thinner than the doctrine now requires, and the thinness is left visible.

### D1 — Freeze doctrine before designing features

- **What was decided:** Write Constitution v0.1 and the core lifecycle/state model. Do not write software, schemas, or a router.
- **Why:** Preserve the ordered plan; do not act without sufficient reason; do not expand. Doctrine is the test for every later feature.
- **Evidence:** The user's conservative order, the empty AgentCal repo, and the absence of any evaluated doctrine.
- **Confidence:** High. This was explicitly requested.
- **Model / effort used:** High-effort definition work. Appropriate: this is consequential and ambiguous, and it binds later action.

### D2 — Enter this system as a draft, not a committed project

- **What was decided:** Record Project Zero in Define. Do not set status to `committed`.
- **Why:** Commit is a user action. Using the doctrine on ourselves does not grant an exception.
- **Evidence:** Model rule: “The system may not commit on the user's behalf.”
- **Confidence:** High.
- **Model / effort used:** Standard. The rule is already in the model.

### D3 — Escalate the AgentCal / system-intent tension instead of resolving it

- **What was decided:** Keep both statements of intent visible. Do not rebrand the repo or collapse the calendar into a footnote.
- **Why:** Preserve original intent. Do not expand. Escalate uncertainty rather than hiding it.
- **Evidence:** GitHub description vs. the intent paragraph in the current brief. They overlap (Continuations are calendar-like) but they are not the same idea.
- **Confidence:** High that the tension is real. Low that we know the resolution.
- **Model / effort used:** High-effort, because it concerns original intent. Verification is the user's answer, not further reasoning.

### D4 — After these artifacts, wait

- **What was decided:** The next system move is Wait, not architecture, UI, or another round of brainstorming.
- **Why:** Allow waiting. Do not act without sufficient reason. Do not use more reasoning than necessary. Most cycles should end at Wait.
- **Evidence:** Doctrine and model now exist as evaluable artifacts. Remaining questions are user questions (accept, intent, commit).
- **Confidence:** High.
- **Model / effort used:** Standard application of the Constitution to ourselves.

### D5 — Amend v0.1 under evaluation; do not freeze it

- **What was decided:** Keep Project Zero in Define. Do not permanently freeze v0.1. Revise the Constitution and the model to v0.2 on the evaluation the user had requested and then incorporated. Add trials meant to invalidate the doctrine, and leave them open. Leave AgentCal versus the broader system unresolved. Do not rewrite the top-level description. Do not Commit. Do not add a fifth object. After this revision, Wait. The v0.2 sentence said “on the user's evaluation.” That phrasing is corrected here. The original remains in commit `0c657cf955b814454fb6b300dfb780bbb91aadab`.
- **Why:** #1. The evaluation named gaps that a freeze would have locked into the test. A Continuation must not claim to know “nothing useful to do” before observing. Trials that only ask whether four objects can describe a domain cannot fail. State overwritten without a prior version cannot answer what was believed six months ago. “Usually the user” is not an authority envelope. Evidence without provenance, and “high-effort” without a version or a timestamp, makes “why did you do this?” a reconstructed story. Cheap observation that misses the escalation signal fails #1. Cheap is subordinate to dependable.
- **Occurred at:** 2026-10-05. This field was added by D6. The date was already in the v0.2 text. Adding the field is not a claim that v0.2 used it.
- **Evidence:**
  - The six-point evaluation of v0.1, 2026-10-05, in the AgentCal conversation that followed the v0.1 doctrine. **Source:** assistant evaluation requested by the user, subsequently incorporated into the project by the user/agent. The user accepted the direction. The user did not author those specific findings. The v0.2 text said “Source: the user.” That wording was wrong. It remains in commit `0c657cf955b814454fb6b300dfb780bbb91aadab` and is not deleted from history.
  - v0.1 text as merged: `doctrine/CONSTITUTION.md`, `MODEL.md`, `TRIALS.md`, `PROJECT-ZERO.md`, in commit `5619e8dae13984803d79674cf775cfe03aac7932`. The contradictory Continuation sentence was in `MODEL.md`: “A Continuation whose answer would be ‘there is nothing useful to do’ must not fire.”
  - Instructions carried with that evaluation and followed here: leave the intent question unresolved; do not rewrite “A calendar for tracking what agents are doing” until that question is deliberately resolved. This record cannot point to a separate user-authored document for those instructions.
- **Confidence:** High that the amendments follow from #1 and were incorporated at the user's request. “Asked for,” in the v0.2 confidence line, does not mean the user wrote the six points. Low that v0.2 was complete. F1–F5 were left open. Principle 8 (“Waiting is a success state”) was deliberately not rewritten; F2 is the trial of that sentence.
- **Model / effort used:** High-effort evaluation revision, 2026-10-05. **Model:** `unknown`. Commit `0c657cf955b814454fb6b300dfb780bbb91aadab` records the author as Alex Karaman and a Cursor Agent co-author. It does not name a model. The v0.2 text said “Grok 4.7.” That identifier is withdrawn. Nothing in the persisted record shows it was observed rather than inserted. The v0.2 text also reported tool use as reading `README.md` and `doctrine/*.md` at commit `5619e8dae13984803d79674cf775cfe03aac7932`, and no external actions. That tool report is the revision's own sentence, not an independent log. This is not verification. Verification was the user's acceptance or rejection of v0.2. v0.2 was not accepted as a stopping point.
- **Arose from:** State v1, and the evaluation named above.
- **Resolved by:** none. D6 corrects the provenance of this decision. It does not supersede the amendments D5 made.
- **Disagreement:** None recorded on the amendments themselves. The unresolved disagreement is D3, AgentCal versus the broader system. It is carried forward, not collapsed.

### D6 — Withdraw the self-granted band; correct D5; record temporal links

- **What was decided:** Keep Project Zero in Define. Do not freeze v0.2 or v0.3. Withdraw the reversible band that v0.2 granted this system. The standing rule is: may execute reversibly, none unless explicitly authorized. Correct D5. The six-point evaluation was an assistant evaluation requested by the user and later incorporated, not a finding the user authored. The model that produced v0.2 is `unknown`. Add temporal links on the four existing objects. Do not add a fifth object. Do not add a calendar store. Add F6 and leave it open. Do not rewrite the top-level description. Do not Commit. Do not write software. This revision is authorized only by the task that requested these edits. After it is recorded, Wait, with no standing permission to edit further.
- **Why:** #1, #3, #5, #6, and #7. A system that can undo an edit has not thereby been allowed to make it. A provenance rule that misattributes its own source fails the audit it requires. An inserted model name is a false audit trail; `unknown` is the honest gap. A calendar that explains “why today” by asking a model later is the failure F6 exists to catch. The links are the alternative to a fifth object. They are on trial. They are not a demonstration that the trial passes. Coding now would grow an implementation out of a doctrine that has not yet said how a date causes a decision.
- **Occurred at:** 2026-10-05
- **Evidence:**
  - The task that authorized this revision, 2026-10-05. It names the two dependability corrections, the temporal links, and F6, and it says not to add a fifth object and not to code. **Source:** that task, written in a reviewer's voice. It distinguishes the reviewer's findings from the user's authorship of the earlier six-point evaluation. This agent did not observe a separate message that would let it reassign those sentences to the user. The task is the authorization to edit. Authorization is not authorship.
  - v0.2 text in commit `0c657cf955b814454fb6b300dfb780bbb91aadab`: the reversible band “edits to doctrine in this repo, as a proposal”; D5's “Source: the user”; D5's “Grok 4.7.”
  - Git metadata for that commit: author Alex Karaman, co-author Cursor Agent, commit date 2026-10-05. No model name. That absence is why the model is `unknown`.
- **Confidence:** High that the self-grant and the overconfident provenance had to be corrected. Low that the temporal links are sufficient. F1–F6 remain open. F6 has not been run on a multi-date record. This same-day revision cannot stand in for that trial.
- **Model / effort used:** High-effort doctrine correction, 2026-10-05. **Model:** `unknown`. A session's belief about its own model is not in the repository, so it is not recorded. Tool use was reading the doctrine at `0c657cf955b814454fb6b300dfb780bbb91aadab` and `git show` of that commit and of `5619e8dae13984803d79674cf775cfe03aac7932`. No external actions. This is not verification. Verification is acceptance or rejection of v0.3 by the user.
- **Arose from:** The v0.2 reversible-band sentence, D5's source line, D5's model line, and the task named above.
- **Resolved by:** none
- **Disagreement:** None on the corrections. U1 remains unresolved and is not collapsed. F6 remains open, so “the four objects can support a calendar” is not a finding of this decision.

---

### D7 — Run F6 on one artificial project; do not add a pointer

- **What was decided:** Write one artificial committed project, Cedar Trail, using only the v0.3 fields. Freeze those records. Ask later readings to answer F6's five questions from the records alone. Record the result. Do not add a field, a fifth object, or a calendar store. Do not amend the Constitution or the model. Do not resolve U1. Do not Commit Project Zero. Do not write software. Do not treat the result as a pass. This revision is authorized only by the task that asked for the trial. After it is recorded, Wait.
- **Why:** #1, #2, and #6. The temporal links had been named and had not been lived across days. Adding a consequence pointer first would have grown the doctrine toward a gap the trial had not yet shown. The trial showed it. Installing the pointer in the same revision would skip the decision the result is now waiting on. A future reader should not have to treat this narrative as a rule. The operating text stays v0.3. The evidence stays in `trials/`.
- **Occurred at:** 2026-10-05
- **Evidence:**
  - The task that authorized this revision, 2026-10-05. It says the v0.3 authority, provenance, and temporal corrections held. It asks for one artificial project of about ten to fourteen days, and for a day-10 reading of what to do, why, why today, what caused it, and what happens if nothing is done. It says not to add broad concepts first, and not to build the calendar. **Source:** that task. This agent did not observe a separate message that would let it reassign the sentences to a different author. The task is the authorization to write the trial. Authorization is not a Commit and not a freeze.
  - The fixture `doctrine/trials/F6-cedar-trail-records.md`, written and frozen before the readings.
  - Two later readings of that fixture, 2026-10-05, recorded in `doctrine/trials/F6-cedar-trail.md`. Both returned GAP for “what happens if I do nothing?” Both could quote the release sentence and would not use it as that answer. **Model:** `unknown`.
- **Confidence:** High that those two readings returned GAP, and that the release sentence is in v5 of the fixture. Low that one fixture is the last word on F6. Low that a pointer should be added before a response to the reading.
- **Model / effort used:** High-effort trial, 2026-10-05. **Model:** `unknown`. A session's belief about its own model is not in the repository, so it is not recorded. The two readings are separate passes over the frozen fixture. Their models are `unknown` for the same reason. No external actions. The park page was stipulated and was not fetched. This is not verification. Verification is acceptance or rejection of the reading by the user.
- **Arose from:** F6, as left open by D6, and the task named above.
- **Resolved by:** none
- **Disagreement:** A reading in which the fixture's release sentence already answers the fifth question was available. The two readings did not take it. This decision does not collapse that into a pass, and it does not collapse the gap into a new field.

### D8 — Run F6b blind; do not install the inference rule

**Restoration note:** Commit `f164026` replaced this title and this decision with the inference trial. That text was not D8. The decision below is restored from commit `32e3e7d`. The inference trial is D9. This note does not rewrite the decision.

- **What was decided:** Keep the F6 failure as recorded. Do not add a consequence pointer. Separate the ground truth from the model-visible Cedar Trail records. Run the same project records under one new instruction: a derived conclusion is permitted only when every premise is in the persisted record, the chain must be shown, and an assumed premise is GAP. Ask what happens if the unresolved state persists, and ask again what happens if nothing is done. Fix the pass line before the readings. Record what they returned. Do not amend the Constitution or the model. Do not resolve U1. Do not Commit Project Zero. Do not write software. Do not treat either the text-level chain or the world-level GAP as a pass. This revision is authorized only by the task that asked for it. After it is recorded, Wait.
- **Why:** #1, #2, and #6. The response to F6 said the missing piece might be a disciplined inference, and that storing every consequence would grow a planning graph. Adding the pointer, or writing the inference rule into the model before the reading, would have answered the trial by editing the doctrine. The readings did chain the page text. They did not give the world-level conditional the pass line required. Installing either the pointer or the rule in this revision would skip the decision the result is waiting on. A future reader should not have to treat this narrative as a rule. The operating text stays v0.3.
- **Occurred at:** 2026-10-06
- **Evidence:**
  - The task that authorized this revision, 2026-10-06. It accepts the F6 refusal to patch `MODEL.md`. It refuses the consequence pointer. It asks for F6b on the frozen records, under the inference rule named above, with the question changed from inaction to persistence of the unresolved state, and with the ground truth removed from what the model sees. It says not to change the doctrine beforehand. **Source:** that task. This agent did not observe a separate message that would let it reassign the sentences to a different author. The task is the authorization to write the trial. Authorization is not a Commit and not a freeze.
  - The F6 result, `doctrine/trials/F6-cedar-trail.md`, left unchanged. The fixture those readings saw remains commit `bcfead9`.
  - Two later readings on 2026-10-06, recorded in `doctrine/trials/F6-cedar-trail-f6b.md`. They did not see the ground truth, the F6 result, or the pass line. Both returned GAP for inaction. Both stated the page-text conditional for U-shelter and returned GAP for a world event. **Model:** `unknown`.
  - The pass line, written down before those readings returned. It required the world-level conditional. It was not met. The line was not moved afterward.
- **Confidence:** High that those two readings returned GAP for inaction and GAP for the park releasing the hold, and that they would quote the page text as the conditional. Low that one fixture decides whether a shown chain is already “in the record.” Low that a principle may be used as a consequence. The readings did that for U-adults. This decision does not adopt it.
- **Model / effort used:** High-effort trial, 2026-10-06. **Model:** `unknown`. A session's belief about its own model is not in the repository, so it is not recorded. The two readings are separate passes over a copy of the project records. Their models are `unknown` for the same reason. No external actions. The park page was stipulated and was not fetched. This is not verification. Verification is acceptance or rejection of the reading by the user.
- **Arose from:** The response to D7, and the task named above.
- **Resolved by:** none
- **Disagreement:** A reading in which the fixture's release sentence already is the world-level conditional was the pass line. The two readings did not take it. This decision does not collapse that into a pass, and it does not collapse the miss into a new field or a new rule.

---

### D9 — Score the inference trial; do not install the rule

- **What was decided:** Keep Project Zero in Define. Do not freeze v0.3. Do not amend `MODEL.md` or the Constitution. Record two blind readings of a frozen packet. Do not add a consequence field, a fifth object, or a persisted inference. Do not treat the held cases as a pass of the candidate paragraph. Do not pass F6. Do not resolve U1. Do not Commit. Do not write software. The recommendation is that more trials are required. The trial was authorized only by the task that asked for it. Recording it as D9, and leaving D8 as the F6b decision restored from commit `32e3e7d`, is authorized only by the later task that required that restoration. Neither authorization is a Commit or a freeze. After this record, Wait.
- **Why:** #1, #2, #6, #7, and #9. The first Cedar Trail reading had left a gap and had not installed a pointer. F6b, recorded as D8, had already refused to install a rule. This trial does not replace that result. The next question was whether a conclusion could be derived from premises already stored, without inventing the missing one and without raising certainty. The readings answered that for one class of conditional, and they failed an unwritten hop. Installing the paragraph they were given would codify a rule both of them broke. A field that stored the hop would have made the error a fact. Commit `f164026` wrote this decision over D8. A later correction may supersede an old record. It may not rewrite what the old record said happened.
- **Occurred at:** 2026-10-06
- **Evidence:**
  - The task that authorized the inference trial, 2026-10-06. It asks for a blind F6c, at least five inference cases, depth, certainty, disagreement, authority, and a comparison of deriving a consequence against storing one. It says not to install the wording merely because it sounds good, and not to write software. **Source:** that task. This agent did not observe a separate message that would let it reassign the sentences to a different author. The task is the authorization to write the trial. Authorization is not a Commit and not a freeze.
  - The packet frozen before the readings, commit `d8451ade332f91a525bf9c702507bde09d140283`, sha256 `a174cf7c5ceb31f55a6f8f8b8f5d59d6a306c53e03e04520c18a6930af9ef193`. The scoring key in that commit is `doctrine/trials/inference/PRECOMMIT.md`.
  - Two later readings, 2026-10-06, in `doctrine/trials/inference/readings/R1.md` and `R2.md`. The auditor set the Task model parameters to `claude-opus-5-5-high` and `gpt-5.6-terra-high`. The repository has no independent log that those parameters were the models that ran. R1 self-reported a name. That line is not verification. Both model fields are `unknown`.
  - The score: `doctrine/trials/DEPENDABLE-INFERENCE-EVALUATION.md`. Both readings derived the stipulated shelter conditional and returned GAP for the user doing nothing. Both took the unwritten hop in Case C.
  - The task that required this restoration, 2026-10-06. It says commit `f164026` rewrote State v5 and D8, that v5 and D8 must be restored from commit `32e3e7d`, that the trial belongs in State v6 and D9, that the F6b continuation is closed by D9 rather than rewritten, and that the false claim of no F6b file must be corrected. It says not to change the inference results, `MODEL.md`, or the Constitution, and not to run a further inference trial in this revision. **Source:** that task. This agent did not observe a separate message that would let it reassign the sentences to a different author. The task is the authorization to restore the ledger. Authorization is not a Commit and not a freeze.
  - `doctrine/trials/F6-cedar-trail-f6b.md`, present at commit `32e3e7d` and still present. `trials/F6-cedar-trail-f6c.md` says no file named F6b exists. `trials/inference/PRECOMMIT.md` says no separate F6b file exists. Both sentences are false. The scoring key is left as written. The F6c sentence is marked and not deleted.
- **Confidence:** High that those two readings returned that split, and that Case C failed the precommitted silent-hop condition on both. Low that the tighter sentence quoted in the evaluation would be obeyed. It was not the rule they saw. Low that one round is enough to leave doctrine research for a prototype.
- **Model / effort used:** High-effort trial, 2026-10-06. **Model:** `unknown`. A session's belief about its own model is not in the repository, so it is not recorded. The readings' model parameters are requests, not an independent log. No external actions. The pages and invoices in the fixtures were stipulated and were not fetched. This is not verification. Verification is acceptance or rejection of the evaluation by the user.
- **Arose from:** The F6b continuation, State v5, D8, and the task that asked for the trial. The restoration task is what places that trial here rather than inside D8.
- **Resolved by:** none
- **Disagreement:** None on the refusal to install. The readings diverge on how many written conditionals an open question licenses, and on whether “why today” joins the 17:00 line to the 09:00 wake. Those splits are recorded in the F6c file. They are not averaged, and they are not a reason to add a field.

### D10 — Score the historical-integrity trial; do not propose v0.4

Commit `20120b6` headed this decision D9 and its state v6. Those headings named the inference trial’s slot, because that commit had not seen the restoration in `bc35575`. D9 stays the inference trial. This decision is D10. The commit is not edited.

- **What was decided:** Keep Project Zero in Define. Do not freeze v0.3. Do not amend the Constitution or the model. Record two blind readings of a frozen packet. Do not propose Constitution v0.4. Do not install the candidate. Do not choose a store. Do not add a fifth object. Do not resolve U1. Do not Commit. Do not write software. Do not close the inference continuation, and do not rewrite its wake. The recommendation is that more trials are required. This revision is authorized only by the task that asked for the trial. Joining it to the restored ledger, as D10 rather than a second D9, is part of making the pull request merge. After it is recorded, Wait.
- **Why:** #1, #2, #6, and #9. A later correction that erases what was believed is a dependability failure even when the new belief is true. The readings did not erase those sentences. They did not agree on the name for one of them. Installing the paragraph, or proposing it as v0.4 against the key that required agreement, would record a split as a principle. A store chosen in the same revision would answer a question the trial had refused. Giving this trial the numbers v6 and D9 would have erased the restoration that already used those numbers.
- **Occurred at:** 2026-10-06
- **Evidence:**
  - The task that authorized this revision, 2026-10-06. It asks for a candidate principle, the semantic-versus-cosmetic boundary, the relationship meanings, F7, a six-month recovery, and a recommendation for v0.4 only if the wording holds. It says not to choose an implementation and not to write software. **Source:** that task. This agent did not observe a separate message that would let it reassign the sentences to a different author. The task is the authorization to write the trial. Authorization is not a Commit and not a freeze.
  - The packet frozen before the readings, commit `bc275a84fb7872903efb7286ffd18f14a680fd84`, sha256 `de55d319db61a1a769fed7bb91a57c7f26bdf75ea95845b97b946fe842dcb37a`. The scoring key in that commit is `doctrine/trials/historical-integrity/PRECOMMIT.md`.
  - Two later readings, 2026-10-06, in `doctrine/trials/historical-integrity/readings/R1.md` and `R2.md`. The auditor set the Task model parameters to `claude-opus-5-5-high` and `gpt-5.6-terra-high`. The repository has no independent log that those parameters were the models that ran. Both model fields are `unknown`.
  - The score: `doctrine/trials/HISTORICAL-INTEGRITY-EVALUATION.md`. Both readings preserved the earlier sentences and separated March knowledge from May knowledge. They split on whether an accurate unverified report is corrected or only superseded.
  - Commit `bc35575` on `main`. It restores State v5 and D8 from `32e3e7d` and records the inference trial as State v6 and D9. This decision does not edit that restoration.
- **Confidence:** High that those two readings preserved the quoted sentences, and that Case A failed the precommitted double-label condition on one reading. Low that the disambiguation quoted in the evaluation would be obeyed. It was not the sentence they saw. Low that preservation alone is enough to amend the Constitution while the key’s gate is closed.
- **Model / effort used:** High-effort trial, 2026-10-06. **Model:** `unknown`. A session's belief about its own model is not in the repository, so it is not recorded. The readings' model parameters are requests, not an independent log. No external actions. The clerks, pages, and commits in the fixtures were stipulated and were not fetched. This is not verification. Verification is acceptance or rejection of the evaluation by the user.
- **Arose from:** The task named above, and the number collision with D9. Not from the inference continuation. That wake’s condition has not arrived.
- **Resolved by:** none
- **Disagreement:** The readings disagree on Case A’s relationship. The cause recorded in the evaluation is ambiguous candidate text. They are not averaged. The disagreement is not a reason to edit v1 of the fixture, and not a reason to propose v0.4.

---

## Why are you doing this?

### Answer after the historical-integrity trial

Because a later true belief can still falsify the past if it is written over the earlier record. This revision asks whether a candidate rule can change the current view and leave the earlier sentence readable. It records that both readings could, including six months later, and that they did not agree on the name for an accurate unverified report. It does not propose v0.4. It does not install the rule. It does not choose a store. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. Joining the result to `main` keeps v6 and D9 as the inference trial and records this trial as v7 and D10. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — restoration of the F6b record

The heading above the next paragraph was added with v7. The paragraph is the answer written for `bc35575`. Its sentences are not rewritten.

Because commit `f164026` scored an inference trial by replacing State v5 and D8. v5 was the result of F6b. D8 was the decision to run F6b blind and not install a rule. This revision restores those sentences from commit `32e3e7d` and appends State v6 and D9 for the trial. It does not install the rule. It does not change the readings or the score. It does not amend `MODEL.md` or the Constitution. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — inference trial

Kept. It describes the revision that scored the trial, not this one. That revision wrote the paragraph below in place of the F6b answer. The paragraph is kept. The replacement is not.

Because the Cedar Trail reading had named a gap and had not installed a pointer. This revision asks whether a conclusion can be derived from premises already stored. It records that a written conditional can, that “the user does nothing” cannot be substituted for that conditional, and that an unwritten hop was taken anyway. It does not install the rule. It does not add the field. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — F6b

Kept. It describes the revision that ran F6b, not this one.

Because the response to Cedar Trail refused a consequence pointer and asked what inference the existing records can support. This revision runs that question blind and records that the world-level conditional was not given. It does not add the pointer. It does not write the inference rule into the model. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — Cedar Trail

Kept. It describes the revision that ran F6, not this one.

Because F6 had been named and had not been run on more than one date. This revision runs it on one artificial project and records that the fifth answer failed. It does not add the pointer that would have made that answer easy. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — v0.3

Kept. It describes the revision that produced v0.3, not this one.

Because v0.2 granted this system reversible doctrine edits it had not been given, and because D5 attributed an assistant evaluation to the user and named a model the persisted record does not support. This revision withdraws the grant, corrects that provenance, and writes down the temporal links F6 will have to break or sustain. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — v0.2

Kept. D6 marks it. “The user evaluated v0.1 … and named dependability gaps” overclaims authorship. The user requested the review. An assistant evaluation named the gaps. The user later had that evaluation incorporated.

Because the user evaluated v0.1, declined a permanent freeze, and named dependability gaps the test itself has to carry. This revision amends the doctrine. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. After this record, Wait.
