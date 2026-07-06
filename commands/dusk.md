---
command: /dusk
skill: daily-priming-ritual
reads: [daily/]
writes: [daily/]
---

# /dusk

Run the evening reflection — close the day's loop. Ten prompts on what you gave, what
you learned, where you followed intuition, and where you made progress. The counterpart
to [`/dawn`](dawn.md); together they bracket the day.

## Usage

```
/dusk                # read the sequence aloud, reflect
/dusk --capture      # write answers into today's daily note
/dusk --brief        # the 3 that carry most signal (learned · progress · grateful)
```

## What it does

1. Loads the `daily-priming-ritual` skill.
2. Prints the evening sequence one prompt at a time. Reflection runs the cadence in
   reverse: recall the actual moment from today, then let the feeling register —
   before writing the answer down.
3. In `--capture` mode: appends a `## Reflection` block to `daily/YYYY-MM-DD.md`, and
   folds *what did I learn* / *did I follow my intuition* / *where did I make progress*
   into the note's existing `## Learned (learning · metacognition)`,
   `## What moved me (emotion)`, and `## Decided / did (decision-making · behavior)`
   sections rather than duplicating. Tags touched constructs on the `constructs::` line.
4. Surfaces prompt 8 (*where did I make progress*) as the hook for any external
   accountability you keep — it names the entry; it does not own the ledger.

## Output

Read-aloud by default. With `--capture`, a `## Reflection` block in today's daily note —
which is exactly the recurrence signal `/review-week` consolidates on come Sunday.

## Guardrail

Reflection, not diagnosis. `observation → interpretation → hypothesis → evidence →
decision` stays separated; the call is always yours. No clinical language. On crisis,
the ritual stops and points to real human help. See [`../CANON.md`](../CANON.md).

Built on SIP.
