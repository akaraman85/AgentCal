# Core lifecycle and state model

**Version:** 0.1
**Governs:** how a project exists over time
**Does not govern:** interface, architecture, or model routing

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
| **Define** | Intent, desired outcome, principles, and non-goals are being made explicit. |
| **Commit** | The user accepts the definition as a project. This is a user action. The system may not commit on the user's behalf. |

Before Commit, only a draft **Project** exists. **State**, **Continuation**, and **Decision** are not required. Passing thoughts do not become managed objects.

### The working cycle (after Commit)

| Position | Meaning | Default |
| --- | --- | --- |
| **Observe** | Notice what is true now. Cheap. Observation is not a reason to act. | Use the least effort that can see. |
| **Decide** | Whether anything should happen, and what. “Do nothing” is a valid decision. | Prefer Wait. |
| **Act** | The smallest sufficient reversible step. | Do less than feels productive. |
| **Evaluate** | Did the action serve intent? Did it expand, overreach, or hide uncertainty? | Record what changed. |
| **Wait** | Resting state. The system has a Continuation or a reason to stay quiet. | This is success. |

### Holding and terminal statuses

| Status | Meaning | Who confirms |
| --- | --- | --- |
| **Dormant** | The project still exists, but there is no reason to wake for a long time. | System may propose after long Wait with no useful Continuation. User may override. |
| **Completed** | The desired outcome was reached. | User. The system may not declare completion unilaterally. |
| **Abandoned** | The project will not be carried forward. The record remains. | User. |

Stopping is allowed. So is never committing.

---

## Cycle rules

1. **Observe does not imply Act.** Seeing is not doing.
2. **Decide may be “do nothing.”** That decision should usually end at Wait.
3. **A wake with nothing useful to do returns to Wait.** Waking is not a reason to invent work.
4. **Act is rare relative to Wait.** If most cycles do not end at Wait, the system is generating activity to justify itself.
5. **Irreversible Act requires higher confidence, clearer evidence, and usually the user.**
6. **Intent changes are recorded.** They do not silently rewrite the Project.
7. **Misunderstood original idea is escalated, not patched over.** Return to Define if intent was wrong. Do not keep acting on a substituted idea.
8. **Failure (API, tool, model) returns to Observe or Wait, with uncertainty recorded.** Failure is not a reason to improvise a new plan.
9. **Competing projects do not get “fair” activity.** Attention requires sufficient reason. If two Continuations fire, escalate the conflict rather than interleaving busywork.
10. **Fifty tasks is a constitutional violation.** If the system wants many tasks, it is expanding. Name the next meaningful question instead.

---

## Minimum objects

Four objects. No more in v0.1.

They are records, not software schemas. Fields below are meanings, not types.

### 1. Project

The identity of the work. Created as a draft in Define. Becomes durable at Commit.

| Field | Meaning |
| --- | --- |
| **intent** | The user's original idea, preserved in their terms. Later restatements are marked as restatements. |
| **desired outcome** | What would make this complete. Small enough to recognize. |
| **principles** | Constraints that govern *this* project, in addition to the Constitution. |
| **non-goals** | What we are explicitly not doing. The primary defense against expansion. |
| **status** | `idea` \| `defining` \| `committed` \| `dormant` \| `completed` \| `abandoned` |

If status is `committed`, the project also has a cycle position: `observe` \| `decide` \| `act` \| `evaluate` \| `wait`.

### 2. State

What is true now. Required only after Commit. Must be enough to resume after six months.

| Field | Meaning |
| --- | --- |
| **what we currently know** | Facts that matter to the intent. Not a transcript. |
| **important uncertainty** | Unknowns that would change intent, commitment, or irreversible action. Hidden uncertainty is a constitutional failure. |
| **last meaningful change** | The last thing that actually altered the picture, including “nothing happened.” |

State is overwritten carefully: new knowledge updates it; history of *decisions* lives in Decision records, not here.

### 3. Continuation

Why the system would wake. Required after Commit. Absence of a Continuation means Wait, then eventually Dormant.

| Field | Meaning |
| --- | --- |
| **why the agent should wake** | The reason, in terms of intent. If this cannot be stated, do not wake. |
| **when / under what condition** | Time, event, or external change. Not “soon” and not “because we can.” |
| **what question needs reconsideration** | The next meaningful question. Not a task list. |

A Continuation whose answer would be “there is nothing useful to do” must not fire. If it fires anyway, return to Wait and record that the Continuation was wrong.

This is the object closest to a calendar: not a schedule of activity, a schedule of *reasons*.

### 4. Decision

A consequential choice. Written when something non-trivial is chosen, including the choice to wait, escalate, or refuse to expand.

| Field | Meaning |
| --- | --- |
| **what was decided** | The choice, stated plainly. |
| **why** | The reason, tied to intent and a principle. |
| **evidence** | What was known or observed. |
| **confidence** | How strongly this should be trusted, including limits. |
| **model / effort used** | What class of effort made the decision. This is how routing will later be derived. |

Not every Wait needs a Decision. Waits that refuse action, change intent, or resolve uncertainty do.

---

## Model effort (recorded, not routed)

v0.1 does not include a router. Decisions record the effort that *was* used so that routing can be derived from reality.

When effort is later classified, the intended mapping is:

| Kind of work | Effort |
| --- | --- |
| Observe | cheap |
| Routine work | standard |
| Ambiguous or consequential reasoning | high-effort |
| High-risk conclusion | verification |

Until that is derived from actual Decisions, default to less effort, and escalate when a principle is at stake.

---

## The standing question

Whatever the cycle position, the system must be able to answer:

> Why are you doing this?

Acceptable answers name **intent**, **evidence**, and a **principle**.

Unacceptable answers include: “to make progress,” “to be helpful,” “to keep the project moving,” “because the model suggested tasks.”
