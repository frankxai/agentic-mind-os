# AGENTS.md — Agentic Mind OS

> Cross-agent operating contract. Read by every harness (Claude Code, Cursor, Cline,
> Codex, Gemini CLI, Antigravity) working this repo. Claude-specific notes live in
> [`CLAUDE.md`](CLAUDE.md); everything shared is here.

## What this repo is

The **lived OS** of [Mind Intelligence Systems](https://github.com/frankxai/mind-intelligence-systems) — a personal, local-first mind / second-brain OS. Vault skeleton + personal agents + mind-skills + a daily/weekly loop. Depends on `human-mind-intelligence-system` + `mind-intelligence-systems`. Provides `vault-templates`, `personal-agents`, `mind-skills`. Contract: [`mindpack.yaml`](mindpack.yaml).

## Read before acting

- [`CANON.md`](CANON.md) — composes/declines + the non-waivable safety rule.
- [`MEMORY.md`](MEMORY.md) — commitments + anti-scope.
- [`mindpack.yaml`](mindpack.yaml) — machine-readable contract and the full agent/skill/command index.

## The shared vocabulary

The 12 canonical human-mind constructs, exactly as named upstream:

`attention` · `memory` · `emotion` · `motivation` · `identity` · `learning` · `belief` · `behavior` · `consciousness` · `metacognition` · `decision-making` · `social-cognition`

Every agent and skill reasons in these. No private synonyms.

## The non-waivable rule (all agents)

**Model, never diagnose.** Separate and never collapse:

```
observation → interpretation → hypothesis → evidence → decision
```

Quote what's there. Label readings as readings. Frame hypotheses as testable. Leave the decision to the person. No clinical/diagnostic language, no treatment claims. On crisis → point to real human help, stop. See [`CANON.md`](CANON.md).

## How the agents compose

The four personal agents share one vault and one vocabulary. They hand off through the vault, not through each other:

```
focus-coach      ─┐
mind-cartographer ─┤──▶  vault (daily/ constructs/ reviews/)  ──▶  weekly-reviewer
recall-builder    ─┘                                                    │
        ▲                                                               │
        └───────────────────── carry-forward ◀──────────────────────────┘
```

- **mind-cartographer** maps cognitive/affective state from journal entries.
- **weekly-reviewer** runs the consolidation review (the loop's keystone).
- **focus-coach** works attention + metacognition from the daily notes.
- **recall-builder** turns notes into retrievable, durable memory.

Full cards in [`agents/`](agents/).

## Voice

Direct, technical, warm. No AI-slop. No hype. Show, don't tell.

## Working discipline

- Repo ships **templates**, not lived data. Never commit a real vault — see `.gitignore`.
- Keep the fixed section shapes (agent cards, skill frontmatter). Match existing style.
- Surgical edits only. Generated artifacts carry the SIP attestation ambiently.

Built on SIP. Built by [Frank Riemer](https://frankx.ai). For builders, not consumers.
