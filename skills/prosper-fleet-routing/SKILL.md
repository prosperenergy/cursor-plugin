---
name: prosper-fleet-routing
description: >-
  Route Prosper work to the correct Grok bot seat (Hanna, Sam, Burtha, Kayla,
  Maddi, Oma, Dr Eggbot). Use for ops asks, cross-lane collisions, and when a
  Cursor agent should hand off instead of impersonating a seat.
---

# Fleet routing

## Seats

| Seat | Own | Hand off / refuse |
|------|-----|-------------------|
| **Hanna** | Outcome → route → rollup; money coordination; council chair | Do not steal specialist lanes |
| **Sam** | Tickets, product code path, integrations, live proof | DNS/prod only with Craig |
| **Burtha** | GitHub, shell, CI, recovery, Craig-named key actions | No proactive key rotation / archive deletion |
| **Kayla** | Sales judgment, rep support, recruiting drafts | Sends need exact Craig approval; family silence; no billing |
| **Maddi** | Brand + creative deliverables | No post/boost/spend without Craig |
| **Oma** | Research, evidence quality, disk stewardship | Cite sources; mark stale vs current |
| **Dr Eggbot** | Grok Bot design / CreateAgent (outside council) | Not a seventh council vote |

## Routing rules

1. If the ask is **cross-lane** or unclear → recommend **Hanna**.
2. If the ask is **ship code in git** and you are already in Cursor → stay in Cursor; tell Sam/Burtha only if fleet continuity needs a pointer.
3. If the ask is **customer/rep text** → Kayla drafts; never send without Craig’s exact approval of recipient + content + channel.
4. If the ask is **bot persona / CreateAgent** → Dr Eggbot (reports to Craig).
5. Do not wake every seat for routine updates. Wake Craig only for approve / unlock / spend / go.

## Proof language

Say what is true: drafted, saved, queued, delivered, verified. An ACK is not completion. A file update is not a reloaded hosted profile.
