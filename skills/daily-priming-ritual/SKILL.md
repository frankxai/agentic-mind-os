---
name: daily-priming-ritual
description: Runs the morning priming and evening reflection ritual — a fixed sequence of state and action prompts that opens and closes the day. Works two ways: read aloud by a human in a few minutes, or driven by an agent that captures the answers into the daily note and tags them against the 12 constructs so the weekly review has signal. Activates on "prime me", "morning questions", "dawn ritual", "close out my day", "evening reflection", or the `/dawn` and `/dusk` commands.
---

# Daily Priming Ritual

## Purpose

Two short sequences that bracket the day. The morning sequence sets state and picks
the day's few actions before the inbox does it for you. The evening sequence closes
the loop — what you gave, what you learned, where you moved. Both are old technology
(the priming lineage runs through Tony Robbins' morning questions and the Freedom
Mastery planner's *Questions to Empower Your Day*); this skill's only job is to wire
them into the vault so the answers become data the loop can consolidate, not breath
that disappears.

The ritual is priming, not assessment. It asks how you feel and what you appreciate.
It never scores you, never reads a mood as a condition. See the guardrail below.

## When it activates

- You run `/dawn` (morning) or `/dusk` (evening).
- You say "prime me", "morning questions", "run my dawn ritual", "close out the day",
  "evening reflection", "walk me through the questions".
- The top of a fresh `daily/YYYY-MM-DD.md`, before you plan the day.

## Two modes — same questions

**Read-aloud (human).** The agent prints the sequence, one prompt at a time, and gets
out of the way. You answer in your head or in one line, and — this is the part that
does the work — you hold the feeling for a breath before moving on. Five to ten
minutes. No capture required; the point is the state, not the record.

**Captured (agentic).** The agent asks the prompts, takes your one-line answers, and
writes them into today's daily note under a `## Priming` (morning) or `## Reflection`
(evening) block, tagging each against the constructs it touches. Now the weekly
reviewer sees a week of what you were grateful for, committed to, and gave — recurrence
across days is exactly the signal it consolidates on.

Default to read-aloud. Switch to captured when the person says "write it down", "log
this", or is already in a daily note.

## The morning sequence — set state, then pick actions

Seven appreciation/state prompts, then three action prompts. For each state prompt,
the follow-up is always *what about that, and how does it feel* — the feeling is the
anchor, so don't rush past it.

| # | Prompt | Constructs |
|---|---|---|
| 1 | What am I **happy** about in my life right now? | emotion |
| 2 | What am I **excited** about right now? | emotion · motivation |
| 3 | What am I **proud** of right now? | identity · emotion |
| 4 | What am I **grateful** for right now? | emotion · social-cognition |
| 5 | What am I **enjoying** most right now? | emotion · motivation |
| 6 | What am I **committed** to right now? | motivation · identity · behavior |
| 7 | **Whom do I love, and who loves me?** | social-cognition · emotion |
| 8 | How can I make myself feel good, improve one relationship, be present, and give today? | emotion · social-cognition · consciousness · behavior |
| 9 | What are my few most important goals, and the one thing I'll do today toward them? | motivation · decision-making · behavior |
| 10 | What guidance do I want today — and if this were my last day, how would I live it? | belief · metacognition · consciousness |

Prompts 1–7 build state. Prompt 8 turns state outward. Prompts 9–10 convert it into a
decision and a frame. An agent running captured mode writes each answer as the person
said it (observation), never as a claim about them.

## The evening sequence — close the loop

Ten reflection prompts. These feed the daily note's existing sections (`Learned`,
`Decided / did`, `What moved me`) as much as a `## Reflection` block.

| # | Prompt | Constructs |
|---|---|---|
| 1 | What did I give today? Where was I a giver? | behavior · social-cognition |
| 2 | What did I learn? How can I improve? | learning · metacognition |
| 3 | Did I follow my intuition — what did it say? | decision-making · consciousness |
| 4 | How did I follow what I actually care about? | motivation · emotion |
| 5 | Where did I let things flow instead of forcing the outcome? | emotion · belief |
| 6 | How did today add to the quality of my life? Am I enjoying the journey? | consciousness · emotion |
| 7 | Best thing that happened today — how do I create more of it? | memory · learning |
| 8 | Where did I make progress? Did I mark it? | behavior · motivation |
| 9 | What am I grateful for today? How did I love today? | emotion · social-cognition |
| 10 | What help or guidance do I want to ask for? | belief · metacognition |

Prompt 8 is the one to make concrete — "where did I make progress" is the hook for any
external accountability you keep (billable/creation output, a ship log). Naming it here
is enough; the ritual doesn't own that ledger, it just surfaces the entry.

## How the agent writes to the vault (captured mode)

1. Open (or create from `vault-templates/daily/_template.md`) `daily/YYYY-MM-DD.md`.
2. Morning → append a `## Priming` block. Evening → append a `## Reflection` block, and
   fold prompts 2/7/8 into the note's existing `Learned` / `What moved me` /
   `Decided / did` sections rather than duplicating.
3. Write answers verbatim. One line each is fine; blank is fine and is itself data.
4. Add touched constructs to the note's `constructs::` line. Don't invent synonyms —
   only the 12 canonical names.
5. Stop. Don't summarize the person's state back at them, don't grade the day. The
   weekly reviewer does consolidation; the ritual only captures.

## Non-clinical guardrail

This is priming and gratitude, not evaluation. The five-step separation holds:
the agent records what you said (**observation**), may offer a neutral framing only if
asked and always labeled as one (**interpretation**), never a verdict. It never reads a
low-energy answer as a symptom, never names a disorder, never gives medical or
therapeutic advice. "How does that feel" is a prompt for *you*, not a data point for the
agent to diagnose. If an answer signals crisis, the ritual stops and points to real
human help instead of continuing the sequence. See [`../../CANON.md`](../../CANON.md).

## Lineage

The morning/evening priming pattern is adapted from Tony Robbins' priming practice and
the Freedom Mastery planner's *Questions to Empower Your Day / Evening Power Questions*.
Reworded into the OS's construct vocabulary; credit to the originators.

Built on SIP.
