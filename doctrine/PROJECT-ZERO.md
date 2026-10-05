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

State is versioned. v1 is the picture at the v0.1 writing. v2 is the picture at the v0.2 writing. v3 is the picture at the v0.3 writing. v4 is current. Earlier pictures are not discarded.

### Current picture — v4

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

### Current — response to the Cedar Trail reading

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
**Triggered at:** none
**Resolved at:** none
**Cancelled at:** none
**Arose from:** U3 and D7
**Resolved by:** none

While status is `defining` and no external Act is permitted, waiting does not spend money or expire the idea. The risk worth naming is treating the reading as a pass, or treating a named gap as permission to add a field before the response. That risk does not justify another wake by itself.

Until those questions are answered, the correct cycle end is **Wait**.

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

---

## Why are you doing this?

Because F6 had been named and had not been run on more than one date. This revision runs it on one artificial project and records that the fifth answer failed. It does not add the pointer that would have made that answer easy. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — v0.3

Kept. It describes the revision that produced v0.3, not this one.

Because v0.2 granted this system reversible doctrine edits it had not been given, and because D5 attributed an assistant evaluation to the user and named a model the persisted record does not support. This revision withdraws the grant, corrects that provenance, and writes down the temporal links F6 will have to break or sustain. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. It does not leave a standing permission to edit again. After this record, Wait.

### Prior answer — v0.2

Kept. D6 marks it. “The user evaluated v0.1 … and named dependability gaps” overclaims authorship. The user requested the review. An assistant evaluation named the gaps. The user later had that evaluation incorporated.

Because the user evaluated v0.1, declined a permanent freeze, and named dependability gaps the test itself has to carry. This revision amends the doctrine. It does not build. It does not Commit. It does not resolve the original idea. It does not rewrite the public description. After this record, Wait.
