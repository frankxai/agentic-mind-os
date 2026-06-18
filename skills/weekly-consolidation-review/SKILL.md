---
name: weekly-consolidation-review
description: >
  Run the weekly consolidation review — read the week's daily notes against last week's
  review and the week's intentions, consolidate across the 12 constructs, name concrete
  learnings, and write the carry-forward. Activates on "/review-week", "weekly review",
  "consolidate this week", "close out the week". The keystone of the daily/weekly loop;
  drives the weekly-reviewer agent. Mind-skill of agentic-mind-os.
primary_constructs: [memory, metacognition]
---

# Weekly Consolidation Review

## What it does
The step that turns a week of scattered capture into durable, integrated memory. Mirrors how consolidation actually works — selective (not everything is kept), repeated (built on last week, not from scratch), and integrative (links across days and constructs). It also runs a metacognition pass: not just *what* happened, but what you learned about how you attend, decide, and learn.

## When to use
- The weekly cadence, e.g. Sunday. Triggered by `/review-week`.
- Any time you want to close a stretch of capture into a kept record.

## The procedure

1. **Recall last week.** Read the prior `reviews/` note first. Consolidation strengthens existing structure; starting cold loses the continuity that makes the loop compound.
2. **Read the week.** Pull `daily/` notes in range. If `weekly/` holds intentions you set, hold the week up against them — did attention and behavior match what you meant to do?
3. **Consolidate per construct.** Walk the 12 constructs. For each that appeared: what recurred, what changed, what's worth keeping. **Recurrence across days is the keep-signal** — a one-off thought stays in the daily stream; a pattern that showed up three times earns a place in long-term memory.
4. **Name learnings concretely (metacognition).** A learning is a sentence you can reuse next week. "I focus best before noon and shouldn't schedule deep work after 3pm" is a learning. "It was a hard week" is not. Make them concrete and reusable.
5. **Carry forward.** Pick 1–3 things to bring into next week. Fewer is better. Seed them as next week's intentions in `weekly/`.
6. **Hand off retention.** Pass any learning worth keeping for the long term to `active-recall-generator` so it doesn't decay.
7. **Write `reviews/YYYY-Www.md`** and stop. The plan is the user's to set.

## Output shape
Use [`vault-templates/weekly/_review-template.md`](../../vault-templates/weekly/_review-template.md) as the structure: recap → per-construct consolidation → learnings → carry-forward.

## Quality bar
- Built on last week's review, not from zero.
- Keep-decisions justified by recurrence, not vibe.
- Learnings concrete and reusable.
- Carry-forward is 1–3 items, not a wishlist.

## Guardrail
Consolidates the week; never diagnoses the person. Keeps `observation → interpretation → hypothesis → evidence → decision` separate — reports what recurred, offers readings labeled as readings, proposes carry-forwards as testable experiments, leaves the decision to the user. No clinical or diagnostic language. On any sign of crisis, stop the review and point to real human help. See [`../../CANON.md`](../../CANON.md).

Built on SIP.
