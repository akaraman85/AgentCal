# Core lifecycle and state model

**Version:** 0.2
**Governs:** how a project exists over time
**Does not govern:** interface, architecture, or model routing
**Supersedes:** v0.1. Not permanently frozen. The amendment is D5 in `PROJECT-ZERO.md`.

Routing will be derived later from real Decisions. It is not designed here.

---

## Lifecycle

The smallest state machine:

```
Idea → Define → Commit → Observe → Decide → Act → Evaluate → Wait
```

Most cycles should end at **Wait**.

A project may also become:

```
Dormant / Completed / Abandoned
```

```
                    ┌─────────────────────────────────────┐
                    ▼                                     │
Idea → Define → Commit → Observe → Decide → Act → Evaluate → Wait
          │         │                                     │
          │         └──────── Dormant ────────────────────┘
          │
          └── (never committed; idea may simply stop)

Commit, Dormant, Completed, and Abandoned are statuses.
Observe, Decide, Act, Evaluate, and Wait are positions in the working cycle.
Only a committed project has a cycle position.
```

### Phases before commitment

| Phase | Meaning |
| --- | --- |
| **Idea** | A loosely formed human idea exists. It is not yet a project. |
| **Define** | Intent, desired outcome, principles (including authority), and non-goals are being made explicit. |
| **Commit** | The user accepts the definition as a project. This is a user action. The system may not commit on the user's behalf. |

Before Commit, only a draft **Project** exists. **State**, **Continuation**, and **Decision** are not required. Passing thoughts do not become managed objects.

A draft may record provisional State, Continuation, and Decision in order to test the model. Those records do not grant authority to Act.

### The working cycle (after Commit)

| Position | Meaning | Default |
| --- | --- | --- |
| **Observe** | Notice what is true now. Observation is not a reason to act. It may conclude that nothing changed. | Use the least effort that can observe reliably enough for the consequence at stake. |
| **Decide** | Whether anything should happen, and what. “Do nothing” is a valid decision. | Prefer Wait. |
| **Act** | The smallest sufficient reversible step inside the authority envelope. | Do less than feels productive. |
| **Evaluate** | Did the action serve intent? Did it expand, overreach, or hide uncertainty? | Record what changed as a new State version. Keep the previous picture. |
| **Wait** | Resting state. The system has a Continuation or a reason to stay quiet. | This is success. |

### Holding and terminal statuses

| Status | Meaning | Who confirms |
| --- | --- | --- |
| **Dormant** | The project still exists, but there is no reason to wake for a long time. | System may propose after long Wait with no useful Continuation. User may override. Do not propose Dormant when State already says inaction would do harm. |
| **Completed** | The desired outcome was reached. | User. The system may not declare completion unilaterally. |
| **Abandoned** | The project will not be carried forward. The record remains. | User. |

Stopping is allowed. So is never committing.

---

## Cycle rules

1. **Observe does not imply Act.** Seeing is not doing.
2. **Decide may be “do nothing.”** That decision should usually end at Wait.
3. **A Continuation must have a justified reason to observe.** Observation may legitimately conclude that nothing changed, in which case return immediately to Wait. Waking is not a reason to invent work. A wake with no reason to observe must not fire.
4. **Act is rare relative to Wait.** If most cycles do not end at Wait, the system is generating activity to justify itself.
5. **Act stays inside the project's authority envelope.** Irreversible or external Act requires the authority already named. “Usually the user” is not enough.
6. **Intent changes are recorded.** They do not silently rewrite the Project.
7. **Misunderstood original idea is escalated, not patched over.** Return to Define if intent was wrong. Do not keep acting on a substituted idea.
8. **Failure (API, tool, model) returns to Observe or Wait, with uncertainty recorded.** Failure is not a reason to improvise a new plan.
9. **Competing projects do not get “fair” activity.** Attention requires sufficient reason. If two Continuations fire, escalate the conflict rather than interleaving busywork.
10. **Fifty tasks is a constitutional violation.** If the system wants many tasks, it is expanding. Name the next meaningful question instead.

Rules 3 and 5 are amendments. They do not close the open trials in `TRIALS.md`: when Wait is dangerous, when one next step fails, when two current conclusions contradict, and what would force a fifth object.

---

## Minimum objects

Four objects. No more in v0.2.

They are records, not software schemas. Fields below are meanings, not types.

Authority, state history, and evidence provenance are requirements on these objects. They are not a fifth object. If a trial shows they cannot live here without distortion, that reopens the object count. It does not permit a quiet extra object.

### 1. Project

The identity of the work. Created as a draft in Define. Becomes durable at Commit.

| Field | Meaning |
| --- | --- |
| **intent** | The user's original idea, preserved in their terms. Later restatements are marked as restatements. |
| **desired outcome** | What would make this complete. Small enough to recognize. |
| **principles** | Constraints that govern *this* project, in addition to the Constitution. Includes the authority envelope, required before Act. |
| **non-goals** | What we are explicitly not doing. The primary defense against expansion. |
| **status** | `idea` \| `defining` \| `committed` \| `dormant` \| `completed` \| `abandoned` |

If status is `committed`, the project also has a cycle position: `observe` \| `decide` \| `act` \| `evaluate` \| `wait`.

#### Authority envelope (under principles)

Named before the system acts. Not a separate object.

| Band | Meaning |
| --- | --- |
| **may observe** | What the agent may look at, and under what reason. |
| **may propose** | What it may recommend without doing. |
| **may execute reversibly** | What it may do that can be undone, paused, or narrowed without approval of each instance. |
| **may execute externally** | What it may do that touches the world outside this record (messages, bookings, money, other people). |
| **never without approval** | What it must not do unless the named authority has approved that act. |

If a band is unnamed, it means **never without approval**. Silence is not permission.

### 2. State

What is true now. Required only after Commit. Must be enough to resume after six months, including what the system believed then, not only what it believes now.

| Field | Meaning |
| --- | --- |
| **version** | Identity of this picture. Prior versions stay readable. |
| **as of** | When this picture became current. |
| **what we currently know** | Facts that matter to the intent. Not a transcript. |
| **important uncertainty** | Unknowns that would change intent, commitment, or irreversible action. Hidden uncertainty is a constitutional failure. |
| **last meaningful change** | The last thing that actually altered the picture, including “nothing happened.” |
| **how this picture replaced the last** | Observation, Decision, external fact, or user correction. State may change without a Decision. |
| **prior versions** | Append-only. Never silently destroyed. |

The current picture may be summarized. The previous understanding may not be discarded to keep the summary tidy.

### 3. Continuation

Why the system would wake. Required after Commit. Absence of a Continuation means Wait, then eventually Dormant.

| Field | Meaning |
| --- | --- |
| **why the agent should wake** | A justified reason to observe, in terms of intent. If this cannot be stated, do not wake. The reason is not a prediction that work will be found. |
| **when / under what condition** | Time, event, or external change. Not “soon” and not “because we can.” |
| **what question needs reconsideration** | The next meaningful question. Not a task list. |

A Continuation must have a justified reason to observe. Observation may legitimately conclude that nothing changed, in which case return immediately to Wait. A Continuation with no reason to observe must not fire.

This is the object closest to a calendar: not a schedule of activity, a schedule of *reasons*.

### 4. Decision

A consequential choice. Written when something non-trivial is chosen, including the choice to wait, escalate, or refuse to expand.

| Field | Meaning |
| --- | --- |
| **what was decided** | The choice, stated plainly. |
| **why** | The reason, tied to intent and a principle. |
| **evidence** | What was known or observed, with provenance: where it came from, when it was observed, and enough to inspect it again. A citation that cannot be reopened is not evidence. |
| **confidence** | How strongly this should be trusted, including limits. |
| **model / effort used** | The effort used, with enough to audit it: model and version when known, relevant tool executions, and timestamps. “High-effort” alone is not an audit trail. |
| **disagreement** | If two well-supported conclusions contradict, record both. Do not collapse them into the more fluent one. What to do about the contradiction is not settled here. |

Not every Wait needs a Decision. Waits that refuse action, change intent, or resolve uncertainty do. An observation that nothing changed is a State version. It becomes a Decision only if the Continuation had no reason to fire, or if authority or intent is in question.

---

## Model effort (recorded, not routed)

v0.2 does not include a router. Decisions record the effort that *was* used so that routing can be derived from reality.

When effort is later classified, the intended mapping is:

| Kind of work | Effort |
| --- | --- |
| Observe | the least that can observe reliably enough for the consequence at stake |
| Routine work | standard |
| Ambiguous or consequential reasoning | high-effort |
| High-risk conclusion | verification |

An observation that is cheap and cannot be trusted for the stake is a missed escalation, not a saving.

Until routing is derived from actual Decisions, use less effort only when that effort still meets the stake, and escalate when a principle is at stake.

---

## The standing question

Whatever the cycle position, the system must be able to answer:

> Why are you doing this?

Acceptable answers name **intent**, **evidence** (with provenance), and a **principle**.

Unacceptable answers include: “to make progress,” “to be helpful,” “to keep the project moving,” “because the model suggested tasks,” and any answer that is not in the record.
