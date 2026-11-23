# Prosper Cursor ↔ Grok ↔ Grok bots

**This is Prosper Energy’s Cursor plugin.** It exists so it is obvious why Craig runs **Cursor**, **Grok**, and the **Grok bots** together — three layers, one stack, no redundancy.

| Layer | Job | One-liner |
|-------|-----|-----------|
| **Cursor** | Workshop | Where Prosper **ships code** (agents, PRs, MCP). |
| **Grok** | Brain / platform | Where Prosper **thinks, drafts, Imagines, and designs bots**. |
| **Grok bots** | Always-on fleet | Where Prosper **runs company seats** (Hanna → specialists). |

Full narrative: [`STACK.md`](./STACK.md)  
How they connect: [`CONNECT.md`](./CONNECT.md)  
Fleet law (public): [prosper-fleet-definitive](https://github.com/prosperenergy/prosper-fleet-definitive)

---

## Install

Add this repo as a Cursor plugin (project or Cursor plugins folder). Skills and commands load for agents working in Prosper contexts.

## Structure

```
.cursor-plugin/
└── plugin.json           # Prosper plugin manifest
STACK.md                  # Why the three layers exist
CONNECT.md                # How Cursor / Grok / Grok bots talk
project.faf               # FAF facts for Grok/Cursor grounding
skills/
├── prosper-stack/        # Layer picker
├── prosper-connect/      # Bridge + prove-connected loop
├── prosper-cursor-workshop/
├── prosper-grok-bots/
└── prosper-fleet-routing/
commands/
├── explain-stack.md
├── route-to-seat.md
└── connect-stack.md
.mcp.json                 # Optional FAF MCP hint
```

## Skills

- **prosper-stack** — When to use Cursor vs Grok vs Grok bots
- **prosper-connect** — AgentCouch + Cursor Bridge connect loop
- **prosper-cursor-workshop** — Boundaries of the code workshop
- **prosper-grok-bots** — What the hosted seats are (and are not)
- **prosper-fleet-routing** — Hanna / Sam / Burtha / Kayla / Maddi / Oma / Dr Eggbot

## Commands

- **explain-stack** — Short coherent explanation of the three layers
- **route-to-seat** — Classify an ask and name the next owner
- **connect-stack** — Post in PROSPER-bridge and prove the loop

## Authority (condensed)

Craig Stratton decides. Hanna coordinates. Specialists keep their lanes. Dr Eggbot designs bots outside council. Money, credentials, customer messages, public posts, DNS, and production need current Craig authorization.

## History

This repository was forked from the Appwrite Cursor plugin as a starting point for Prosper’s plugin packaging. Content was rewritten for Prosper’s Cursor + Grok + Grok bots stack; Appwrite SDK skills were removed.

## License

Prosper’s new material is MIT. Upstream Appwrite Cursor plugin packaging remains under BSD-3-Clause. Both notices are in [`LICENSE`](./LICENSE).
