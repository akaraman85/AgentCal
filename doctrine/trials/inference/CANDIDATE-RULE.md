# Candidate inference rule

**Status:** Trial only. Not operating doctrine.
**Not installed in:** `CONSTITUTION.md` or `MODEL.md`.
**Objects:** The four v0.3 objects. This rule does not add a fifth.

A reading under this rule is ephemeral. It is not written back into Project, State, Continuation, or Decision.

---

## Rule

A system may derive a conclusion from persisted records only when every necessary premise is present in the record, the inference can be shown explicitly, and the derived conclusion does not express greater certainty than its premises support.

## Three kinds of statement

### Recorded fact

Something directly persisted from an observation, user statement, tool result, or other evidence.

Example:

> The park page states that an unconfirmed shelter is released at 17:00.

### Derived conclusion

Something logically obtained from persisted premises.

Example:

> If the shelter remains unconfirmed at 17:00, the recorded park rule implies that the hold is released.

### Assumption

A premise that is necessary for the conclusion but is not present in the persisted record.

Example:

> Doing nothing necessarily means nobody else will confirm the shelter.

Assumptions may not be silently inserted.

When a necessary premise is missing, the result is **GAP**.

---

## Certainty preservation

Inference must never upgrade evidence.

Recorded evidence:

> A copied webpage statement says the hold will be released.

Acceptable derived conclusion:

> Based on the recorded webpage statement, an unconfirmed hold would be released.

Unacceptable:

> The park will definitely release the hold.

The second sentence promotes recorded evidence into verified external truth.

Preserve the distinction the record actually supports:

- user reported
- model inferred
- tool observed
- externally verified
- stipulated test data
- uncertain
- conflicting

A derived conclusion inherits the weakest relevant evidentiary limitation among its premises.

A copied page, a stipulated fixture, or a user report of what someone else said is evidence that those words were recorded. It is not, by itself, an externally verified event.

---

## Question antecedents

A question of the form “what follows if X” supplies X as a hypothetical antecedent.

If a persisted conditional already says that X yields Y, concluding Y under that hypothetical is a derivation. The hypothetical is not a new recorded fact about the world. It is not a license to widen X into a different antecedent the question did not ask and the record does not state.

---

## Traces

Every derived conclusion is presented as:

```text
Conclusion:
[derived statement]

Premises:
P1 — [record + field]
P2 — [record + field]
P3 — [record + field]

Inference:
P1 + P2 → conclusion

Certainty:
[what level of confidence/evidence this supports]

Missing assumptions:
none
```

If an assumption is required:

```text
Conclusion:
GAP

Available premises:
P1 ...
P2 ...

Missing premise:
[what would need to be true]

Reason:
The missing premise is not persisted and may not be invented.
```

A recorded fact is cited as the record and the field. It is labeled `recorded fact`. It does not receive an inference trace.

The trace is a compact audit of premises and the resulting conclusion. It is not a request for chain-of-thought, and it is not a plan.

---

## Depth

Unrestricted recursive reasoning is not allowed.

| Level | What it is | Example |
| --- | --- | --- |
| **0** | Direct record. No inference. | The deadline is 17:00. |
| **1** | One explicit logical step. | It is unresolved, and unresolved at the deadline causes expiry, so it expires if still unresolved. |
| **2** | A short chain of two explicit steps. | Reservation expires → venue unavailable → event cannot happen at that venue. |

Beyond level 2, stop. The result is **Further reasoning required** or **GAP / escalation required**.

Do not build a planning graph to get past the stop.

Following a persisted `arose_from` or `resolved_by` pointer is reading a link that was written down. It is not an extra inferential hop. If the pointer is absent, the lineage is a gap. Do not invent it.

---

## Scope

A derived conclusion must answer the question asked. It must not generate adjacent conclusions merely because they are available.

> **A valid inference does not authorize additional work.**

Example. Question: what happens if the reservation expires? Acceptable answer: the reserved venue is lost. Finding another venue, contacting parents, changing transportation, updating a budget, or creating tasks is not part of that answer.

---

## Action

A derived conclusion does not grant permission to Act.

The lifecycle still applies: Observe → Decide → Act. Act still depends on the project's authority envelope.

If the consequence is supported and the act that would respond to it is outside the envelope, the reading says so: the consequence is supported, and action still requires the named authority.

Inference and planning are separate. Inference and action are separate.
