# Decision log

Lightweight ADR-style format: each decision has a status (**decided** / **open**), context and consequence. Open decisions are this project's real backlog.

---

## DEC-001 — Project name: `float64` ✅ decided

Floating-point home, double precision. Runner-up `jangada-de-pedro` stays reserved as the future blog brand (domain jangadadepedro.pt to be registered). `drop-anchor` and `waterfall` honourably discarded.

## DEC-002 — Repo description ✅ decided

> Double-precision floating home. Plans, research and telemetry for migrating one engineer (and one dog) from solid ground to the Tagus.

GitHub topics: `houseboat`, `liveaboard`, `tejo`, `lisboa`, `boatops`. Website field reserved for jangadadepedro.pt. The original PT tagline ("Casa de vírgula flutuante, precisão dupla…") stays reserved for the blog — the pun only works in Portuguese.

## DEC-003 — Methodology: measure before choosing ✅ decided

Requirements derived from data, not brochures. Before any platform decision: 3–4 weeks of telemetry on current life (ESP32/M5Stack already in the drawer — humidity and temperature per room, smart plugs on key loads), 8–10 interviews with actual liveaboards, and an activity→requirement matrix with MoSCoW priorities (Phase 1.3). The matrix constrains the boat model, not the other way around. The January POC gets acceptance criteria defined before stepping aboard; a NO-GO in February is also a success — it cost €400 to find out instead of €140k.

## DEC-004 — Home berth: Oeiras vs Parque das Nações ⚠️ OPEN

**Context:** the crossing scenario test ([research/oeiras-estuary-crossing.md](../research/oeiras-estuary-crossing.md)) revealed a requirements conflict: Apartboat XL + Oeiras berth + weekend crossings don't coexist.

**Option A — Oeiras is a Must:** the model stops being a houseboat and becomes something CE-C that can handle the estuary mouth — trawler, motorsailer, or a liveable power cat à la Overblue. You trade square metres for seaworthiness.

**Option B — Anchoring getaways in home mode are a Must:** keep the houseboat, base at Parque das Nações (Mar da Palha: sheltered, no bar; Seixal and Alcochete 1h–1h30 away). Oeiras becomes 20 minutes by train.

**Status:** undecided. Note: this may not need deciding yet — Phase 1 telemetry and the interviews should reveal which of the two uses is actually a Must and which is a Nice-to-have.

## DEC-005 — Repo language: English ✅ decided

Content switched from PT-PT to English on 2026-07-28 (folders renamed: `planos`→`plans`, `investigacao`→`research`, `telemetria`→`telemetry`). Portuguese terms kept where they're the proper noun (*nortada*, Mar da Palha, carta de Marinheiro).

## DEC-006 — Site architecture: plain Jekyll on GitHub Pages ✅ decided

The repo doubles as the project site, built by GitHub Pages' built-in Jekyll — no Actions, no npm, no build step. Custom layouts + CSS; blog entries in `_posts/`, boat archive as the `_boats` collection, scenario suite as the `_scenarios` collection (front matter: `id`, `status` pass/fail/open, `dimension`). Adding a markdown file is publishing. Constraint accepted: only GitHub-whitelisted Jekyll plugins.

---

## Immediate backlog (from roadmap v0.2)

- **SPK-1 — Email the marina** ← critical path: the only thing that can sink the whole project and doesn't depend on us. This week.
- Liveaboard interview script (Phase 1.1).
- Activity-log template to kick off telemetry (Phase 1.2).

> **TODO:** export the "Roadmap casa flutuante" document (artifact from the claude.ai conversation) into `plans/roadmap-v0.2.md` — it's the source of these phases and the full backlog. Translate to English on the way in.
