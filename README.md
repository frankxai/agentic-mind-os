# Agentic Mind OS

**A local-first second brain and self-intelligence operating system for students, creators, founders, and lifelong learners.**

Agentic Mind OS is the lived personal layer of Mind Intelligence Systems. It turns raw notes, sources, and reflections into a structured personal canon using agents, skills, and workflows.

## Purpose
Help humans build, maintain, and leverage a high-fidelity second brain that supports learning, reflection, decision-making, and creative output. It is "lived" — designed for daily human use while being fully agent-readable.

## How People Experience It
**Onboarding (7 days)**: Import existing notes → run mind-cartographer agent → build initial canon → first weekly review.

**Daily Experience**:
- Morning: 01_Daily capture with active-recall-generator skill.
- Throughout day: Source distillation (02_Sources → 03_Concepts).
- Evening: Pattern logging in 04_Patterns, link to human-mind models.

**Weekly**: Structured review using weekly-review skill → update 08_Reviews and personal canon.

**Key Vault Structure** (Markdown-first, frontmatter + JSON schemas):
- 00_Start_Here.md
- 01_Daily, 02_Sources, 03_Concepts, 04_Patterns, 05_Learning, 06_Projects, 07_Identity, 08_Reviews

UX is calm, local-first (works offline, Obsidian-compatible), with clear affordances for both humans and agents.

## How Agents Explore It
Agents use:
- vault-template structure
- schemas/ (note.schema.json, pattern.schema.json, review.schema.json)
- agents/ (mind-cartographer.agent.md, learning-architect.agent.md, pattern-analyst.agent.md, memory-governor.agent.md)
- skills/ (daily-mind-capture, weekly-review, source-distillation, active-recall-generator, personal-canon-builder)
- workflows/ (daily-capture.md, weekly-review.md, source-to-canon.md)

**Example Prompt**:
"As memory-governor + pattern-analyst, using human-mind models (memory.md, belief.md, metacognition.md), review last 7 days of captures. Identify recurring patterns in motivation and decision-making. Output structured review using review.schema.json. Suggest updates to personal canon."

Navigation: Start at 00_Start_Here.md → .codex/tasks.md → follow AGENTS.md and SKILL.md.

## Usefulness
- **Humans**: Dramatically improves retention, self-awareness, and creative output. Builds "personal textbook" that compounds over years.
- **Agents**: Fully structured environment enables reliable long-running personal intelligence agents.
- **Integrations**: Feeds directly into Research Intelligence Systems (e.g., distill sources into research packs). Uses shared human-mind models for grounding.
- **Latest Best Tech**: Structured outputs (JSON Schema), ReAct-style agent loops, local-first with frontmatter, integration points for latest LLMs and tools.

See mindpack.yaml, AGENTS.md, HERMES.md, EXPERIENCE.md, AGENT_EXPLORATION.md, USEFULNESS.md, and workflows/.

This is the personal foundation for the entire swarm.