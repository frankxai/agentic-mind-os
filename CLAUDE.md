# CLAUDE.md — Agentic Mind OS

> Operating contract for Claude Code (and any agent) working inside this repo.

## What this repo is

The **lived OS** layer of [Mind Intelligence Systems](https://github.com/frankxai/mind-intelligence-systems). A personal, local-first mind / second-brain OS: a vault skeleton (`vault-templates/`), personal agents (`agents/`), mind-skills (`skills/`), and a daily/weekly loop. It depends on `human-mind-intelligence-system` + `mind-intelligence-systems` and provides `vault-templates`, `personal-agents`, `mind-skills`. Contract: [`mindpack.yaml`](mindpack.yaml).

## Read first

1. [`CANON.md`](CANON.md) — what this repo composes and declines. The non-waivable safety rule.
2. [`MEMORY.md`](MEMORY.md) — commitments and anti-scope.
3. [`mindpack.yaml`](mindpack.yaml) — the machine-readable contract.

## The 12 constructs (use exactly these names)

`attention` · `memory` · `emotion` · `motivation` · `identity` · `learning` · `belief` · `behavior` · `consciousness` · `metacognition` · `decision-making` · `social-cognition`

Sourced from `mind-intelligence-systems/models/human-mind/`. Never invent a synonym. If the model needs to change, it changes upstream in canon, not here.

## The non-waivable rule

**Model, never diagnose.** Keep these five steps separate and never collapse them:

```
observation → interpretation → hypothesis → evidence → decision
```

- Observation quotes/counts what the user wrote.
- Interpretation is labeled as a reading, never asserted as fact.
- Hypothesis is testable, never a verdict.
- The decision belongs to the person.

No clinical/diagnostic language (`disorder`, `diagnosis`, `symptom of`, `you have X`). No therapy or treatment claims. On any sign of crisis: point to real human help, stop the loop. Full rule in [`CANON.md`](CANON.md).

## Voice

Direct, technical, warm. No AI-slop ("delve", "dive into", "it's worth noting", "unlock", "harness the power", "seamless", "elevate your", "supercharge"). No hype. Show, don't tell.

## Working here

- This repo ships **templates**, not a real vault. A user's lived vault is private and lives outside the repo (`~/mind-vault`). Never commit a real vault — `.gitignore` guards this.
- Match the existing structure: agent cards have a fixed section shape (Role / When it activates / Reads / Writes / How it works / Non-clinical guardrail). Skills are `SKILL.md` with frontmatter (`name`, `description`).
- Surgical edits. Touch only what the task needs.
- Generated artifacts carry the SIP attestation ambiently.

Built on SIP. Built by [Frank Riemer](https://frankx.ai). For builders, not consumers.
