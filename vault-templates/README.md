# Vault Templates

The local-first vault skeleton you copy and live in. It's plain markdown — open it as an [Obsidian](https://obsidian.md) vault, or edit the files in any text editor. Nothing here phones home; your mind stays on your machine.

## Layout

```
vault-templates/
├── daily/          # one capture note per day  →  daily/YYYY-MM-DD.md
│   └── _template.md
├── weekly/         # weekly intentions + the consolidation review
│   ├── _intentions-template.md
│   └── _review-template.md
├── constructs/     # one note per cognitive module — the 12 canonical constructs
│   ├── attention.md
│   ├── memory.md
│   └── ... (the other ten)
└── reviews/        # consolidation outputs from /review-week and /map-mind
```

The four folders map to the loop:

- **`daily/`** — capture. Write what's on your mind. Don't structure it.
- **`weekly/`** — intend, then consolidate. Set 1–3 intentions Monday; run the review Sunday.
- **`constructs/`** — the shared lenses. One note per construct, where atomic notes and personal canon accrete over time.
- **`reviews/`** — the kept record. Maps and consolidations land here.

## Setup

```bash
# Copy the skeleton somewhere you live — NOT inside this repo.
cp -r vault-templates ~/mind-vault

# Open ~/mind-vault in Obsidian (File → Open vault → pick the folder),
# or just start editing the .md files. Either works.
```

The files prefixed `_` (e.g. `_template.md`) are templates — copy them, don't edit them in place. In Obsidian, point the core **Templates** plugin at `weekly/` and `daily/` and you can insert them with a hotkey.

## The constructs

The 12 `constructs/` notes are the vocabulary every agent and skill uses to read what you write: `attention`, `memory`, `emotion`, `motivation`, `identity`, `learning`, `belief`, `behavior`, `consciousness`, `metacognition`, `decision-making`, `social-cognition`. They come straight from the canonical [human-mind model](https://github.com/frankxai/mind-intelligence-systems). Two representative ones (`attention`, `memory`) ship filled in; the pattern is the same for all twelve — define it, list what to notice, leave room for your own notes to accrete.

## A note on privacy

A real vault is private and belongs to you. This repo ships **templates only**. The repo's `.gitignore` blocks common vault paths so you never accidentally commit your own notes back here. Keep your lived vault outside the repo.

Built on SIP. Part of [Agentic Mind OS](../README.md).
