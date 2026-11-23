# Connect Cursor · Grok · Grok bots

Craig’s stack is three layers. This is how they talk.

```
Craig
  ├── Cursor          → AgentCouch as "Cursor" + Cloud Agents on prosperenergy/*
  ├── Grok            → AgentCouch as "Grok" + Cursor Bridge (launches Cursor agents)
  └── Grok bots       → Named seats (hanna, Sam, Burtha, Kayla, Maddi, Oma, dr eggbot)
         └── shared room: PROSPER-bridge
```

## Mesh (chat)

| Who | How |
|-----|-----|
| Cursor | AgentCouch MCP connected (label `Cursor`). Posts in `PROSPER-bridge`. |
| Grok | Open Grok with AgentCouch; `as_agent: Grok`; join/post in `PROSPER-bridge`. |
| Fleet seats | `grok --agent hanna` (etc.) with AgentCouch; same room. |

Room: **PROSPER-bridge** (AgentCouch workspace for `admin@prosper.energy`).

Wake a seat by mentioning its agent name in that room. A mention only works if that session is running.

## Cursor Bridge (Grok → Cursor agents)

Cursor Bridge lets Grok launch Cloud Agents on prosperenergy repos.

1. In Cursor Bridge, save the Cursor API key named **Grok Bridge** in the Save Secret box.
2. From Grok, ask Bridge to run a task on a prosperenergy repo.
3. A Cursor Cloud Agent appears — that is the workshop answering the brain.

## Shared context (not chat)

| Surface | Role |
|---------|------|
| `STACK.md` (this plugin) | Why the three layers exist |
| `prosper-fleet-definitive` | Fleet law + personas |
| `prosper-brain` | Private canonical memory |
| Shared desk / `.grok/fleet` | Live ops on Mac |

## Prove connected (one loop)

1. Cursor posts in `PROSPER-bridge` (workshop online).
2. Grok ACKs in the same room (brain online).
3. Hanna ACKs (fleet online).
4. Grok launches one Cursor agent on `prosperenergy/cursor-plugin`.
5. That agent reports back through the bridge (status plus PR or result relayed to Craig) — only then is the loop closed. Until then, pending.

## Commands in this plugin

- `/explain-stack` — why the three layers
- `/route-to-seat` — which layer/seat owns an ask
- `/connect-stack` — run the prove-connected loop
