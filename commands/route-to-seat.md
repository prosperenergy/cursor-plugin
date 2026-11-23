---
name: route-to-seat
description: Given a Prosper ask, pick Cursor vs Grok vs the right Grok bot seat.
---

# Route to seat

1. Read `STACK.md` and `skills/prosper-fleet-routing/SKILL.md`.
2. Classify the ask: workshop (Cursor), brain/design (Grok / Dr Eggbot), or fleet seat.
3. Return exactly:
   - **Layer:** Cursor | Grok | Grok bots
   - **Seat / owner:** (if bots) Hanna | Sam | Burtha | Kayla | Maddi | Oma | Dr Eggbot
   - **Why:** one sentence
   - **Next action:** what to do now
   - **Approval needed?** yes/no — and for what
4. If cross-lane, route via Hanna.
5. Never authorize sends, spends, DNS, or production without Craig’s current word.
