# MEMORY.md — Agentic Mind OS

> Durable state for this repo: what it is committed to, where its edges are, and what it
> composes from. An agent entering this repo reads this before acting.

**Version:** 0.1.0

---

## Composes-from

This OS holds no canon of its own. It inherits, in order:

1. **SIP** — [Starlight-Intelligence-System](https://github.com/frankxai/Starlight-Intelligence-System). Substrate, attestation, sovereignty clause.
2. **Canon** — [mind-intelligence-systems](https://github.com/frankxai/mind-intelligence-systems). Naming doctrine, the 12-module human-mind model, the mesh.
3. **Cognitive schemas** — [human-mind-intelligence-system](https://github.com/frankxai/human-mind-intelligence-system). Ontology + response-prediction primitives.

Edges declared in [`mindpack.yaml`](mindpack.yaml). Authority flows down, never up.

---

## Commitments

These are the promises this repo keeps across versions.

- **Local-first.** The user's vault lives on their machine, in plain markdown, openable in Obsidian or any text editor. No cloud dependency to read or write your own mind. The repo ships templates; the lived vault is the user's and stays private.
- **One vocabulary.** Every note, agent, and skill speaks the 12 canonical constructs (`attention`, `memory`, `emotion`, `motivation`, `identity`, `learning`, `belief`, `behavior`, `consciousness`, `metacognition`, `decision-making`, `social-cognition`). No private synonyms. If the model changes, it changes upstream and flows here.
- **The loop is the product.** Capture daily → map on demand → consolidate weekly → carry forward. The value is the loop, not any single agent.
- **Model, never diagnose.** The five-step separation (observation → interpretation → hypothesis → evidence → decision) is non-waivable. See [`CANON.md`](CANON.md).
- **Voice: direct, technical, warm.** No AI-slop, no hype, no guru tone. Show, don't tell.
- **SIP attestation is ambient.** Generated artifacts carry *Built on SIP* without the user invoking anything.

---

## Anti-scope

What this repo deliberately does **not** do. Naming these prevents drift.

- **No diagnosis, no therapy, no treatment.** Not a clinical tool. Not medical advice. Not a substitute for a professional. Hard line.
- **No new canon.** No competing mind model, no naming authority, no construct of its own. Declines its vertical canon per SIP § Sovereignty.
- **No SaaS, no hosting, no accounts.** This is a lived OS, not a platform. The premium/distribution surface (dashboards, onboarding, workshops) is [starlight-mind-os-pro](https://github.com/frankxai/starlight-mind-os-pro)'s job, not this repo's.
- **No research runtime.** Literature workflows, evidence synthesis, psychometrics, and cross-domain research belong to the `research-intelligence-*` family, not here.
- **No data exfiltration.** Agents read and write the local vault. They do not phone home with a person's private notes.
- **No memory-palace / Blessing Protocol, and no method-of-loci as this OS's memory layer.** The `*-mind-palace` sibling ([mind-palace-agent-skills](https://github.com/frankxai/mind-palace-agent-skills)) now spans two registers — the Blessing ritual, and a real method-of-loci mnemonic suite — but neither is this OS's chosen approach. This OS's memory/learning layer stays `recall-builder` + `active-recall-generator` + `distill-to-atomic-notes` (retrieval-practice, atomic-notes pedagogy). Different register, different repo — even for the technique, not just the ritual.

---

## State

- **v0.1.0** — Foundation. Vault skeleton (daily / weekly / constructs / reviews), 4 personal agents (cartographer, weekly-reviewer, focus-coach, recall-builder), 3 mind-skills (distill-to-atomic-notes, active-recall-generator, weekly-consolidation-review), 2 commands (`/review-week`, `/map-mind`). Manifest live in the mesh.

### Next (not committed, just noted)
- Per-construct review prompts in each `constructs/*.md` note.
- A `monthly/` consolidation tier above weekly.
- Optional encryption guidance for the local vault.

---

Built on SIP. Part of the [Mind Intelligence Systems](https://github.com/frankxai/mind-intelligence-systems) ecosystem.
