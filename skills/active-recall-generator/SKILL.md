---
name: active-recall-generator
description: >
  Generate active-recall questions from atomic notes or consolidated learnings — questions
  that force retrieval, not recognition — so captured material becomes durable memory.
  Activates on "make recall questions", "quiz me on this", "turn this into flashcards",
  or when the recall-builder agent processes carry-forward learnings. Wraps retrieval
  practice, the highest-leverage move in the learning construct. Mind-skill of agentic-mind-os.
primary_constructs: [memory, learning]
---

# Active Recall Generator

## What it does
Converts notes into questions that make you *retrieve* an answer from memory rather than *recognize* it on a page. Retrieval practice is the single most reliable way to move something from fragile short-term encoding into durable long-term memory. Recognition ("does this look right?") feels easier and does almost nothing; this skill refuses to generate it.

## When to use
- After `distill-to-atomic-notes` — atomic notes make clean questions.
- On the weekly review's carry-forward learnings — the things you most want to keep.
- Any time you want a self-test set for a topic in the vault.

## The procedure

1. **Take atomic input.** Best from atomic notes or consolidated learnings. Non-atomic input produces vague questions — distill first.
2. **Write retrieval questions.** For each idea, write a question that can't be answered without recalling. Prefer:
   - "What is the difference between X and Y?" over "Is X different from Y?"
   - "Why does X lead to Y?" over "Does X lead to Y?"
   - "When would you use X instead of Y?" over "Can you use X?"
   Open-ended and generative beats yes/no and multiple-choice for durability.
3. **Pair with a terse answer.** One clear answer per question, in the user's words.
4. **Tag construct + source.** So the set links back into the vault.
5. **Vary difficulty.** Mix a few easy recalls with harder synthesis questions ("how do X and Z combine?"). Synthesis questions exercise the links, not just the facts.

## Output shape

```markdown
### Recall set — <topic> — <date>

Q: <retrieval question>
A: <terse answer in your words>
construct:: memory
source:: [[<atomic-note>]]

Q: ...
A: ...
```

## Quality bar
- Every question forces retrieval — no recognition, no yes/no padding.
- One unambiguous answer each.
- At least one synthesis question per set if the material supports it.
- Linked back to source notes and a construct.

## Guardrail
Generates study material from notes, never an assessment of the person. No claims about memory capacity or health; forgetting is normal and expected. No clinical language. See [`../../CANON.md`](../../CANON.md).

Built on SIP.
