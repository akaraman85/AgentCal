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

**Strain:** v0.2 does not rewrite principle 8 to answer this. It forbids proposing Dormant when State already says inaction would do harm. That is a limit, not a proof. Escalation with nobody to escalate to is unsolved.

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

v0.1 said observe cheaply. That is the failure this trial exists to catch. v0.2 says: use the least effort that can observe reliably enough for the consequence at stake.

**Would invalidate that rule if:** Reliability cannot be known until after the miss, so the rule can only be checked once it has already failed.

**Strain:** You cannot know that nothing changed before observing, and you cannot always know the look was reliable before choosing the effort. Stake can set a floor: do not use the weakest observer where a miss is costly. The floor is not a proof against missed signals. A miss, once caught, becomes a new State version. It is not a reason to use high-effort for every wake.

Partial. The rule subordinates cheap to dependable. It is not yet a non-circular way to choose effort before the first look.

---

## Does the same doctrine work?

T0–T4 still describe unlike ideas with four objects. That was the confirmatory result. F1–F5 do not let it stand as a proof.

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
| Domain-specific machinery | None yet | No fifth object | Joint authority is a live candidate (F1) |

What did not appear: a need for twenty schemas, a router, or a swarm of agents.

**Finding:** The framework is not software-shaped. The confirmatory pass was too easy to count as dependability. The open failures are joint authority, dangerous waiting, conjunctive acts, contradiction without a present user, and observation that is cheap and not reliable.

Naming F1–F5 does not solve them. v0.2 is not a freeze.

---

## What we are not doing next

We are not adding a fifth object.
We are not designing model routing.
We are not designing UI beyond the already-named obligations (Commit; Why are you doing this?; current intent, state, next question, and next continuation; authority named before Act).
We are not encoding these records as software.
We are not rewriting the repo description until the intent question is deliberately resolved.

Those wait on the questions in `PROJECT-ZERO.md`.
