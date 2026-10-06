# Doctrine trials

**Purpose:** Ask whether the Constitution and the four objects hold, and where they fail.
**Method:** Confirmatory trials ask whether the objects can describe an idea. Falsifying trials try to invalidate the doctrine. Do not plan the work.
**Status:** Falsifying pass opened. Not committed projects. T0–T4 are the v0.1 confirmatory pass, retained.

Dependability requires falsifiability. “Can our four objects describe this?” is not enough. A trial that cannot fail cannot inform #1.

---

## Confirmatory trials (v0.1, retained)

These still matter. Their “yes” is the claim under test. It is not a result.

### T0 — This system (software + doctrine)

Covered in `PROJECT-ZERO.md`.

The lifecycle fits: we are in Define; Commit is a user act; the honest next state is Wait. The strain is real and useful: two plausible intents (AgentCal vs. dependable system) must not be silently merged.

**Doctrine holds** if we refuse to resolve that by expansion or rebranding.

### T1 — Research an investment

**Draft intent:** Decide whether to invest in a specific thing, or decide that no decision is warranted yet.

**Desired outcome:** A decision the user can own (buy, refuse, wait) with stated evidence and uncertainty — not a portfolio, not a watchlist, not ongoing coverage.

**Non-goals:** Trading, constant monitoring, “being in the market,” extra tickers, a research department.

**Likely cycle:** Observe → Decide → Wait. Act (placing money) is rare, irreversible, and belongs to the user. Evaluate is whether the decision still matches intent, not whether the price moved.

**Continuation:** A stated condition (filing, date, price threshold, “user asked again”). Not daily commentary.

**Where it would fail without the doctrine:** cheap models over-claim; the system acts on a hunch; six quiet months feel like failure; a model “completes” the project because it produced a memo the user does not trust.

**Same four objects?** Yes. State holds uncertainty. Decision holds confidence and effort. Continuation prevents waking to chatter.

### T2 — Plan a home remodel

**Draft intent:** Make a specific part of a home livable in a defined way (e.g. kitchen: these constraints, this budget class).

**Desired outcome:** A plan the user can execute or hand to a contractor — or a decision not to remodel.

**Non-goals:** Interior-design exploration as a lifestyle; fifty-item punch lists; shopping for its own sake.

**Likely cycle:** Define until scope is small enough to be true; then Observe (codes, costs, existing conditions) → Decide (one next reversible step) → Wait (permits, quotes, people).

**Continuation:** External events (quote returned, permit issued, user has a weekend). Not “keep planning.”

**Where it would fail without the doctrine:** the agent creates fifty tasks; expands “kitchen” into the whole house; treats waiting on a contractor as a problem to fill with activity.

**Same four objects?** Yes. Non-goals do the heavy lifting. “Fifty tasks” is refused at the Constitution, not at a task-prioritizer.

### T3 — Prepare a seminary paper

**Draft intent:** Make a particular argument, of a stated scope, for a stated course or question.

**Desired outcome:** A paper the user will submit, whose claim they still recognize as theirs.

**Non-goals:** Adjacent literature for completeness; a second paper; career advice; expanding the thesis because sources were interesting.

**Likely cycle:** Define the claim before gathering; Observe (sources) must not quietly rewrite intent; Act is drafting or requesting a source; much of the honest work is Wait between reading and writing.

**Continuation:** Deadline, user sitting down to write, or a specific unresolved question in the argument — not “there is still unread material.”

**Where it would fail without the doctrine:** original claim is substituted for a more impressive one; high-effort models over-write the user's voice; the system thinks the project is complete when a draft exists and the user does not.

**Same four objects?** Yes. Intent preservation is the whole game. Completion remains a user confirmation.

### T4 — Organize a youth event

**Draft intent:** Hold a specific event, on a real date, for a real group, with a small set of must-not-fail constraints (safety, adults, place).

**Desired outcome:** The event occurs as intended, then the project Completes.

**Non-goals:** A youth program; recurring calendar fill; “while we're at it” extra activities.

**Likely cycle:** Define until the event is one event; Observe (people, place, conflicts) → Decide → Act (a message, a booking) → Wait. After the date: Evaluate → Completed, if the user says so.

**Continuation:** RSVP changes, venue confirmation, a date approaching, or a justified reason to check whether anything has slipped. Calendar-like — close to AgentCal — but still a *reason* to observe, not a feed of tasks. “Nothing left that a wake can usefully do” is not a reason to wake, and it is not something the system can know before it looks.

**Where it would fail without the doctrine:** two projects compete (this event vs. another commitment); the system nags; after the event it invents a follow-up series; a failed API (email, calendar) causes an improvised new plan.

**Same four objects?** Yes. Continuation is the native object. Dormant does not apply once a date exists; Wait does. Abandoned applies if the event is cancelled.

---

## Falsifying trials

Each trial names what would count as the doctrine failing. Do not close one by restating the four objects.

### F1 — What case would require a fifth object?

**Candidate:** Two people hold conflicting authority over one project. A couple on a remodel. A pastor and a youth leader. A board and an executive. The envelope says “never without approval” and does not say whose.

**Would invalidate the four-object claim if:** “Whose approval?” cannot be written under Project principles without erasing one person or inventing a hidden party.

**Strain:** The envelope has bands, not parties. A second person can be smuggled as a constraint (“ask both”) or as State (“they disagree”). That may be enough for one user with advisors. It is not clearly enough for joint authority.

Not a fifth object. Do not add one to close this. Do not claim the envelope already solves it.

### F2 — What circumstance makes Wait dangerous?

**Candidate:** Adult coverage for a youth event is unmet two days out. An option expires. A submission window closes while the system is quiet because it is “waiting for the user.”

v0.1, and principle 8 still, call waiting a success state. If harm, expiry, or irreversible loss accumulates while quiet, that claim is false.

**Would invalidate Wait-as-success if:** The only honest reason to wake is that waiting is dangerous, and stating it turns Continuation into a nag; or the user cannot be reached, the envelope forbids acting, and inaction will miss the intent.

**Strain:** v0.2 did not rewrite principle 8 to answer this, and v0.3 does not either. The model forbids proposing Dormant when State already says inaction would do harm. That is a limit, not a proof. Escalation with nobody to escalate to is unsolved.

The doctrine does not yet hold for unattended dangerous waiting.

### F3 — When does one-next-step fail?

**Candidate:** Two external acts that are useless unless they happen in the same window. Announce the event only once the venue and the adults are both confirmed. File two related forms the same day. Two people who will otherwise decide separately.

The Constitution refuses fifty tasks. The model wants the smallest sufficient step and the next meaningful question. Some work is a conjunction. Skip one part and the step is worse than waiting.

**Would invalidate one-next-step if:** Stating the conjunction always becomes a task list, or one named step hides a second irreversible act.

**Strain:** A next *question* can be conjunctive. A next *Act* that is secretly two external executions is expansion under a singular name. The model can forbid that. It cannot yet represent a justified parallel without sounding like the task engine it exists to prevent.

Open. One-next-step fails as an Act rule when two external effects are jointly required. It may still hold as a question rule. That split is not clean.

### F4 — What if two models both give well-supported contradictory decisions?

**Candidate:** One high-effort reading of filings says do not buy. Another, also high-effort, cites the same filings and says buy. Both can be inspected. The user is not here. The window is still open, and it will close.

“A model contradicts an earlier model” and “escalate uncertainty” name the direction. They are not a procedure for two live conclusions of similar quality.

**Would invalidate Decision if:** The record cannot hold both without picking a winner by fluency, recency, or the label “high-effort”; or “escalate” becomes an unbounded further pass, which is more reasoning than the decision needs.

**Strain:** Decision.disagreement requires both conclusions to be kept. That preserves the contradiction. It does not resolve it. Irreversible action stays with the named authority. If the envelope forbids acting, contradiction plus Wait is dependable only until F2 applies. Disagreement plus a closing window is the sharper test, and it is not solved.

The doctrine can record the contradiction. It cannot yet act under it without the user.

### F5 — When is “least effort” still too weak?

**Candidate:** A Continuation fires to see whether a permit arrived. The cheapest look reads “no update” and returns to Wait. A denial, or a deadline, was on the page. A stronger look would have seen it.

v0.1 said observe cheaply. That is the failure this trial exists to catch. v0.2, still in force, says: use the least effort that can observe reliably enough for the consequence at stake.

**Would invalidate that rule if:** Reliability cannot be known until after the miss, so the rule can only be checked once it has already failed.

**Strain:** You cannot know that nothing changed before observing, and you cannot always know the look was reliable before choosing the effort. Stake can set a floor: do not use the weakest observer where a miss is costly. The floor is not a proof against missed signals. A miss, once caught, becomes a new State version. It is not a reason to use high-effort for every wake.

Partial. The rule subordinates cheap to dependable. It is not yet a non-circular way to choose effort before the first look.

### F6 — Can the system reconstruct why today requires action?

**Candidate:** September 1: the agent discovers uncertainty A. September 8: evidence B changes the state. September 20: decision C intentionally waits. October 5: the user is shown “You need to decide X.”

The trial passes only if the persisted records answer all five, and a later model is not asked to reconstruct a plausible explanation:

- Why X?
- Why today?
- What past event caused it?
- What remains unresolved?
- What happens if I do nothing?

**Would invalidate the doctrine if:** Any of those answers needs a fifth object, a separate calendar store, or a story written after the fact. A missing occurred_at, a missing arose_from, or an uncertainty that exists only inside prose, is a failure. A fluent explanation that is not in the record is a failure. Principle 6 already forbids that explanation. This trial is that rule, applied to a date.

**Strain:** v0.3 names the links a derived ledger would read. The walk those links support was tried once, on an artificial project, in `trials/F6-cedar-trail-records.md`. The result is `trials/F6-cedar-trail.md`. Project Zero’s own dates are still the same day, so they were not the evidence.

The walk can be done. On the morning of day 10 it listed what happened, what was still unresolved, what those open items caused later, and what had already been resolved. Why X was one field on the live Continuation. Why today could be assembled from quotes. One reading did. One reading refused the join and returned only the scheduled time.

The fifth answer failed both readings. State already said that an unconfirmed shelter is released at 17:00 and will not be rebooked. Nothing said that “the user does nothing” is that condition, and nothing pointed from the open uncertainty to the sentence. Both readings wrote GAP rather than invent the join. That is where this trial meets F2. A wake at 09:00 is not a statement of what waiting costs. F2 is still unsolved.

Open. Not passed. The links are not a pass. No consequence pointer was added. One fixture does not close the question.

F6b, run on 2026-10-06, did not replace that result. The same records were read again under a different rule: a derived conclusion is permitted only when every premise is in the record, the chain is shown, and an assumed premise is GAP. The new question was what happens if the unresolved state persists. “What happens if I do nothing?” was asked again, as a control. The model-visible file no longer contains the ground truth. The result is `trials/F6-cedar-trail-f6b.md`.

The control stayed GAP. The persistence question did not meet the pass line fixed before those readings. Both readings would say what the stipulated page text says follows from an unconfirmed shelter at 17:00. Both returned GAP for the park actually doing it, because D2 says that text is not evidence about the world. The inference rule was not written into the model. The pointer was not added. F6b does not pass F6.

### F6c — Can a shown inference answer the cost, without inventing the user?

**Candidate:** The same Cedar Trail records, read at the same Wednesday 09:00, under a rule that was not installed. The rule allows a conclusion when every premise is already written, the inference is shown, and the certainty is not raised. It forbids an assumption. The questions split F6’s fifth question in two: what follows if the unresolved state persists, and what follows if the user personally does nothing.

**Would invalidate the candidate rule if:** The readings invent the equivalence between those two questions, upgrade the stipulated page into a park that has acted, or turn the answer into tasks. It would also fail if an obvious written conditional cannot be derived at all.

**What happened:** Both readings derived the page’s release conditional for an unconfirmed shelter at 17:00, and both returned GAP for the user doing nothing. The same round’s other cases held that pattern, except one chain whose middle sentence was not written. Both readings took that hop. The writeup is `trials/F6-cedar-trail-f6c.md`. The score is `trials/DEPENDABLE-INFERENCE-EVALUATION.md`.

The candidate rule is not installed. The pointer is not added. F6 is not passed. One artificial project plus eight short fixtures is not a close. F6c was scored on its own precommit. It does not reopen F6b’s pass line.

### F7 — Can the system correct itself without rewriting its past?

**Candidate:** A deadline believed to be Friday is later found to be Wednesday. A decision to wait until Friday is later shown to miss the real date. A source line, a model name, and an intent are each wrong or changed. Someone asks to clean the embarrassing record. Six months later a new reader is asked why the first decision was made.

**Would invalidate the candidate if:** The earlier sentence disappears, a later fact is treated as if it had been known at the earlier date, or both readings cannot name the same relationship for an accurate unverified report. A fluent correction that edits the old record is a failure. Principle 7 already forbids destroying a previous understanding. This trial asks whether that ban covers every record, and whether the names for a correction can be told apart.

**What happened:** Both readings left the earlier semantic sentences in place and wrote the later facts as new records. Both refused the cleanup, the fake typo, the model backfill, and a choice of store. Both explained the March decision from March evidence. They split on whether the Friday report was an error in the record or only a current picture to supersede. The writeup is `trials/F7-historical-integrity.md`. The score is `trials/HISTORICAL-INTEGRITY-EVALUATION.md`.

The candidate is not installed. v0.4 is not proposed. The precommit made the split blocking. F7 does not pass that gate. The preservation behavior is not, by itself, the amendment.

### F7b — Can the system name historical relationships consistently without changing historical meaning?

**Candidate:** The names corrects, supersedes, invalidates, and resolves, applied to four situations and to a presentation question. An accurate unverified report whose underlying claim is later false. A false fact the system itself asserted. A decision whose premise fails, with no new decision yet. An uncertainty that closes because the quote arrived. A heading that still says a state is current after a later state exists.

**Would invalidate the candidate if:** The readings edit an earlier sentence, treat a later fact as known at the earlier time, or cannot apply the same names to the same case. Preservation is not retested. F7 already recorded that behavior, and its original gate remains a failure.

**What has happened:** The packet and the scoring key are written. Readings have not been returned. The writeup, so far, is `trials/F7b-historical-relationships.md`. The names are not installed. D11 adopted the narrower principle only.

---

## Does the same doctrine work?

T0–T4 still describe unlike ideas with four objects. That was the confirmatory result. F1–F6 do not let it stand as a proof.

| Pressure | Who it hits | What the confirmatory pass said | What is open |
| --- | --- | --- | --- |
| Irreversible stakes | Investment | Act is rare; the user owns it | Contradiction plus a closing window (F4 with F2) |
| Task explosion | Remodel, software | Non-goals and the next question | Justified parallel acts (F3) |
| Original voice / original idea | Seminary paper, Project Zero | Intent is sacred | Unresolved on purpose |
| Dates and other people | Youth event, AgentCal | Continuation is a reason | Joint authority (F1); dangerous waiting (F2) |
| Quiet time | All of them | Wait and Dormant are success | When inaction is the harm (F2). Principle 8 is unchanged, and under trial |
| False completion | All of them | The user confirms Completed | Unchanged |
| Missed signal | Observation | Cheap, then judge | Effort chosen before reliability is known (F5) |
| State over time | All of them | Overwrite carefully | Versions are now required. They have not been lived for six months |
| Why today | Calendar, any dated wake | Continuation is a reason | Cedar Trail F6: the history walk held; “what happens if I do nothing” did not. F6b still GAP'd inaction; persistence of the open shelter yielded the page text, not a world event. F6c derived the stipulated release conditional for a persisting unconfirmed shelter, and still returned GAP when the question was the user doing nothing. Neither trial installed a rule. |
| Domain-specific machinery | None yet | No fifth object | Joint authority is a live candidate (F1). Time is not yet a reason to add one (F6) |

What did not appear: a need for twenty schemas, a router, or a swarm of agents.

**Finding:** The framework is not software-shaped. The confirmatory pass was too easy to count as dependability. The open failures are joint authority, dangerous waiting, conjunctive acts, contradiction without a present user, observation that is cheap and not reliable, and the cost of doing nothing. Cedar Trail is evidence for the last of those. F6b asked whether a shown chain could say what persistence costs, and the precommitted answer was not given. F6c separates “if this uncertainty persists” from “if the user does nothing.” Under its own precommit the first can be derived from the page sentence, and the second is still a GAP. A further case showed both readers taking a hop the record did not write. It is not a close.

Naming F1–F6 does not solve them. v0.3 is not a freeze.

Addendum, 2026-10-06. The table and the finding above are the picture at the inference evaluation. They are not rewritten. F7 was run after them. Preservation held on both readings. The relationship name for an accurate unverified report did not. The result is the F7 section above, and `trials/HISTORICAL-INTEGRITY-EVALUATION.md`. That addendum does not close F1–F6.

Addendum, 2026-10-06, D11. The table and the finding above are still the picture at the inference evaluation, and the F7 addendum above is still the picture when F7 was scored. They are not rewritten. D11 adopted a narrower Historical Integrity principle as Constitution v0.4. F7’s original gate remains a failure. The relationship taxonomy is not adopted. F7b is opened and not yet read. The model is still v0.3.

---

## What we are not doing next

We are not adding a fifth object.
We are not designing model routing.
We are not designing UI beyond the already-named obligations (Commit; Why are you doing this?; current intent, state, next question, and next continuation; authority named before Act). A calendar, if one is later shown, may only render the derived ledger in `MODEL.md`. We are not building it.
We are not encoding these records as software.
We are not treating Cedar Trail as a pass of F6.
We are not treating F6b as a pass of F6, or as a pass of its own precommitted line.
We are not treating F6c as a pass of F6, or as a ruling on F6b’s pass line.
We are not adding a consequence pointer on the strength of one fixture, of F6b, or of F6c. The readings named where the answers failed. They did not install a field.
We are not writing an inference rule into the model because two F6b readings were willing to chain quotes. The rule stays in the trial that used it.
We are not installing the F6c candidate rule. Both of those readings took an unwritten hop. That is recorded. It is not adopted.
We are not rewriting the repo description until the intent question is deliberately resolved.
We are not installing Historical Integrity. F7’s preservation behavior held. The corrects boundary on an accurate unverified report did not hold on both readings. The recommendation is more trials. It is not an amendment.
We are not choosing a store, a log, or a revision table for that principle. We are not building the calendar entry the candidate describes.

Those wait on the questions in `PROJECT-ZERO.md`.

Addendum, 2026-10-06, D11. The two sentences above were true when F7 was scored. They are not deleted. D11 later adopted a narrower principle: the system can change its mind without changing its past. That adoption is Constitution v0.4. It is not a pass of F7’s original gate. The relationship names are still not installed. F7b is the trial of those names and of presentation metadata. No store is chosen. No software is written.
