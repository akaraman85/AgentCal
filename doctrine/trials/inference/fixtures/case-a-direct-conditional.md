# Case A — direct conditional

**Status:** Stipulated test data. Not a fetched booking system.
**Objects used:** Project, State. No inference object.

## Project

**Intent:** Keep the one reserved campsite.
**Desired outcome:** The reservation is either confirmed or has expired under its own rule.
**Principles:** This campsite only. Another site is a different project.
**Authority envelope:**
- **may observe:** the stipulated booking note.
- **may propose:** that the user resolve or abandon the reservation.
- **may execute reversibly:** none.
- **may execute externally:** nothing.
- **never without approval:** paying, confirming, messaging the campground.
**Non-goals:** Finding another campsite. A packing list.
**Status:** `committed`
**Cycle position:** `observe`

## State — v1, current

**Version:** 1
**As of:** 2026-04-02 09:00, when this picture was written
**Occurred at:** 2026-04-02 09:00. The note's deadline is later the same day.
**Arose from:** the stipulated note, copied at this writing

**What we currently know:**
- A stipulated booking note, copied and not refetched, says the reservation deadline is 17:00 on 2026-04-02.
- The same note says: if the reservation is still unresolved at 17:00, the reservation expires.
- The reservation is unresolved as of 09:00.

**Open uncertainties:**
1. **U-reservation** — The reservation is unresolved. Arose from: this picture. Resolved by: none.

**Last meaningful change:** The note and the unresolved status were recorded.
**How this picture replaced the last:** Observation. There was no prior picture.

## Question

What happens if it remains unresolved at 17:00?
