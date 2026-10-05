# Doctrine trials

**Purpose:** Ask whether Constitution v0.2 and the four objects work — and where they would fail.
**Method:** Two kinds of trial. Confirmatory trials ask whether the objects can describe unlike ideas. Falsifying trials try to invalidate the doctrine.
**Status:** First falsifying pass. Not committed projects. v0.1's confirmatory pass is retained as T0–T4.

Dependability requires falsifiability. “Can our four objects describe this?” is not enough. A trial that cannot fail cannot inform #1.

---

## Confirmatory trials (v0.1, retained)

These still matter. They are not sufficient.

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

**Same four objects?** Yes, as description. Authority (never place money without approval) and provenance (filings, prices, dates) are the load-bearing additions from v0.2.

### T2 — Plan a home remodel

**Draft intent:** Make a specific part of a home livable in a defined way (e.g. kitchen: these constraints, this budget class).

**Desired outcome:** A plan the user can execute or hand to a contractor — or a decision not to remodel.

**Non-goals:** Interior-design exploration as a lifestyle; fifty-item punch lists; shopping for its own sake.

**Likely cycle:** Define until scope is small enough to be true; then Observe (codes, costs, existing conditions) → Decide (one next reversible step) → Wait (permits, quotes, people).

**Continuation:** External events (quote returned, permit issued, user has a weekend). Not “keep planning.”

**Where it would fail without the doctrine:** the agent creates fifty tasks; expands “kitchen” into the whole house; treats waiting on a contractor as a problem to fill with activity.

**Same four objects?** Yes, as description. State versioning matters: a quote that replaces an earlier cost picture must not destroy the previous number.

### T3 — Prepare a seminary paper

**Draft intent:** Make a particular argument, of a stated scope, for a stated course or question.

**Desired outcome:** A paper the user will submit, whose claim they still recognize as theirs.

**Non-goals:** Adjacent literature for completeness; a second paper; career advice; expanding the thesis because sources were interesting.

**Likely cycle:** Define the claim before gathering; Observe (sources) must not quietly rewrite intent; Act is drafting or requesting a source; much of the honest work is Wait between reading and writing.

**Continuation:** Deadline, user sitting down to write, or a specific unresolved question in the argument — not “there is still unread material.”

**Where it would fail without the doctrine:** original claim is substituted for a more impressive one; high-effort models over-write the user's voice; the system thinks the project is complete when a draft exists and the user does not.

**Same four objects?** Yes, as description. Provenance on sources is the difference between a claim and a reconstructed story.

### T4 — Organize a youth event

**Draft intent:** Hold a specific event, on a real date, for a real group, with a small set of must-not-fail constraints (safety, adults, place).

**Desired outcome:** The event occurs as intended, then the project Completes.

**Non-goals:** A youth program; recurring calendar fill; “while we're at it” extra activities.

**Likely cycle:** Define until the event is one event; Observe (people, place, conflicts) → Decide → Act (a message, a booking) → Wait. After the date: Evaluate → Completed, if the user says so.

**Continuation:** RSVP changes, venue confirmation, a date approaching, or a justified reason to check that nothing has slipped. Calendar-like — close to AgentCal — but still a *reason* to observe, not a feed of tasks.

**Where it would fail without the doctrine:** two projects compete (this event vs. another commitment); the system nags; after the event it invents a follow-up series; a failed API (email, calendar) causes an improvised new plan.

**Same four objects?** Yes, as description. Waiting on a date is not the same as waiting when a safety constraint is unmet — see F2.

---

## Falsifying trials (v0.2)

Each trial names what would count as the doctrine failing. Open strain is recorded. Do not close a trial by restating the four objects.

### F1 — What case would require a fifth object?

**Candidate:** Two humans share a project and hold *conflicting* authority (a couple remodeling; a board and an executive; a pastor and a youth leader). The envelope is “never without approval,” but approval *by whom*, when they disagree, is not a principle of one Project. It is a relation among authorities.

**What would invalidate the four-object claim:** If “whose approval?” cannot be recorded without distortion — if putting it in Project.principles either erases one person or invents a hidden Actor/Party object.

**Present strain:** The envelope has bands, not parties. A second person is currently smuggled as a constraint (“ask Alex and Sam”) or as State (“Sam disagrees”). That may be enough for a single user plus advisors. It is not clearly enough for joint authority.

**Not yet a fifth object.** It is a live candidate. Do not add Actor/Party unless a committed project cannot name approval without it. Do not pretend the envelope already solves joint authority.

### F2 — What circumstance makes Wait dangerous?

**Candidate:** A youth event whose adult-coverage constraint is unmet two days before the date; or an investment whose option expires; or a paper whose submission window closes while the system is “waiting for the user to sit down.”

v0.1 treated Wait as success. If harm, expiry, or irreversible loss can accumulate while quiet, that default is wrong.

**What would invalidate the Wait doctrine:** If the only honest Continuation is “wake because waiting is dangerous,” and that reason cannot be stated without turning Continuation into a nagging schedule; or if naming the risk still leaves no permitted Act when the user is unavailable.

**Present strain:** v0.2 requires Continuation to name **risk of waiting**, and forbids proposing Dormant when waiting is dangerous. That is a patch, not a proof. The remaining hole: the user is gone, the envelope says never-without-approval, and inaction will fail the intent. Escalation with no one to escalate to is not solved.

**Doctrine does not yet hold for unattended dangerous waiting.** It holds only when someone who can approve is reachable, or when the envelope already permits a named reversible Act.

### F3 — When does one-next-step fail?

**Candidate:** Two filings, bookings, or messages that are useless unless they happen in the same window (announce the event only once the venue is confirmed *and* adults are confirmed; submit two related forms the same day; a coordinated conversation with two people who will otherwise decide separately).

The Constitution refuses fifty tasks. The model prefers “the smallest sufficient reversible step” and “the next meaningful question.” Some work is not a sequence of next steps. It is a conjunction: skip one conjunct and the step is worse than waiting.

**What would invalidate one-next-step:** If stating the conjunction always explodes into a task list, or if compressing it into one “step” hides a second irreversible Act inside the first.

**Present strain:** A next *question* can be conjunctive (“are venue and adults both confirmed?”). A next *Act* that is secretly two external executions is expansion under a singular name. The model can forbid that. It cannot yet *represent* a justified parallel without sounding like the fifty-task engine it exists to prevent.

**Open.** One-next-step fails as an Act rule when two external effects are jointly required. It may still hold as a question rule. That split is not yet clean.

### F4 — Two models, both well-supported, contradict each other

**Candidate:** Investment research. Model A, high-effort, cites filings and concludes do not buy. Model B, also high-effort, cites the same filings plus a different reading of risk and concludes buy. Both leave inspectable evidence. The user is not present. The window is not yet closed, but it will close.

v0.1 said “a model contradicts an earlier model” and “escalate uncertainty.” Escalation is the right direction. It is not a procedure for two live, current, contrary conclusions of similar quality.

**What would invalidate the Decision object:** If the record cannot hold both conclusions without picking a winner by fluency, recency, or effort-label; or if “escalate” becomes an unbounded third reasoning pass that is itself more reasoning than the decision needs.

**Present strain:** v0.2 adds Decision.**disagreement**. That preserves the contradiction. It does not resolve it. Resolution remains a user act when stakes are irreversible. If the envelope forbids acting, contradiction plus Wait is dependable — until F2 applies (the window is closing). The collision of F4 and F2 is the sharper test: disagreement plus dangerous waiting.

**Doctrine holds for recording contradiction. It does not yet hold for acting under contradiction without the user.**

### F5 — Cheap observation misses the escalation signal

**Candidate:** A Continuation fires to check whether a permit arrived, using the least effort available. The cheap pass reads a portal as “no update.” A later high-effort pass would have seen a denial hidden behind a tab, or a deadline in a PDF. The system returns to Wait, correctly under “nothing changed,” incorrectly on the facts.

v0.1 said observe cheaply. That is the failure mode this trial exists to catch.

**What would invalidate the effort rule:** If “least effort that can observe reliably enough for the consequence” cannot be stated before observing — because reliability is only known after the miss.

**Present strain:** This is the Continuation problem in another form. You cannot know nothing-changed before observing, and you cannot always know the observation was reliable before choosing effort. v0.2 makes cheap subordinate to dependable and requires provenance so a later pass can inspect again. That is better. It does not give a non-circular rule for choosing effort *before* the first look.

**Partial hold.** Stake can set a floor (irreversible → do not use the weakest observer). The floor is not a proof against missed signals. Missed-signal cases should be recorded as State versions and as Decision disagreement when caught — not silently patched by always using high-effort.

---

## Does the same doctrine work?

Confirmatory trials T0–T4 still describe unlike ideas with four objects. Falsifying trials F1–F5 do not let us keep that conclusion unmodified.

| Pressure | Who it hits | What holds | What is open |
| --- | --- | --- | --- |
| Irreversible stakes | Investment | Act is rare; user owns it | Contradiction + closing window (F4 ∩ F2) |
| Task explosion | Remodel, software | Non-goals + next question | Justified parallel Acts (F3) |
| Original-voice / original-idea | Seminary paper, Project Zero | Intent is sacred | Unchanged |
| Dates and other people | Youth event, AgentCal | Continuation is a reason | Joint authority (F1); dangerous wait (F2) |
| Quiet time | All of them | Wait when inaction is justified | Wait when inaction harms (F2) |
| False completion | All of them | User confirms Completed | Unchanged |
| Missed signal | Observation generally | Cheap is subordinate to dependable | Effort chosen before reliability is known (F5) |
| State over time | All of them | Versions must remain readable | Not yet lived through six months |
| Domain-specific machinery | None yet | No fifth object added | Joint authority is a live candidate (F1) |

What did *not* appear: a need for twenty schemas, a router, or a swarm of agents.

**Finding:** the framework is not software-shaped. The confirmatory pass was too easy. The failure modes to watch are now specific: joint authority, dangerous waiting, conjunctive Acts, contradiction without a present user, and observations that are cheap but not reliable.

Do not treat F1–F5 as solved by having named them.

---

## What we are not doing next

We are not adding a fifth object.
We are not designing model routing.
We are not designing UI beyond the already-named obligations (Commit; Why are you doing this?; current intent / state / next question / next continuation; authority named before Act).
We are not encoding these records as software.
We are not rewriting the repo description until the intent question is deliberately resolved.

Those wait on the questions in `PROJECT-ZERO.md`.
