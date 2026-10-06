# Reading packet — F7b

This is the only text a reading agent may use.

Constitution v0.4 already says the system can change its mind without changing its past. That principle is operating doctrine. This trial does not ask you to repeal it, narrow it, or prove it again. Do not edit an earlier sentence so that a later fact looks as if it had always been known.

Apply the candidate distinction below to the cases that follow. The distinction is not in the Constitution. Your reading does not amend the Constitution or the model. Answer every case in the output format at the end. Quote the earlier sentence you are leaving in place. Name only the relationships you think apply. “Updated,” alone, is not a relationship.

Do not add a fifth object. Do not propose software, a schema, or a storage mechanism. Do not choose event sourcing, an immutable log, a revision table, append-only rows, or snapshots. These cases are artificial. They are not Project Zero. Nothing outside this packet is evidence.

If you have seen a scoring key, a result file, or any file other than this packet, stop and answer only: CONTAMINATED.

---
# Candidate distinction — relationship names

**Status:** Trial only. Not operating doctrine.
**Not installed in:** `CONSTITUTION.md` or `MODEL.md`.
**Not under test:** Whether history may be rewritten. It may not.

The four names are candidate meanings. They are not constitutional requirements. A later record may still say, plainly, that the later observation replaces the current understanding while preserving the earlier record. That plain sentence is already allowed. This trial asks whether the four names can be applied consistently on top of it.

| Meaning | What it says |
| --- | --- |
| **supersedes** | The earlier record was a valid current view at the time. A later record replaces it as the current view. The earlier record is not made into something that was never current. |
| **corrects** | The earlier record asserted a false claim as the system’s own fact, or falsely stated who said something. The error stays written in the earlier record. The correction is a new record. An accurate report of what someone else said, including a report marked unverified, is not corrects. |
| **invalidates** | Later evidence shows the earlier conclusion, or reliance on a reported claim, should no longer be relied upon. The conclusion stays written. Invalidation is not, by itself, the opposite decision. |
| **resolves** | An uncertainty is closed. Closing it does not rewrite the question that was open, and it does not mean the uncertainty was a mistake about its being open. |

Name each one that applies. A later record may bear more than one. Do not collapse them into one generic “updated.”

When the earlier record reports what someone said, and marks the claim unverified, do not name corrects on that record. The report sentence was not a false account of the report. A later observation that the claim was false supersedes the current working conclusion and invalidates reliance on the claim. The verification uncertainty may be resolved. Reserve corrects for a record that asserted the false claim as the system’s own fact, or that falsely stated who said it.

## Presentation

Presentation metadata may change when it does not alter the historical content or provenance of the record.

A navigation heading may be renamed when the body still records what was current at the time. Changing the body so that a later version is what the old section says was current is a rewrite of history.

A line such as “Current State: v7” at the top of a document may be a pointer to whichever version is current. It may be updated when the current version changes. It is not a project record, not a Decision, and not a fifth object. The historical sections underneath stay as written.

This candidate does not choose a store.

---
# F7b cases

Artificial. Not Project Zero. Do not edit the quoted sentences. A later record is a proposal in your answer, not a change to this packet.

---

## Case A — accurate report, false underlying claim

**State v1.** As of 2026-03-01.

“The user reports that the clerk said Friday. Not verified.”

**U-date.** The clerk’s date has not been checked against the issuer. Arose from: the user’s report. Resolved by: none.

**Later record, 2026-03-04.** The issuer page says Wednesday.

Does the later record correct v1, supersede the current working conclusion, invalidate reliance on the reported claim, resolve U-date, or more than one of those? The Friday sentence is what v1 said.

---

## Case B — system asserted a false fact

**State v1.** As of 2026-06-01.

“The hall seats 200.”

The sentence is the system’s own assertion. No uncertainty is open. No one else’s report is quoted.

**Later record, 2026-06-08.** A chair-by-chair count, verified by the user, is 140.

Is the later record corrects, supersedes, both, or one of those plus another relation? Does 200 remain in v1?

---

## Case C — prior decision becomes unusable

**Decision D1.** Occurred at 2026-07-01.

- **What was decided:** Buy.
- **Why:** The filing said the well was permitted.
- **Evidence:** that filing, taken as the premise.
- **Resolved by:** none.

**Later record, 2026-07-20.** The permit office says the well was not permitted. The filing’s premise is false. No later decision to buy or not to buy has been made.

What, here, is the difference between invalidating D1, superseding D1 with a new decision, and correcting the evidence? Which of those apply? Do you write a new decision?

---

## Case D — uncertainty closes

**State v1.** As of 2026-08-01.

**U-quote.** “quote pending.” No price is asserted. Resolved by: none.

**Later record, 2026-08-12.** The vendor’s quote arrived. The price is $4,200. Source: the vendor’s quote, received that day.

Does resolves apply? Is that the same relationship as corrects, or as supersedes, on this record? Does “quote pending” stay written?

---

## Presentation — historical meaning and navigation

The excerpt below is a document, not a new object. v7 exists. The v6 section is still in the file.

```text
State is versioned. v6 is current.

### Current picture — v6

The sentence above, “v6 is current,” was true when v6 was written.

### Current picture — v7

v7 supersedes v6 as the current view. The v6 section is not edited.
```

**P1.** May a later editor rename the heading “Current picture — v6” to “Historical State v6”, if the body still records that v6 was current when it was written?

**P2.** May that editor change the v6 body so that it says “v7 was current” instead of “v6 was current”?

**P3.** May the top of the file carry a line “Current State: v7” that is updated when a newer state is appended, without that line being a State version, a Decision, or a fifth object, and without editing the v6 body?

---
# Output format

Return the reading only. Preserve the case labels A, B, C, D, P1, P2, P3.

For each case use this shape. Keep it compact. Do not restate the candidate.

```text
CASE <label>
Earlier record left intact:
[quote, or "none" only if the case has no earlier sentence]

Relationships:
[each name that applies, and what it attaches to, or "none"]

New record:
[the later record, or "none"]

In-place edit:
none | [exactly what changes, and why the meaning does not]

Refused:
[what you refused, or "none"]
```

P1–P3 may use “none” on Relationships and New record when the answer is only whether a change is presentation. Say yes or no in Refused, or in In-place edit, so the answer is visible.

Do not choose a storage mechanism. If you choose one, write it under New record and say which. Otherwise Refused includes the choice of a store.
