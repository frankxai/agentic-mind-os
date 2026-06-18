# Codex Task Queue — Agentic Mind OS (AMOS)

**Repo Role**: Personal lived operating system.

Use task IDs starting with `AMOS-`.

## AMOS-001
**Objective**: Create the full vault-template structure with 00_Start_Here.md and all numbered sections.
**Files**: vault-template/00_Start_Here.md, vault-template/01_Daily/README.md, ... up to 08_Reviews/README.md
**Acceptance Criteria**: All 9 top level sections have README or content; 00_Start_Here explains the system and how to use with agents.
**Suggested Command**: `codex exec "Build the complete vault-template/ directory following the spec in the main README. Make each section self-documenting and agent-friendly."`

## AMOS-002
**Objective**: Implement the four core agents as rich .agent.md files.
**Files**: agents/mind-cartographer.agent.md, learning-architect.agent.md, pattern-analyst.agent.md, memory-governor.agent.md
**Acceptance Criteria**: Each has name, description, capabilities, prompt template, example invocations.
**Suggested Command**: `codex exec "Create detailed agent definitions for the four agents listed in the README. Make them ready for Codex/Claude consumption."`

## AMOS-003
**Objective**: Implement the five core skills as SKILL.md.
**Files**: skills/daily-mind-capture/SKILL.md etc for all five.
**Acceptance Criteria**: Each SKILL.md has trigger, steps, inputs, outputs, example usage.
**Suggested Command**: `codex exec "Create production-ready SKILL.md files for the five skills. Follow standard skill format."`

## AMOS-004
**Objective**: Create the three core workflows as executable markdown.
**Files**: workflows/daily-capture.md, weekly-review.md, source-to-canon.md
**Acceptance Criteria**: Step-by-step, references skills and agents, includes success criteria.
**Suggested Command**: `codex exec "Write the three workflows as detailed playbooks that a human or agent can follow end-to-end."`

## AMOS-005
**Objective**: Create the three core JSON schemas.
**Files**: schemas/note.schema.json, pattern.schema.json, review.schema.json
**Acceptance Criteria**: Valid schemas with examples; used by skills.
**Suggested Command**: `codex exec "Define minimal but useful JSON schemas for notes, patterns, and reviews. Include examples in the files."`

## AMOS-006
**Objective**: Flesh out 01_Daily with capture templates and daily agent prompts.
**Files**: vault-template/01_Daily/ (multiple files)
**Acceptance Criteria**: Practical templates for morning/evening capture.
**Suggested Command**: `codex exec "Populate the Daily section with high-utility templates."`

## AMOS-007
**Objective**: Add CONTRIBUTING.md, ROADMAP.md, and .github/ISSUE_TEMPLATE/hermes-task.md
**Files**: CONTRIBUTING.md, ROADMAP.md, .github/ISSUE_TEMPLATE/hermes-task.md
**Acceptance Criteria**: Follow the global standard from mind-intelligence-systems.
**Suggested Command**: `codex exec "Add the standard global files adapted for this personal OS repo."`

## AMOS-008
**Objective**: Create HERMES.md and update AGENTS.md with more detail.
**Files**: HERMES.md, AGENTS.md
**Acceptance Criteria**: Clear orchestration and agent guidance.
**Suggested Command**: `codex exec "Ensure HERMES.md and AGENTS.md are complete and reference the swarm correctly."`

## AMOS-009
**Objective**: Add example personal canon starter content.
**Files**: vault-template/07_Identity/personal-canon-starter.md or similar
**Acceptance Criteria**: Useful starting canon examples without being prescriptive.
**Suggested Command**: `codex exec "Add starter content for the Identity and Canon sections."`

## AMOS-010
**Objective**: Add a simple install script or setup guide.
**Files**: scripts/setup-vault.sh or docs/install.md
**Acceptance Criteria**: Helps user copy templates into their vault.
**Suggested Command**: `codex exec "Create installation and setup guidance."`

## Next Focus
AMOS-001, AMOS-002, AMOS-003, AMOS-004, AMOS-005.
