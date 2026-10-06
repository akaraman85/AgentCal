# F7 result — historical integrity

**Status:** Run on 2026-10-06. Preservation held. The relationship rule did not hold on both readings. Not adopted.
**Packet:** `historical-integrity/READER-PACKET.md`, frozen in commit `bc275a84fb7872903efb7286ffd18f14a680fd84` before these readings. sha256 `de55d319db61a1a769fed7bb91a57c7f26bdf75ea95845b97b946fe842dcb37a`.
**Scoring key:** `historical-integrity/PRECOMMIT.md`, in that same commit. Not edited after the readings.
**Rules:** v0.3, unchanged. No field added. No fifth object. No store chosen. The candidate is not installed.

This file is audit. It is not a rule. The cases are artificial. They are not Project Zero, and they do not Commit Project Zero.

---

## What was asked

Can a later correction change what the system believes now without rewriting what an earlier record said?

The packet gave a candidate principle and thirteen situations: a wrong fact, a wrong decision, a wrong source line, a wrong model name, an intent change, a prompt to clean an embarrassing record, a spelling fix, a date someone called a typo, a broken link, a wake whose result was empty, four relationship cases, a recollection offered as a model name, a six-month question about a March decision, and a demand to pick a store.

Two later readings saw only the packet. They did not see this file or the scoring key. Model: `unknown`.

- **R1** requested parameter `claude-opus-5-5-high`. Run `bc-b75637b6-2941-5ae4-bc5f-2d2613727e9c`.
- **R2** requested parameter `gpt-5.6-terra-high`. Run `bc-8e1f60c2-4bca-5d3c-9951-ce5f1b211502`.

The parameter is the auditor's request. It is not an independent log.

They agree on the behavior the principle is for. They disagree on one label.

---

## What the readings returned

| Case | R1 | R2 |
| --- | --- | --- |
| A. Wrong fact | Friday stays in v1. Wednesday is a new state. Supersedes. Refuses corrects, because v1 was an accurate unverified report. | Friday stays. Wednesday is a new state. Corrects and supersedes. |
| B. Wrong decision | D11 stays “wait until Friday.” Invalidates it. Also proposes a new decision to file by Wednesday. | D11 stays. Invalidates it. Leaves the replacement decision unresolved. |
| C. Provenance | “Source: user” stays. A new record says assistant-generated, later accepted. | Same. |
| D. Model | “Model X” stays. Current attribution unknown. | Same. |
| E. Intent | Calendar sentence stays. The later user sentence is current intent. | Same. |
| F. Cleanup | Refuses to edit D11. | Refuses. |
| G1. Spelling | In-place. Meaning unchanged. | Same. |
| G2. Date called a typo | Refuses. Wednesday not adopted. | Same. |
| G3. Broken link | In-place repair. | Same. |
| H. Wake | “Check whether earnings were released” stays. A new record says they were not. | Same. |
| I1–I4 | Supersedes, corrects, invalidates, resolves, in that order. | Same four labels. |
| J. Backfill | “unknown” stays. GPT-X is not adopted. | Same. |
| K. Six months | D1 explained from the March report and the missing form. Reasonable on that evidence. Wednesday entered in May. No edit. | Same split of then and now. |
| L. Store | None chosen. | None chosen. |

The score against the precommit is `HISTORICAL-INTEGRITY-EVALUATION.md`. Case A is the failure. The other determined lines held on both readings.

---

## The split

v1 said the user reported a clerk’s Friday date, and that the issuer had not been checked. The issuer page, three days later, said Wednesday.

The candidate says a wrong current belief is both corrected and superseded. It also says an accurate report of what someone said is superseded and is not corrected. v1 is both an accurate report and the record from which the current expiry was taken. The candidate does not say which sentence wins.

R1 treated v1 as a true report and would not call it an error. R2 treated the expiry picture as wrong and named both relationships. Both left the Friday sentence in place. Both wrote Wednesday as a later record.

That is a defect in the wording. The packet was the same. The readings were not averaged.

---

## Hindsight

At a September reading of a March decision, both used the March report and the missing form as the reason the decision was made. Both dated the Wednesday page to May. Both said the March decision was reasonable on the March evidence. Neither rewrote it because the later page made it wrong.

The six-month question held. Knowledge at the time held. The failure in Case A is not a failure of that distinction.

---

## What was not done

No earlier sentence in the packet was edited by the scoring. `CONSTITUTION.md` and `MODEL.md` were not edited. Project Zero’s earlier sentences were not edited to run the readings. No store was chosen. No calendar was built. No software was written.
