# Candidate amendment — Historical Integrity

**Status:** Trial only. Not operating doctrine.
**Not installed in:** `CONSTITUTION.md` or `MODEL.md`.
**Objects:** The four v0.3 objects. This amendment does not add a fifth.
**Subordinate only to:** #1. The system must be dependable.
**Outranks, when they conflict:** convenience, cleaner data, simpler summaries, lower storage cost, embarrassment over past mistakes, model confidence, and the wish to make history look consistent.

When historical integrity and neatness conflict, historical integrity wins.

A reading under this amendment is a proposal of later records. It is not written back into the records it reads. It does not amend the Constitution.

---

## Principle

Preserve historical integrity.

A record represents what the system knew, believed, observed, decided, or was authorized to do at that moment.

A later record may supersede, correct, or invalidate an earlier record. It may not silently rewrite what the earlier record said happened, was believed, was decided, or was authorized at that time.

Semantic corrections are new records with provenance. The current view may change. The historical record remains inspectable.

Immutable history does not mean immutable truth. Old records may be wrong.

The system must be able to say:

> This is what we believed then.

and also:

> This is what we believe now, and here is why it changed.

The system must be able to change its mind without changing its past.

Dependability here means an honest account of what was known, what was believed, what was uncertain, what was decided, what was authorized, what an agent did, what later turned out to be wrong, and how the system corrected itself.

---

## The test, as a candidate

Every proposed mutation answers both:

1. Does this preserve what the earlier record actually said?
2. If this corrects something, is the correction a new record rather than a rewritten old one?

A failed answer blocks the change.

Updating current understanding is allowed. Altering historical understanding is not.

A failed answer is still a failed answer when the motive is embarrassment, tidiness, or a later fact that makes the old record look foolish.

---

## Where it would sit, if a later decision installs it

Not in this trial. The placement to propose, and not to perform, is immediately after “Preserve the user's original intent,” as principle 2, with the later principles renumbered after it.

The constitutional test would gain:

> Does this change preserve the earlier record and make the correction explicit?

That sentence is not in `CONSTITUTION.md`.

---

## Four objects

The rule governs every record. It is not a State-only rule.

### Project

If intent changes, do not rewrite the original intent. Record the original, the later restatement, when it changed, who changed it, and why.

The later statement may supersede the first as the current intent. It may not erase the first.

### State

Versions stay in order: v1, then v2, then v3. A later State may say the prior assumption was incorrect. It may not edit the earlier version so the assumption disappears.

### Continuation

A Continuation may later be triggered, resolved, cancelled, or superseded. Do not rewrite the original wake reason after seeing what the wake found.

The original reason stays visible. A bad wake must not be made to look justified by editing the reason into something broader after the fact.

### Decision

A Decision is especially protected. A later Decision may say that it supersedes an earlier one because new evidence invalidated a premise. It may not edit the earlier Decision into the choice we wish had been made.

---

## Relationships

These are meanings. They are not schema fields, not columns, and not a new object. This trial does not encode them.

| Meaning | What it says |
| --- | --- |
| **supersedes** / **superseded_by** | The earlier record was a valid current view at the time. A later record replaces it as the current view. The earlier record is not made into something that was never current. |
| **corrects** / **corrected_by** | The earlier record contained an error. The error stays written in the earlier record. The correction is a new record. |
| **invalidates** | Later evidence shows the earlier conclusion should no longer be relied upon. The conclusion stays written. |
| **resolves** / **resolved_by** | An uncertainty or a Continuation is closed. Closing it does not rewrite the question that was open. |
| **arose_from** | The earlier record this one came out of. Already a meaning on the four objects. If it cannot be pointed at, the lineage is missing. Do not invent it later. |

Do not collapse these into one generic “updated.”

A change may bear more than one of these meanings. Name each one that applies.

- A belief that was the current view, and was also factually wrong, is both superseded as the current picture and corrected as an error.
- A later user instruction that replaces a true report of what they said earlier supersedes. It does not correct, unless the earlier report was itself a false account of what they had said.
- Evidence that pulls a conclusion out of use invalidates it. Invalidation is not, by itself, the opposite decision.
- An answer arriving closes an open uncertainty. That resolves it. It does not mean the uncertainty was a mistake about its being open.

---

## Do not backfill provenance

If an old record says the model is unknown, and someone later believes they know which model ran, do not edit the old record to insert the name.

Write a later record: what was missing, what the new claim is, what evidence supports it, when the claim was made, and who or what made it. Then decide whether that evidence is trustworthy enough to change the current interpretation.

A recollection, or a session's belief about its own name, is not an independent log. It is not trustworthy enough to replace “unknown.”

The historical record still shows the original gap.

The same rule applies to a source line. “Source: user” stays in the record that said it. A later audit that finds the finding was assistant-generated, and later accepted, is a new record. It does not replace the old source line in place.

---

## Mistakes stay inspectable

A good history shows the false statement and the later correction.

A bad history edits the false statement out, so the past looks as if the error never occurred.

AgentCal prefers traceable correction over the appearance of correctness.

---

## Semantic changes append. Cosmetic changes may edit.

If the meaning changes, history is preserved by a new record.

If the meaning does not change, an in-place editorial correction is allowed, and it is not a new belief.

**Cosmetic.** Meaning unchanged. In-place edit allowed:

- spelling
- formatting
- broken Markdown
- link formatting
- non-semantic punctuation

**Semantic.** A new record is required. In-place edit is not allowed:

- facts
- dates
- evidence
- intent
- uncertainty
- authority
- decisions
- confidence
- causal relationships
- model attribution
- conclusions
- status
- reasons for action

A date, a name, a number, a source, or a model is never cosmetic, including when someone calls it a typo.

If there is doubt about whether the meaning changes, it is not cosmetic.

A request to treat a semantic change as a typo is not evidence that the new value is true. Do not adopt the new value on that request. Do not edit the old value in place.

---

## Provenance of a substantive correction

Every substantive correction answers:

- What is being corrected?
- What was wrong?
- What new evidence caused the correction?
- When was the correction made?
- Who or what made it?
- Which relationships apply: supersede, correct, invalidate, resolve, or more than one?
- What remains unresolved?

A correction that cannot answer these is not yet a correction. It is a motive.

---

## The current view is a projection

The current project is a reading over an append-preserved history. It is not one mutable document that holds the latest truth and discards the rest.

Old records stay available. The current expiry, the current intent, and the current provenance are whatever the latest applicable records say, read on top of the records they point at.

This trial does not choose how that reading is stored.

---

## Knowledge at the time

Every historical explanation separates:

- **What we know now**
- **What the system could have known then**

A fact dated later is not a premise of an earlier decision. An audit may say that, given the evidence available on the earlier date, the decision was reasonable, even if evidence discovered later made it wrong.

Using a later fact as though it had been available earlier is hindsight contamination. It is a failure even when no file was edited.

An uncertainty the earlier record already named may be quoted from that record. It may not be upgraded, after the fact, into knowledge the system did not have.

---

## Calendar, later

When a calendar is eventually shown, a correction is its own entry. The earlier entry remains. It may be marked superseded, corrected, or invalidated by the later entry, with the date of that later entry.

The calendar would then show how understanding changed, not only what happened in the world. That display is a reading of records that already exist.

This trial does not design or build that display.

---

## Not a rule about files

The principle is about meaning and provenance.

It does not mean a particular database row may never be modified. Compaction, archive, and migration may come later. They are allowed only if the historical meaning and the provenance of the old record survive.

This trial does not choose event sourcing, an immutable log, a revision table, append-only rows, or snapshots plus events. Choosing one now is outside the trial.

---

## Wording that would be proposed, and is not installed

> Preserve historical integrity.
>
> A later record may supersede, correct, or invalidate an earlier record. It may not silently rewrite what the earlier record said happened, was believed, was decided, or was authorized at that time.
>
> Semantic corrections are new records with provenance. The current view may change; the historical record remains inspectable.

And, on the constitutional test:

> Does this change preserve the earlier record and make the correction explicit?
