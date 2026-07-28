---
title: Home
---

<div class="hero" markdown="1">

# `// TODO: move house`

<p class="tagline">Double-precision floating home. Plans, research and telemetry for migrating one engineer (and one dog) from solid ground to the Tagus — run like any serious migration: requirements first, POC before commitment, telemetry throughout, and a rollback plan always at hand.</p>

</div>

## Where things stand

| | |
|---|---|
| **Phase** | Discovery — measuring current life before choosing a platform |
| **Critical path** | [SPK-1 — email the marina](plans/roadmap.md) |
| **Big open decision** | [DEC-004 — Oeiras vs Parque das Nações](plans/decisions.md) |
| **POC target** | January: weeks aboard, workdays included, Marley aboard |

## Latest from the log

<ul class="item-list">
{% for post in site.posts limit:5 %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a><span class="meta"> — {{ post.date | date: "%-d %b %Y" }}</span></li>
{% endfor %}
</ul>

## How this site works

- **[Log](log/)** — a running journal of findings, visits and conversations.
- **[Boats](boats/)** — archive of manufacturers and models worth tracking, with specs and a verdict.
- **[Scenarios](scenarios/)** — the unit-test suite for life aboard: every dimension of land life gets a scenario, and every scenario ends PASS, FAIL (which generates requirements), or stays OPEN until tested.
- **[Roadmap](plans/roadmap.md)** — phases, gates and the immediate backlog.
- **[Decisions](plans/decisions.md)** — lightweight ADR log; open decisions are the real backlog.
