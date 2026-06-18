---
name: distill-to-atomic-notes
description: >
  Distill raw capture (daily notes, sources, transcripts) into atomic, self-contained,
  linkable notes — one idea per note, in the user's own words, filed under the right
  canonical construct. Activates on "distill this", "make atomic notes", "break this
  down", or when the recall-builder agent processes a week's notes. Improves encoding
  for later retrieval. Mind-skill of agentic-mind-os.
primary_constructs: [memory, learning]
---

# Distill to Atomic Notes

## What it does
Takes messy input and produces atomic notes: each one idea, self-contained, restated in the user's own words, and linked. Atomicity is what makes a note reusable — you can drop it into any future thought without dragging context along. Restating in your own words is the deep-encoding move; copying verbatim is shallow and decays.

## When to use
- After a daily brain-dump that has three good ideas tangled in one paragraph.
- When reading a source worth keeping — distill the claims, not the prose.
- As the first step before `active-recall-generator` (you can't make good questions from a non-atomic note).

## The procedure

1. **Find the ideas.** Read the input. Mark each distinct claim, insight, or fact. A paragraph usually holds 1–4.
2. **One note per idea.** Split. If a note still has an "and" joining two claims, split again.
3. **Restate in your words.** Rewrite each so it stands alone and reads as *yours*. This is the encoding work — don't skip it by pasting the original. If you can't restate it, you don't understand it yet; flag it instead of faking it.
4. **Make it self-contained.** The note should make sense with nothing else open. Inline the minimum context it needs.
5. **File and link.** Tag each note with its canonical construct (`attention`, `memory`, `emotion`, `motivation`, `identity`, `learning`, `belief`, `behavior`, `consciousness`, `metacognition`, `decision-making`, `social-cognition`). Link to related existing notes. Links are what make later retrieval cheap.

## Output shape

```markdown
## <one-line idea, in your words>
<2–4 sentences, self-contained>

construct:: learning
links:: [[<related-note>]], [[constructs/learning]]
source:: daily/2026-06-18  (or the source)
```

## Quality bar
- One idea per note — no compound notes.
- Own words, not pasted text.
- Stands alone — no orphan references.
- Filed under exactly one primary construct from the canonical 12.

## Guardrail
Works on ideas and notes, never on diagnosing the person. No clinical language, no claims about memory health. Distilling is an encoding aid, not an assessment. See [`../../CANON.md`](../../CANON.md).

Built on SIP.
