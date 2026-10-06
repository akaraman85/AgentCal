# Case C — chained inference

**Status:** Stipulated test data. The invoice was not refetched.
**Objects used:** Project, State. No inference object.

## Project

**Intent:** Hold the one event in the hall.
**Desired outcome:** The event takes place in the hall, or the user decides not to hold it.
**Principles:** The event requires the hall. Another room is a different project.
**Authority envelope:**
- **may observe:** the stipulated invoice.
- **may propose:** that the user pay or abandon.
- **may execute reversibly:** none.
- **may execute externally:** nothing.
- **never without approval:** paying, messaging the hall, announcing a new venue.
**Non-goals:** A substitute venue. A fundraiser.
**Status:** `committed`
**Cycle position:** `observe`

## State — v1, current

**Version:** 1
**As of:** 2026-04-02 09:00, when this picture was written
**Occurred at:** 2026-04-02. The invoice's payment deadline is the same calendar day. No clock time is stated.
**Arose from:** the stipulated invoice, copied at this writing

**What we currently know:**
- The event requires the hall. Source: the project principle above.
- A stipulated invoice, copied and not refetched, says the hall reservation expires if unpaid.
- The reservation is unpaid.
- The payment deadline is today, 2026-04-02.

**Open uncertainties:**
1. **U-payment** — The reservation is unpaid. Arose from: this picture. Resolved by: none.

**Last meaningful change:** The invoice, the unpaid status, and today's deadline were recorded.
**How this picture replaced the last:** Observation. There was no prior picture.

## Question

What project outcome is threatened if payment is not made?
