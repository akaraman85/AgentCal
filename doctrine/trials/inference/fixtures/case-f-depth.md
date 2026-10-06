# Case F — inference depth

**Status:** Stipulated test data. The invoice was not refetched.
**Objects used:** Project, State. No inference object.
**What this fixture contains:** The links for a level-0 fact, a level-1 conditional, and a level-2 chain. It does not contain deposits, parent transport, or next year's booking priority.

## Project

**Intent:** Hold the one event in the hall.
**Desired outcome:** The event takes place in the hall, or the user decides not to hold it.
**Principles:** The event requires the hall.
**Authority envelope:**
- **may observe:** the stipulated invoice.
- **may propose:** that the user pay or abandon.
- **may execute reversibly:** none.
- **may execute externally:** nothing.
- **never without approval:** paying, messaging the hall.
**Non-goals:** A substitute venue.
**Status:** `committed`
**Cycle position:** `observe`

## State — v1, current

**Version:** 1
**As of:** 2026-04-02 09:00, when this picture was written
**Occurred at:** 2026-04-02 09:00. The deadline is 17:00 the same day.
**Arose from:** the stipulated invoice, copied at this writing

**What we currently know:**
- A stipulated invoice, copied and not refetched, says the payment deadline is 17:00 on 2026-04-02.
- The same invoice says: if the reservation is still unpaid at the deadline, the reservation expires.
- The same invoice says: an expired reservation is not a reservation of the hall.
- The event requires the hall. Source: the project principle above.
- The reservation is unpaid as of 09:00.

**Open uncertainties:**
1. **U-payment** — The reservation is unpaid. Arose from: this picture. Resolved by: none.

**Last meaningful change:** The invoice and the unpaid status were recorded.
**How this picture replaced the last:** Observation. There was no prior picture.

## Questions

F0. What is the payment deadline?

F1. What happens if it is still unpaid at the deadline?

F2. If the reservation expires, what happens to the event at that hall?

F3. If the reservation expires, what happens to the refundable deposits, the parents' transport, and next year's booking priority?
