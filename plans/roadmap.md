# Roadmap

> Reconstructed from the roadmap v0.2 conversation; the original document still needs exporting from claude.ai into this file (see TODO in [decisions](decisions.md)). Structure: phases with go/no-go gates. A NO-GO at any gate is a success of the method, not a failure of the project.

## Phase 0 — Knowledge sprint *(now — time-boxed, per [DEC-007](decisions.md))*

Before any marina hears from us, build enough knowledge to be an informed counterpart:

- **0.1 Course & licence.** Pick and book the boating course (carta de Marinheiro as baseline; evaluate going straight to Patrão Local). Knowing the licence path also answers what we're legally allowed to do ([SCN-001](../_scenarios/scn-001-weekend-crossing-from-oeiras.md)'s daytime-return constraint).
- **0.2 Micro-rental.** Rent a moored houseboat for 2–3 nights — the cheapest possible first data point for [SCN-002](../_scenarios/scn-002-a-week-of-january-gales.md)/[SCN-003](../_scenarios/scn-003-back-to-back-video-calls.md)/[SCN-004](../_scenarios/scn-004-a-normal-tuesday-for-marley.md) before the full January POC.
- **0.3 Market survey.** Populate the [boat archive](../boats/): more models, real pricing, delivery conditions to Lisbon, and what the used market actually offers.
- **SPK-1 — Email the marina(s)** moves to the *exit* of Phase 0: still the question that can kill the project ([SCN-012](../_scenarios/scn-012-the-marina-says-no.md)), now asked from an informed position. With [DEC-004](decisions.md) open, ask both Parque das Nações and Oeiras.

**Gate G0:** course booked or done, nights slept aboard ≥ 2, archive has ≥ 5 models with prices — then SPK-1 goes out.

## Phase 1 — Discovery: measure production

- **1.1 User research** — 8–10 interviews with actual liveaboards in Lisbon-area marinas (interview script to write).
- **1.2 Telemetry of current life** — 3–4 weeks on land: humidity/temperature per room (ESP32/M5Stack), smart plugs on key loads, activity log. This is the baseline every boat scenario gets compared against.
- **1.3 Requirements matrix** — activity → requirement, MoSCoW priorities. The matrix constrains the boat, not the other way around.

**Gate G1:** matrix exists, is data-backed, and DEC-004 has an answer (or a justified deferral).

## Phase 2 — Platform selection

- Shortlist from the [boat archive](../boats/) filtered through the matrix and the [scenario suite](../scenarios/).
- Visits, sea trials where possible, real quotes (boat + berth + insurance + delivery).

**Gate G2:** no scenario still OPEN in any Must dimension; total cost model ([SCN-013](../_scenarios/scn-013-the-real-monthly-burn.md)) complete.

## Phase 3 — POC in staging *(target: January)*

- Rent/borrow a comparable boat and live aboard: weeks not days, normal workdays included, Marley aboard for at least a few nights, same sensors deployed for land-vs-boat comparison.
- Acceptance criteria agreed **before** stepping aboard: productivity, sleep, humidity, Marley.

**Gate G3 — go/no-go.** NO-GO in February costs ~€400. The same discovery in June costs ~€140k.

## Phase 4 — Migration

- Purchase, survey, insurance, berth contract, move aboard.
- **Rollback plan:** the land home stays available through one full winter.

## Phase 5 — Production

- Telemetry aboard, costs logged, scenarios re-run against reality, and the [log](../log/) tells the story.

---

## Immediate backlog

| # | Task | Status |
|---|---|---|
| 0.1a | Shortlist courses/schools (Marinheiro vs Patrão Local), prices and dates | **now** |
| 0.2a | Find rentable moored houseboats near Lisbon, book 2–3 nights | **now** |
| 0.3a | Market survey → boat archive: models, prices, delivery, used market | **now** |
| SPK-1 | Email marinas re: liveaboard policy (PdN + Oeiras) | after Gate G0 |
| 1.1a | Liveaboard interview script | todo |
| 1.2a | Activity-log template + sensor deployment plan | todo |
| — | Export roadmap v0.2 artifact from claude.ai into this file | todo |
