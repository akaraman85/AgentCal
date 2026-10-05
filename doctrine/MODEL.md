# Core lifecycle and state model

**Version:** 0.3
**Governs:** how a project exists over time
**Does not govern:** interface, architecture, or model routing
**Supersedes:** v0.2. Not permanently frozen. The amendment is D6 in `PROJECT-ZERO.md`.

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
5. **Act stays inside the project's authority envelope.** Irreversible or external Act requires the authority already named. “Usually the user” is not enough. Reversible does not mean authorized. The system does not write its own permission into the reversible band.
6. **Intent changes are recorded.** They do not silently rewrite the Project.
7. **Misunderstood original idea is escalated, not patched over.** Return to Define if intent was wrong. Do not keep acting on a substituted idea.
8. **Failure (API, tool, model) returns to Observe or Wait, with uncertainty recorded.** Failure is not a reason to improvise a new plan.
9. **Competing projects do not get “fair” activity.** Attention requires sufficient reason. If two Continuations fire, escalate the conflict rather than interleaving busywork.
10. **Fifty tasks is a constitutional violation.** If the system wants many tasks, it is expanding. Name the next meaningful question instead.

The observe/act split, the envelope, and the rule that reversible does not mean authorized are amendments. They do not close the open trials in `TRIALS.md`. F6 asks whether the temporal links below can say why today requires action. Naming the links does not pass it.

---

## Minimum objects

Four objects. No more in v0.3.

They are records, not software schemas. Fields below are meanings, not types.

Authority, state history, evidence provenance, and the temporal links are requirements on these objects. They are not a fifth object. If a trial shows they cannot live here without distortion, that reopens the object count. It does not permit a quiet extra object.

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
| **may execute reversibly** | Acts a named authority has explicitly allowed, and that can be undone, paused, or narrowed without approval of each instance. |
| **may execute externally** | What it may do that touches the world outside this record (messages, bookings, money, other people). |
| **never without approval** | What it must not do unless the named authority has approved that act. |

If a band is unnamed, it means **never without approval**. Silence is not permission.

**Reversible does not mean authorized.** The reversible band lists only acts a named authority has explicitly allowed. The system does not fill that band by noticing that an act can be undone. None, unless explicitly authorized, is the default. An empty band means no reversible execution. A later explicit authorization may name a class of act. That authorization is recorded as a Decision. It is not inferred from status `defining`, from a review that did not grant it, or from the fact that the act can be reverted.

### 2. State

What is true now. Required only after Commit. Must be enough to resume after six months, including what the system believed then, not only what it believes now.

| Field | Meaning |
| --- | --- |
| **version** | Identity of this picture. Prior versions stay readable. |
| **as of** | When this picture became current. When it was written, not when the world changed. |
| **occurred_at** | When the facts in this picture happened, if that time is known. Distinct from **as of**. Do not collapse them when they differ. If they are the same moment, say so. |
| **what we currently know** | Facts that matter to the intent. Not a transcript. |
| **important uncertainty** | The open uncertainties. Each one is named on its own, so a later record can point at it. What is unknown, and that it is still open. A paragraph that only implies an unknown does not count. Each may say what it **arose_from**. Each stays open until **resolved_by** names a later record. Hidden uncertainty is a constitutional failure. |
| **last meaningful change** | The last thing that actually altered the picture, including “nothing happened.” |
| **how this picture replaced the last** | Observation, Decision, external fact, or user correction. The kind of change. State may change without a Decision. |
| **arose_from** | Which earlier record this picture came out of. The kind of change is the field above. This is the pointer. If it cannot be pointed at, the lineage is missing. Do not invent it later. |
| **prior versions** | Append-only. Never silently destroyed. |

The current picture may be summarized. The previous understanding may not be discarded to keep the summary tidy.

### 3. Continuation

Why the system would wake. Required after Commit. Absence of a Continuation means Wait, then eventually Dormant.

| Field | Meaning |
| --- | --- |
| **why the agent should wake** | A justified reason to observe, in terms of intent. If this cannot be stated, do not wake. The reason is not a prediction that work will be found. |
| **when / under what condition** | Time, event, or external change. Not “soon” and not “because we can.” This is the condition, not the moment it fired. |
| **what question needs reconsideration** | The next meaningful question. Not a task list. |
| **created_at** | When this Continuation was recorded. |
| **triggered_at** | When the condition became true and the wake happened, or should have. Empty until then. |
| **resolved_at** | When the wake was closed because the question was taken up. Closing the wake does not by itself close the uncertainties it named. |
| **cancelled_at** | When the Continuation was withdrawn without being answered. At most one of **resolved_at** or **cancelled_at**. |
| **arose_from** | The State, open uncertainty, Decision, or event that made this wake necessary. |
| **resolved_by** | The later Decision or State version that closed the wake. Empty while the Continuation is live. |

A Continuation must have a justified reason to observe. Observation may legitimately conclude that nothing changed, in which case return immediately to Wait. A Continuation with no reason to observe must not fire.

This is the object closest to a calendar: not a schedule of activity, a schedule of *reasons*. The times above say when the reason was recorded, when it fired, and when it ended. They do not by themselves say why today requires action. That reading is the derived ledger below. F6 is the trial. It is open.

### 4. Decision

A consequential choice. Written when something non-trivial is chosen, including the choice to wait, escalate, or refuse to expand.

| Field | Meaning |
| --- | --- |
| **what was decided** | The choice, stated plainly. |
| **why** | The reason, tied to intent and a principle. |
| **occurred_at** | When the choice was made, if known. Not when a later reader inferred it, and not when a later revision corrected the writeup. |
| **evidence** | What was known or observed, with provenance: where it came from, when it was observed, and enough to inspect it again. A citation that cannot be reopened is not evidence. Who produced a finding and who later incorporated it are different facts. Do not collapse them. |
| **confidence** | How strongly this should be trusted, including limits. |
| **model / effort used** | The effort used, with enough to audit it: model and version when known, relevant tool executions, and timestamps. “High-effort” alone is not an audit trail. If the persisted record does not show which model ran, the model is `unknown`. An inserted name is worse than a gap. |
| **arose_from** | The earlier record this choice came out of. Absent means the lineage was not recorded. That is a gap, not a license to invent one. |
| **resolved_by** | The later record that superseded or closed this decision, if one has. Empty while the choice stands. |
| **disagreement** | If two well-supported conclusions contradict, record both. Do not collapse them into the more fluent one. What to do about the contradiction is not settled here. |

Not every Wait needs a Decision. Waits that refuse action, change intent, or resolve uncertainty do. An observation that nothing changed is a State version. It becomes a Decision only if the Continuation had no reason to fire, or if authority or intent is in question.

---

## Derived temporal ledger

Not a fifth object. Not a calendar database. A calendar, if one is shown, is a reading of records that already exist.

The reading has to be able to walk:

> what happened → what remained unresolved → what that unresolved thing caused later → how and when it was resolved

| From the records | What the reading uses |
| --- | --- |
| What happened | State or Decision **occurred_at**, and the fact recorded there |
| What remained unresolved | An open uncertainty with no **resolved_by** |
| What it caused later | A later record whose **arose_from** points back |
| How and when it was resolved | **resolved_by**. When is that record's **occurred_at**, or the Continuation's **resolved_at** or **cancelled_at** |

The reading renders recorded causal history. It does not invent a past the records do not contain. A missing link is shown as a gap. A model is not asked, afterward, to supply a plausible cause.

These names are meanings, not columns and not a schema. If a trial shows the walk cannot be done without a fifth object, that reopens the object count. It does not permit a quiet calendar store. F6 is that trial. It is open.

---

## Model effort (recorded, not routed)

v0.3 does not include a router. Decisions record the effort that *was* used so that routing can be derived from reality.

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
