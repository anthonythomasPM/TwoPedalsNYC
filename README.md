# Two Pedals

**twopedals.nyc** | A bike lane disruption tracker for New York City cyclists

---

## The Problem

New York City's cycling infrastructure is constantly disrupted by construction, repaving, and major capital projects. But getting a clear picture of what's affected, where, and for how long is genuinely hard.

The city's open data systems cover street construction permits issued by NYC DOT, but that's only part of the story. A significant portion of the projects that impact bike lanes and greenways are controlled by state authorities: the MTA, NYSDOT, the Battery Park City Authority, the Hudson River Park Trust, the Port Authority of NY & NJ, and NYS Parks. Those projects don't appear in NYC's open data at all. They're reported by different agencies, on different websites, in different formats, on different schedules.

For a cyclist trying to plan a route or understand what's coming, there's no single place to look. Two Pedals is that place.

---

## What I Built

**A unified map that combines automated and manually curated data into a single, readable view.**

Repaving and milling schedules are pulled from structured open data sources and updated automatically. Major construction projects, which require tracking across multiple agency websites and formats, are manually curated and enriched with field-report photographs where available. Both layers surface together on one map, so users get a complete picture without knowing or caring where the data came from.

**A flexible visual design system, built with Claude, capable of representing very different types of disruption.**

A repaving schedule and a multi-year capital resiliency project are fundamentally different things. The design system handles both: custom iconography, distinct visual treatments for construction complexity and duration, and a layout that doesn't break when the underlying data is messy or incomplete.

**A way to make sense of fragmented agency information.**

Major projects affecting NYC cyclists are reported by a half-dozen different authorities in incompatible formats. Two Pedals normalizes that information into a consistent structure, so users can understand what's happening, who's responsible, and where to find the primary source, without having to know which agency controls which piece of infrastructure.

---

## Product Decisions Worth Noting

**Progressive disclosure.** The map gives users a high-level overview at a glance. Tooltips add context on hover. Clicking a map element opens a detailed view. Users can engage at whatever depth is useful to them, and the interface doesn't front-load complexity.

**Filters that reflect real user needs.** Not every cyclist cares about every disruption. A commuter on a protected lane has different needs than someone planning a long greenway ride. Filters let users narrow to what's relevant, such as resurfacing affecting bike infrastructure specifically, rather than all road work across the city.

**Transparency as a trust mechanism.** Because the data comes from multiple sources with different reliability levels, Two Pedals makes sourcing explicit. Each data layer is explained, and major construction entries link directly to the primary agency source. Users can verify what they're seeing, and the product doesn't ask them to take the data on faith.

---

*Built and maintained by Anthony. Feedback welcome via [twopedals.nyc](https://twopedals.nyc).*
