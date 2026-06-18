---
command: /map-mind
agent: mind-cartographer
reads: [daily/, constructs/]
writes: [reviews/]
---

# /map-mind

Draw back a map of your cognitive and affective state from what you've already written. On-demand, any time — this is the look-at-your-own-mind-from-a-small-distance command. Lighter than `/review-week`: it maps, it doesn't consolidate.

## Usage

```
/map-mind                    # map the current week
/map-mind --days 14          # map a wider window
/map-mind --construct attention   # focus the map on one construct
```

## What it does

1. Dispatches the `mind-cartographer` agent.
2. Reads the daily notes in range and the 12 `constructs/` notes as sorting lenses.
3. Sorts what's there across the constructs — which lit up, which stayed quiet.
4. Surfaces patterns as observations first, then offers readings explicitly labeled as readings.
5. Writes `reviews/YYYY-Www-map.md` — a map note alongside your daily notes, never editing them.

## Output

A `reviews/YYYY-Www-map.md` note: the construct breakdown, the recurring threads (quoted, not paraphrased), and clearly-flagged readings you can test against your own sense of the week.

## Guardrail

Maps; never diagnoses. Observation and interpretation stay separate, interpretations are labeled, and what the map means is yours to decide. No clinical language. On crisis, mapping stops and points to real human help. See [`../CANON.md`](../CANON.md).

Built on SIP.
