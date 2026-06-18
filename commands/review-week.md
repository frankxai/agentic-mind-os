---
command: /review-week
agent: weekly-reviewer
skill: weekly-consolidation-review
reads: [daily/, weekly/, reviews/]
writes: [reviews/, weekly/]
---

# /review-week

Run the weekly consolidation review — the keystone of the loop. Reads the week's daily notes against last week's review and the week's intentions, consolidates across the 12 constructs, names concrete learnings, and writes the carry-forward.

## Usage

```
/review-week                 # review the current ISO week
/review-week 2026-W24        # review a specific week
/review-week --since 2026-06-09 --until 2026-06-15   # explicit range
```

## What it does

1. Dispatches the `weekly-reviewer` agent, which loads the `weekly-consolidation-review` skill.
2. Recalls last week's `reviews/` note for continuity.
3. Reads the range's `daily/` notes and any `weekly/` intentions.
4. Consolidates per construct (recurrence = keep-signal), names reusable learnings, picks 1–3 carry-forwards.
5. Writes `reviews/YYYY-Www.md` and seeds next week's intentions into `weekly/`.
6. Hands durable learnings to `recall-builder` if you want retention sets.

## Output

A new `reviews/YYYY-Www.md` note following [`vault-templates/weekly/_review-template.md`](../vault-templates/weekly/_review-template.md). It never edits your daily notes — only produces the consolidation alongside them.

## Guardrail

Consolidation, not diagnosis. The `observation → interpretation → hypothesis → evidence → decision` separation holds; the decision stays yours. No clinical language. On crisis, the review stops and points to real human help. See [`../CANON.md`](../CANON.md).

Built on SIP.
