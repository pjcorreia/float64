---
title: "float64 sets sail"
---

This repo is the public record of a migration: one engineer, one dog (Marley), moving from an apartment near Lisbon to a floating home on the Tagus. Career-wise I've done plenty of migrations; this is the first one where the production environment is literally the river.

The method is the point. No boat gets bought because a brochure looked good. The sequence is:

1. **Measure current life** — 3–4 weeks of telemetry on the land apartment (ESP32 and M5Stack sensors already in the drawer: humidity and temperature per room, smart plugs on the key loads), plus a proper activity log.
2. **Talk to production users** — 8–10 interviews with people actually living aboard in Lisbon-area marinas.
3. **Derive requirements** — an activity→requirement matrix with MoSCoW priorities. The matrix constrains the boat model, not the other way around.
4. **POC in staging** — a January rental with acceptance criteria agreed *before* stepping aboard: productivity, sleep, humidity, Marley.
5. **Go/no-go gates** between phases, and a rollback plan: the land home stays available through one full winter.

A NO-GO in February is also a success — it cost €400 to find out, instead of €140k.

Everything lives here: the [roadmap](../plans/roadmap.md), the [decision log](../plans/decisions.md), a [boat archive](/float64/boats/), and a [scenario suite](/float64/scenarios/) that works like unit tests for life aboard. First failing test already logged — more on that in the next entry.
