# float64

```c
// TODO: move house
```

> Double-precision floating home. Plans, research and telemetry for migrating one engineer (and one dog) from solid ground to the Tagus.

**This repo is a website:** https://pjcorreia.github.io/float64/ — GitHub Pages renders it straight from `main`; pushing a markdown file is publishing.

## Structure

| Path | What it is |
|---|---|
| `_posts/` | The log — blog entries, newest at [/log/](https://pjcorreia.github.io/float64/log/) |
| `_boats/` | Boat archive — one file per model worth tracking, front matter carries the specs |
| `_scenarios/` | The unit-test suite for life aboard — Given/When/Then, status `pass`/`fail`/`open` |
| `plans/` | [Roadmap](plans/roadmap.md) and [decision log](plans/decisions.md) |
| `research/` | Research notes (marinas, navigation, legislation, costs) |
| `telemetry/` | Real-world measurements, land baseline first |
| `_layouts/`, `assets/`, `_config.yml` | The site itself — plain Jekyll, no build tooling |

## Adding content

- **Log entry:** `_posts/YYYY-MM-DD-slug.md` with a `title` in front matter.
- **Boat:** `_boats/slug.md` — copy an existing file, fill the spec front matter, end with a verdict.
- **Scenario:** `_scenarios/scn-NNN-slug.md` — `id`, `title`, `status`, `dimension` in front matter, Given/When/Then in the body. Every dimension of land life must have at least one.

---

*Rollback plan: dry land isn't going anywhere.*
