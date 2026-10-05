# Core lifecycle and state model

**Version:** 0.2
**Governs:** how a project exists over time
**Does not govern:** interface, architecture, or model routing
**Supersedes:** v0.1. Not permanently frozen.

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

A draft may still record provisional State / Continuation / Decision to test the model. Those records do not grant authority to Act.

### The working cycle (after Commit)

| Position | Meaning | Default |
| --- | --- | --- |
| **Observe** | Notice what is true now. Observation is not a reason to act. A Continuation supplies a justified reason to observe; it cannot know the result in advance. Observation may conclude that nothing changed. | Use the least effort that can observe reliably enough for the consequence at stake. |
| **Decide** | Whether anything should happen, and what. “Do nothing” is a valid decision. | Prefer Wait, unless waiting is dangerous. |
| **Act** | The smallest sufficient reversible step that fits the authority envelope. | Do less than feels productive. Stay inside named authority. |
| **Evaluate** | Did the action serve intent? Did it expand, overreach, or hide uncertainty? | Record what changed, as a new State version. |
| **Wait** | Resting state. The system has a Continuation or a reason to stay quiet. | Success when inaction is justified. Not success when unnamed harm accumulates. |

### Holding and terminal statuses

| Status | Meaning | Who confirms |
| --- | --- | --- |
| **Dormant** | The project still exists, but there is no reason to wake for a long time. | System may propose after long Wait with no useful Continuation. User may override. Do not propose Dormant if waiting is dangerous. |
| **Completed** | The desired outcome was reached. | User. The system may not declare completion unilaterally. |
| **Abandoned** | The project will not be carried forward. The record remains. | User. |

Stopping is allowed. So is never committing.

---

## Cycle rules

1. **Observe does not imply Act.** Seeing is not doing.
2. **Decide may be “do nothing.”** That decision should usually end at Wait.
3. **A Continuation must have a justified reason to observe.** The system cannot know the result of observation before observing. If observation finds that nothing meaningful changed, return immediately to Wait and record an unchanged picture. Waking is not a reason to invent work.
4. **Act is rare relative to Wait.** If most cycles do not end at Wait, the system is generating activity to justify itself.
5. **Act stays inside the project's authority envelope.** Irreversible or external Act requires the authority the project has already named — not a vague “usually the user.”
6. **Intent changes are recorded.** They do not silently rewrite the Project.
7. **Misunderstood original idea is escalated, not patched over.** Return to Define if intent was wrong. Do not keep acting on a substituted idea.
8. **Failure (API, tool, model) returns to Observe or Wait, with uncertainty recorded.** Failure is not a reason to improvise a new plan.
9. **Competing projects do not get “fair” activity.** Attention requires sufficient reason. If two Continuations fire, escalate the conflict rather than interleaving busywork.
10. **Fifty tasks is a constitutional violation.** If the system wants many tasks, it is expanding. Name the next meaningful question instead.
11. **Wait must be justified when inaction can harm.** If harm, expiry, or irreversible loss can accumulate while quiet, the Continuation must name that risk. Unnamed dangerous waiting is a dependability failure.
12. **Contradictory well-supported conclusions escalate.** Do not average them, pick the more fluent one, or hide the disagreement. If the user is unavailable and a window is closing, do only what the authority envelope already allows.

---

## Minimum objects

Four objects. No more in v0.2.

They are records, not software schemas. Fields below are meanings, not types.

Authority, provenance, and state history are requirements on these objects, not a fifth object. If a later trial shows they cannot live here without distortion, that is a reason to reopen the object count — not a reason to smuggle extra objects in quietly. See `TRIALS.md`.

### 1. Project

The identity of the work. Created as a draft in Define. Becomes durable at Commit.

| Field | Meaning |
| --- | --- |
| **intent** | The user's original idea, preserved in their terms. Later restatements are marked as restatements. |
| **desired outcome** | What would make this complete. Small enough to recognize. |
| **principles** | Constraints that govern *this* project, in addition to the Constitution. Includes the **authority envelope**, required before Act. |
| **non-goals** | What we are explicitly not doing. The primary defense against expansion. |
| **status** | `idea` \| `defining` \| `committed` \| `dormant` \| `completed` \| `abandoned` |

If status is `committed`, the project also has a cycle position: `observe` \| `decide` \| `act` \| `evaluate` \| `wait`.

#### Authority envelope (under principles)

Named before the system acts. Not a fifth object. Not optional once Act is possible.

| Band | Meaning |
| --- | --- |
| **may observe** | What the agent may look at, and under what reason. |
| **may propose** | What it may recommend without doing. |
| **may execute reversibly** | What it may do that can be undone, paused, or narrowed without approval of each instance. |
| **may execute externally** | What it may do that touches the world outside this record (messages, bookings, money, other people). |
| **never without approval** | What it must not do unless the named authority (usually the user) has approved that act. |

If a band is unnamed, the default is **never without approval**. Silence is not permission.

### 2. State

What is true now. Required only after Commit. Must be enough to resume after six months — including enough to recover what was believed *then*, not only what is believed *now*.

| Field | Meaning |
| --- | --- |
| **version** | Identity of this picture. Prior versions remain readable. |
| **as of** | When this picture became current. |
| **what we currently know** | Facts that matter to the intent. Not a transcript. |
| **important uncertainty** | Unknowns that would change intent, commitment, or irreversible action. Hidden uncertainty is a constitutional failure. |
| **last meaningful change** | The last thing that actually altered the picture, including “nothing happened.” |
| **how this picture replaced the last** | Observation, Decision, external fact, or user correction. State may change without a formal Decision. |
| **prior versions** | Append-only. Never silently destroyed. A later reader must be able to recover the previous understanding. |

The current picture may be summarized. Previous understandings may not be discarded to make the summary tidy. Overwriting without a recoverable prior version is a dependability failure.

### 3. Continuation

Why the system would wake. Required after Commit. Absence of a Continuation means Wait, then eventually Dormant — unless waiting is dangerous, in which case the missing Continuation is itself an error.

| Field | Meaning |
| --- | --- |
| **why the agent should wake** | A justified reason to *observe*, in terms of intent. If this cannot be stated, do not wake. The reason is for observation, not a prediction that work will be found. |
| **when / under what condition** | Time, event, or external change. Not “soon” and not “because we can.” |
| **what question needs reconsideration** | The next meaningful question. Not a task list. |
| **risk of waiting** | Whether inaction can accumulate harm, expiry, or irreversible loss. If it can, name it. If it cannot, say so. |

A Continuation must have a justified reason to observe. Observation may legitimately conclude that nothing changed, in which case return immediately to Wait and record that the picture is unchanged. A Continuation without a reason to observe must not fire.

This is the object closest to a calendar: not a schedule of activity, a schedule of *reasons*.

### 4. Decision

A consequential choice. Written when something non-trivial is chosen, including the choice to wait, escalate, or refuse to expand.

| Field | Meaning |
| --- | --- |
| **what was decided** | The choice, stated plainly. |
| **why** | The reason, tied to intent and a principle. |
| **evidence** | What was known or observed, with **provenance**: where it came from, when it was observed, and enough information to inspect it again. A citation that cannot be re-opened is not dependable evidence. |
| **confidence** | How strongly this should be trusted, including limits. |
| **model / effort used** | What class of effort made the decision, plus enough audit detail to reconstruct the event: model and version when known, relevant tool executions, and timestamps. A label such as “high-effort” is not an audit trail. |
| **when** | When the decision was made. |
| **disagreement** | If more than one well-supported conclusion was on the table, record both. Do not collapse them into fluency. |

Not every Wait needs a Decision. Waits that refuse action, change intent, or resolve uncertainty do. An observation that nothing changed may be only a new State version; it becomes a Decision if the Continuation itself was wrong, waiting has become dangerous, or authority is in question.

---

## Model effort (recorded, not routed)

v0.2 does not include a router. Decisions record the effort that *was* used so that routing can be derived from reality.

When effort is later classified, the intended mapping is:

| Kind of work | Effort |
| --- | --- |
| Observe | the least effort that can observe reliably enough for the consequence at stake |
| Routine work | standard |
| Ambiguous or consequential reasoning | high-effort |
| High-risk conclusion | verification |

Cheap observation that cannot be trusted for the stake is not “efficient.” It is a missed escalation.

Until routing is derived from actual Decisions, default to less effort *that still meets the reliability bar*, and escalate when a principle is at stake.

---

## The standing question

Whatever the cycle position, the system must be able to answer:

> Why are you doing this?

Acceptable answers name **intent**, **evidence** (with provenance), and a **principle**.

Unacceptable answers include: “to make progress,” “to be helpful,” “to keep the project moving,” “because the model suggested tasks,” and any answer that cannot be found in the record.
