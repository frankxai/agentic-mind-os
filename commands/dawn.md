---
command: /dawn
skill: daily-priming-ritual
reads: [daily/]
writes: [daily/]
---

# /dawn

Run the morning priming sequence — set state, then pick the day's few actions before
the day picks them for you. Ten prompts: seven that build state (happy, excited, proud,
grateful, enjoying, committed, loved), one that turns it outward, two that convert it
into a decision and a frame.

## Usage

```
/dawn                # read the sequence aloud — answer in your head, hold each feeling
/dawn --capture      # write answers into today's daily note, tagged by construct
/dawn --brief        # the 3 action prompts only (8–10), when you're short on time
```

## What it does

1. Loads the `daily-priming-ritual` skill.
2. Prints the morning sequence one prompt at a time. For each state prompt (1-7), the
   cadence is answer → *what about that* → picture it → feel it and hold for a
   breath. The felt state is the point; don't rush to the next prompt.
3. In `--capture` mode: opens `daily/YYYY-MM-DD.md` (creating it from the template if
   needed), appends a `## Priming` block with your answers verbatim, and adds the
   touched constructs to the note's `constructs::` line.
4. Stops. It sets you up for the day; it does not plan the day for you.

## Output

Read-aloud by default — nothing is written. With `--capture`, a `## Priming` block in
today's daily note. The evening counterpart is [`/dusk`](dusk.md).

## Guardrail

Priming, not assessment. Answers are recorded as you said them (observation), never
graded or read as a condition. "How does that feel" is a prompt for you, not a data
point to diagnose. On any sign of crisis, the ritual stops and points to real human
help. See [`../CANON.md`](../CANON.md).

Built on SIP.
