# Agentic Mind OS

[![Built on SIP](https://img.shields.io/badge/Built%20on-SIP-c9b6ff.svg)](https://github.com/frankxai/Starlight-Intelligence-System)
[![License: MIT](https://img.shields.io/badge/License-MIT-f4c97a.svg)](LICENSE)
[![Layer: Lived OS](https://img.shields.io/badge/layer-lived%20OS-green.svg)](https://github.com/frankxai/mind-intelligence-systems)

A personal, local-first mind OS you live in daily — a vault, a fleet of agents, and a weekly review loop, built on the canonical human-mind model.

This is the **lived layer** of the [Mind Intelligence Systems](https://github.com/frankxai/mind-intelligence-systems) ecosystem. Not a product you install for one job, not a research runtime — the thing one person runs every day. A vault you write into. Agents that read what you wrote and help you see it. A review loop that turns scattered notes into something you actually remember.

---

## Where this sits

Agentic Mind OS depends on two repos upstream and inherits everything from them:

- **[mind-intelligence-systems](https://github.com/frankxai/mind-intelligence-systems)** — the canon. Naming doctrine, the human-mind model, the mesh that defines who depends on whom. When an agent here asks you about your *attention* or *belief* state, the vocabulary comes from there.
- **[human-mind-intelligence-system](https://github.com/frankxai/human-mind-intelligence-system)** — the cognitive schemas and ontology. The engineered System that turns the model into something agents can reason over.

This repo's contract with the mesh lives in [`mindpack.yaml`](mindpack.yaml). It **provides** three things to the ecosystem: vault-templates, personal-agents, and mind-skills.

```
mind-intelligence-systems        (canon: names · models · mesh)
        │
        ▼
human-mind-intelligence-system   (cognitive: schemas · ontology)
        │
        ▼
agentic-mind-os  ◀── you are here (lived OS: vault · agents · review loop)
        │
        ▼
starlight-mind-os-pro            (premium distribution)
```

---

## Quick map

| Folder | What it is |
|---|---|
| [`vault-templates/`](vault-templates/) | The Obsidian-style local-first vault skeleton you copy and live in |
| [`agents/`](agents/) | Personal agent cards — cartographer, reviewer, focus coach, recall builder |
| [`skills/`](skills/) | Mind-skills your agent runtime auto-activates |
| [`commands/`](commands/) | Command specs — `/review-week`, `/map-mind` |
| [`mindpack.yaml`](mindpack.yaml) | The manifest the mesh references |
| [`CANON.md`](CANON.md) | What this repo composes and what it declines |
| [`MEMORY.md`](MEMORY.md) | Durable commitments, scope boundaries, what it composes from |

---

## The 12 constructs

Everything in the vault and every agent here speaks the same vocabulary — the 12 modules of the canonical human-mind model:

`attention` · `memory` · `emotion` · `motivation` · `identity` · `learning` · `belief` · `behavior` · `consciousness` · `metacognition` · `decision-making` · `social-cognition`

One vault note per construct lives in [`vault-templates/constructs/`](vault-templates/constructs/). They are the shared lenses every agent uses to read what you write.

---

## Quick start

```bash
# 1. Clone
git clone https://github.com/frankxai/agentic-mind-os.git
cd agentic-mind-os

# 2. Copy the vault skeleton somewhere you live (not inside this repo)
cp -r vault-templates ~/mind-vault
#    Open ~/mind-vault as an Obsidian vault, or just edit the .md files.

# 3. Install the agents + skills into your agent runtime
#    Claude Code:  copy agents/ and skills/ into .claude/ (or ~/.claude/)
#    Cursor/Cline/Codex: point your harness at agents/ and skills/
cp -r agents skills ~/.claude/
```

That's it. Write a daily note. Run `/map-mind` when you want to see the shape of what you've written. Run `/review-week` on Sunday.

See [`vault-templates/README.md`](vault-templates/README.md) for the vault setup in full.

---

## The loop

**Daily** — open `daily/YYYY-MM-DD.md`, write what's on your mind, what you're attending to, what moved you, what you decided. Don't structure it. Just capture.

**Weekly** — run `/review-week`. The `weekly-reviewer` agent reads the week's daily notes, consolidates them against the 12 constructs, and writes a `reviews/YYYY-Www.md` note: what recurred, what you learned, what to carry forward. This is the consolidation step — the thing that turns capture into memory.

```
capture (daily) ──▶ map (/map-mind) ──▶ consolidate (/review-week) ──▶ carry forward
   ▲                                                                        │
   └────────────────────────────────────────────────────────────────────────┘
```

---

## The safety principle

This OS **models** a mind. It never **diagnoses** one.

Every agent here keeps a hard line between five steps, and never collapses them:

```
observation → interpretation → hypothesis → evidence → decision
```

An agent may say *"you mentioned feeling scattered in three notes this week"* (observation). It may offer *"that reads like attention load"* (interpretation, flagged as such). It will never say *"you have an attention disorder"* — that is clinical, diagnostic, and out of scope. No `-therapy`, no `-diagnosis`, no `-disorder`. If a note suggests crisis or clinical need, agents point to real human help, not a hypothesis. See [`CANON.md`](CANON.md) and each agent card's guardrail section.

---

## The Mind Intelligence ecosystem

| Repo | Family | Role |
|---|---|---|
| [mind-intelligence-systems](https://github.com/frankxai/mind-intelligence-systems) | canon | naming · models · mesh |
| [human-mind-intelligence-system](https://github.com/frankxai/human-mind-intelligence-system) | cognitive | schemas · ontology |
| [agentic-mind-os](https://github.com/frankxai/agentic-mind-os) | lived OS | personal mind OS *(this repo)* |
| [starlight-mind-os-pro](https://github.com/frankxai/starlight-mind-os-pro) | lived OS | premium distribution |
| [awesome-mind-agent-skills](https://github.com/frankxai/awesome-mind-agent-skills) | discovery | the front door |
| [mind-palace-agent-skills](https://github.com/frankxai/mind-palace-agent-skills) | memory palace | Blessing skills |
| [frankx-mind-palace](https://github.com/frankxai/frankx-mind-palace) | memory palace | blessed work as data |

---

## License & attestation
MIT — see [`LICENSE`](LICENSE).
**Built on SIP.** Composes the [Starlight Intelligence Protocol](https://github.com/frankxai/Starlight-Intelligence-System). Per SIP § Sovereignty clause.
Built by [Frank Riemer](https://frankx.ai). For builders, not consumers.
