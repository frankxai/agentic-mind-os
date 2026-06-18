# Contributing to Agentic Mind OS

Thanks for wanting to make this better. A few things keep the OS coherent as it grows.

## Before you start

Read [`CANON.md`](CANON.md) and [`MEMORY.md`](MEMORY.md). They define what this repo composes, what it declines, and the one rule that never bends. Most rejected changes are rejected because they crossed a line those two files draw.

## The non-negotiables

1. **Model, never diagnose.** Any new agent, skill, or prompt must keep the five steps separate: `observation → interpretation → hypothesis → evidence → decision`. No clinical or diagnostic language. No therapy/treatment claims. On crisis, point to real human help. A contribution that blurs this line will not be merged.
2. **One vocabulary.** Use the 12 canonical constructs exactly as named upstream (`attention`, `memory`, `emotion`, `motivation`, `identity`, `learning`, `belief`, `behavior`, `consciousness`, `metacognition`, `decision-making`, `social-cognition`). No synonyms. If a construct genuinely needs to change, that change belongs upstream in [mind-intelligence-systems](https://github.com/frankxai/mind-intelligence-systems), not here.
3. **Stay in scope.** This is a lived, local-first OS. No SaaS, no hosting, no research runtime, no new canon. See the anti-scope list in [`MEMORY.md`](MEMORY.md).
4. **Local-first.** Never add a hard cloud dependency for reading or writing the vault. Never commit a real vault.

## How to add things

- **A new agent** → an `agents/<id>.md` card with the fixed section shape: Role · When it activates · Reads · Writes · How it works · Non-clinical guardrail. Register it in `mindpack.yaml` under `agents.ships`.
- **A new skill** → a `skills/<id>/SKILL.md` with frontmatter (`name`, `description`) plus a body. Register it under `skills.ships`.
- **A new command** → a `commands/<id>.md` spec. Register it under `commands.ships`.
- **A new vault template** → a note under the right `vault-templates/` folder. List representative ones under `vault_templates.representative_notes`.

## Quality bar

- Voice: direct, technical, warm. No AI-slop, no hype, no guru tone. Show, don't tell.
- Keep `mindpack.yaml` valid YAML. Verify:
  ```bash
  python3 -c "import yaml; yaml.safe_load(open('mindpack.yaml'))"
  ```
- No README or doc link should point to a file that doesn't exist.

## PRs

Small, focused, one concern per PR. Explain the problem you're solving, not just the change. If it touches the safety boundary or the construct vocabulary, say so explicitly so a reviewer can check it carefully.

Built on SIP. For builders, not consumers.
