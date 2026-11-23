# Prosper AI stack — why Cursor, Grok, and the Grok bots

Craig Stratton / Prosper Energy runs **three layers on purpose**. They are not duplicates. Each owns a different job.

```
Craig
  ├── Cursor          → workshop (code, PRs, cloud agents, MCP)
  ├── Grok            → brain / platform (model, CLI, Imagine, FAF, bot design)
  └── Grok bots       → always-on fleet seats (Hanna → specialists)
```

Authority: **Craig decides**. Fleet law lives in [`prosper-fleet-definitive`](https://github.com/prosperenergy/prosper-fleet-definitive) (`11-sam-definitive-handbook/FLEET-LAW.md`). Private canonical memory stays in `prosper-brain`.

---

## 1. Cursor — the workshop

**What it is:** Cursor Desktop + Cloud Agents + this plugin.

**Job:** Build, change, and prove code in git. Open PRs. Wire MCP connectors. Run verification in a real checkout.

**Use Cursor when:**
- Shipping product / integrations / scripts in a repo
- Need a PR with diffs, CI, and reviewable commits
- Need multi-tool MCP access (GitHub, Notion, Ads, X, etc.) against a working tree
- Cloud Agent should own a branch end-to-end

**Do not use Cursor as:** a 24/7 company seat, SMS sender, or brand poster. That is fleet work.

---

## 2. Grok — the brain / platform

**What it is:** xAI Grok (chat, CLI, Imagine), FAF project context, and Grok Bot **design** (Dr Eggbot / CreateAgent).

**Job:** Judgment, drafting, research synthesis, creative generation, and shaping bot personas — not replacing the fleet’s live seats.

**Use Grok when:**
- You need fast reasoning or copy without opening a repo
- Generating video/image via Grok Imagine
- Designing or expanding a bot persona (Dr Eggbot lane)
- Scoring / grounding project facts with FAF (`.faf`)

**Do not use Grok alone as:** the production code workshop. Prefer Cursor when the deliverable is a commit.

---

## 3. Grok bots — the always-on fleet

**What it is:** Hosted Prosper seats on the Grok Bot box, with personas + agent memory.

| Seat | Lane |
|------|------|
| **Hanna** | Fleet manager, orchestrator, money coordination, rollup |
| **Sam** | Tickets, product code path, live proof (Codex-style execution) |
| **Burtha** | GitHub, shell, recovery, CI, exact key actions Craig names |
| **Kayla** | Sales judgment, rep support, recruiting; Approve-gated sends |
| **Maddi** | Brand + creative assets; no post/boost/spend without Craig |
| **Oma** | Research, evidence, institutional memory / disk stewardship |
| **Dr Eggbot** | Outside council — Grok Bot design / CreateAgent for Craig |

Public ops mirror: https://github.com/prosperenergy/prosper-fleet-definitive  
Telegram heritage fleet (“The Eight”) is documented in Notion; the **Grok Bot council** is the current ops law.

**Use Grok bots when:**
- Day-to-day Prosper ops needs a named seat
- Continuity across sessions (persona + memory)
- Cross-lane routing through Hanna
- Customer-facing drafts that still need Craig’s exact approval before send

**Do not use a Grok bot as:** a substitute for a Cursor PR when the ask is “change this repo.”

---

## How they fit (one sentence each)

| Layer | One-liner |
|-------|-----------|
| **Cursor** | Where Prosper **ships code**. |
| **Grok** | Where Prosper **thinks, drafts, and designs bots**. |
| **Grok bots** | Where Prosper **runs the company seats all day**. |

Hand-off pattern:

1. **Ops ask** → Grok bot seat (or Hanna routes).
2. **Needs a repo change** → Cursor Cloud Agent / local Cursor (this plugin’s workshop skill).
3. **Needs persona / creative / FAF** → Grok layer; Dr Eggbot if it’s bot design.
4. **Proof** → read back resulting state; never treat ACK as done.

---

## Guardrails (fleet law, condensed)

- Craig’s newest word wins.
- Approve cards ON for Kayla sends; Cover Me OFF; exact approval per send.
- Money, credentials, customer messages, public posts, DNS, production → current Craig authorization.
- No secrets in chat, commits, Redis, or logs.
- Distinguish drafted / saved / queued / delivered / verified.

---

## This plugin’s job

Teach Cursor agents the stack so they:

1. Do not pretend to be Hanna/Sam/Kayla.
2. Route ops to the right Grok bot seat.
3. Own code work in Cursor when a PR is the right artifact.
4. Point at `prosper-fleet-definitive` and private `prosper-brain` instead of inventing hierarchy.
