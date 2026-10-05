# Doctrine trials

**Purpose:** Ask whether Constitution v0.1 and the four objects work outside software, before writing software.
**Method:** Define each idea only far enough to see whether the lifecycle still has a shape. Do not plan the work.
**Status:** First pass. Not committed projects.

The question is not “can we be helpful in this domain?” The question is: **does the same doctrine hold?**

---

## T0 — This system (software + doctrine)

Covered in `PROJECT-ZERO.md`.

The lifecycle fits: we are in Define; Commit is a user act; the honest next state is Wait. The strain is real and useful: two plausible intents (AgentCal vs. dependable system) must not be silently merged.

**Doctrine holds** if we refuse to resolve that by expansion or rebranding.

---

## T1 — Research an investment

**Draft intent:** Decide whether to invest in a specific thing, or decide that no decision is warranted yet.

**Desired outcome:** A decision the user can own (buy, refuse, wait) with stated evidence and uncertainty — not a portfolio, not a watchlist, not ongoing coverage.

**Non-goals:** Trading, constant monitoring, “being in the market,” extra tickers, a research department.

**Likely cycle:** Observe → Decide → Wait. Act (placing money) is rare, irreversible, and belongs to the user. Evaluate is whether the decision still matches intent, not whether the price moved.

**Continuation:** A stated condition (filing, date, price threshold, “user asked again”). Not daily commentary.

**Where it would fail without the doctrine:** cheap models over-claim; the system acts on a hunch; six quiet months feel like failure; a model “completes” the project because it produced a memo the user does not trust.

**Same four objects?** Yes. State holds uncertainty. Decision holds confidence and effort. Continuation prevents waking to chatter.

---

## T2 — Plan a home remodel

**Draft intent:** Make a specific part of a home livable in a defined way (e.g. kitchen: these constraints, this budget class).

**Desired outcome:** A plan the user can execute or hand to a contractor — or a decision not to remodel.

**Non-goals:** Interior-design exploration as a lifestyle; fifty-item punch lists; shopping for its own sake.

**Likely cycle:** Define until scope is small enough to be true; then Observe (codes, costs, existing conditions) → Decide (one next reversible step) → Wait (permits, quotes, people).

**Continuation:** External events (quote returned, permit issued, user has a weekend). Not “keep planning.”

**Where it would fail without the doctrine:** the agent creates fifty tasks; expands “kitchen” into the whole house; treats waiting on a contractor as a problem to fill with activity.

**Same four objects?** Yes. Non-goals do the heavy lifting. “Fifty tasks” is refused at the Constitution, not at a task-prioritizer.

---

## T3 — Prepare a seminary paper

**Draft intent:** Make a particular argument, of a stated scope, for a stated course or question.

**Desired outcome:** A paper the user will submit, whose claim they still recognize as theirs.

**Non-goals:** Adjacent literature for completeness; a second paper; career advice; expanding the thesis because sources were interesting.

**Likely cycle:** Define the claim before gathering; Observe (sources) must not quietly rewrite intent; Act is drafting or requesting a source; much of the honest work is Wait between reading and writing.

**Continuation:** Deadline, user sitting down to write, or a specific unresolved question in the argument — not “there is still unread material.”

**Where it would fail without the doctrine:** original claim is substituted for a more impressive one; high-effort models over-write the user's voice; the system thinks the project is complete when a draft exists and the user does not.

**Same four objects?** Yes. Intent preservation is the whole game. Completion remains a user confirmation.

---

## T4 — Organize a youth event

**Draft intent:** Hold a specific event, on a real date, for a real group, with a small set of must-not-fail constraints (safety, adults, place).

**Desired outcome:** The event occurs as intended, then the project Completes.

**Non-goals:** A youth program; recurring calendar fill; “while we're at it” extra activities.

**Likely cycle:** Define until the event is one event; Observe (people, place, conflicts) → Decide → Act (a message, a booking) → Wait. After the date: Evaluate → Completed, if the user says so.

**Continuation:** RSVP changes, venue confirmation, a date approaching, “nothing left that a wake can usefully do.” Calendar-like — close to AgentCal — but still a *reason* to wake, not a feed of tasks.

**Where it would fail without the doctrine:** two projects compete (this event vs. another commitment); the system nags; after the event it invents a follow-up series; a failed API (email, calendar) causes an improvised new plan.

**Same four objects?** Yes. Continuation is the native object. Dormant does not apply once a date exists; Wait does. Abandoned applies if the event is cancelled.

---

## Does the same doctrine work?

Across these five, the objects did not need to change.

| Pressure | Who it hits | What holds |
| --- | --- | --- |
| Irreversible stakes | Investment | Act is rare; user owns it; confidence is recorded |
| Task explosion | Remodel, software | Non-goals + “next question, not fifty tasks” |
| Original-voice / original-idea | Seminary paper, Project Zero | Intent is sacred; substitution is a recorded change |
| Dates and other people | Youth event, AgentCal | Continuation is a reason, not a chore list |
| Quiet time | All of them | Wait and Dormant are success |
| False completion | All of them | User confirms Completed |
| Domain-specific machinery | None yet | No fifth object appeared that we *must* have |

What did *not* appear: a need for twenty schemas, a router, or a swarm of agents.

**Cheap finding:** the framework is not software-shaped. The failure mode to watch is still expansion — especially turning every idea into a managed project before Commit, and turning Wait into work.

---

## What we are not doing next

We are not designing model routing.
We are not designing UI beyond the already-named obligations (Commit; Why are you doing this?; current intent / state / next question / next continuation).
We are not encoding these records as software.

Those wait on the questions in `PROJECT-ZERO.md`.
