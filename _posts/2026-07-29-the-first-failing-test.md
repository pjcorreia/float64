---
title: "The first failing test"
---

The first scenario I ran against the dream configuration failed, and it's the most useful thing that's happened to this project so far.

The dream: a La Mare Apartboat XL berthed at Oeiras — my home turf — and on good weekends, cross the estuary and anchor off the opposite bank. Three reasonable wishes. The scenario test ([SCN-001](/float64/scenarios/scn-001-weekend-crossing-from-oeiras/)) showed they're valid two at a time, but the three together don't coexist.

The short version: the Apartboat XL fits through Oeiras' entrance with room to spare (the port takes up to 25 m length, 6 m beam, 3 m draft). But what's outside is the throat of the estuary — the main shipping channel, spring-tide currents over 2–3 knots, Atlantic swell through the bar, and the *nortada* filling in before lunch. A CE category D box certified for 0.3 m waves, with sail-like walls, two small outboards and 5 knots of top speed, has no margin there. Full analysis in the [research note](/float64/research/oeiras-estuary-crossing.html).

Meanwhile the same weekend from Parque das Nações is a sheltered classic across the Mar da Palha: anchor in Seixal bay or off Alcochete, 1h–1h30 at 5 knots, flamingos at dawn.

So the failing test generated exactly what a failing test should:

- **Five new requirements** for the matrix: oversized anchor, anchor light, tide planning (the flats dry), daytime-only returns, and a dinghy — because Marley needs shore leave and nobody rows a house.
- **One decision**, now open as [DEC-004](/float64/plans/decisions.html): if Oeiras is a Must, the platform stops being a houseboat and becomes something CE-C (trawler, motorsailer, liveable power cat). If anchoring getaways in home mode are the Must, the houseboat stays and the base moves upriver.

The suite is seeded with twelve more scenarios — winter gales, video calls, a dog's Tuesday, haul-out, the 3 a.m. emergency. Red-green-refactor, but for a life.
