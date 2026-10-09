# KPI Influence Explorer

A lightweight single-page dashboard for exploring directional, conceptual relationships between executive KPIs across business functions.

## Overview

This project presents a browser-based KPI influence map for leadership teams. It allows users to:

- search for a KPI by name
- filter by executive function
- view upstream and downstream KPI relationships
- inspect a local network diagram of the selected KPI
- rank KPIs by connectivity and influence patterns

The page is implemented in plain HTML, CSS, and JavaScript and does not require a build step or external dependencies.

## What the project does

The dashboard models a set of executive KPIs grouped by functions such as:

- Finance
- Operations
- Technology
- Security
- IT
- Marketing
- Human Resources
- Procurement

It then builds a simple directed graph where arrows point from an influencing KPI to a KPI it may affect. This is intentionally framed as a conceptual model for exploration, not as statistical proof or causal validation.

## Files in this project

- [index.html](index.html) — the full application including layout, styles, and dashboard logic
- [README.md](README.md) — project documentation

## How to run it

Because this is a static HTML application, you can run it in either of these ways:

1. Open [index.html](index.html) directly in a browser.
2. Or serve the folder locally:

```bash
cd /home/andrewsjohnsamuel/Projects/c-suite-kpis
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Main dashboard features

- KPI search and filtering
- Function-based selection
- Incoming and outgoing influence lists
- Interactive relationship network
- Ranking view for most connected KPIs
- Conceptual caveat displayed in-page to discourage unsupported conclusions

## Important note

This dashboard is designed for strategic discussion and exploratory analysis. The relationships are hypotheses and should be validated with KPI owners, historical performance data, and business context before making decisions.

## Technology stack

- HTML5
- CSS3
- Vanilla JavaScript

## Intended use

This project is useful for:

- executive workshop exploration
- KPI architecture discussions
- leadership narratives around business dependencies
- prototyping a dashboard concept before integrating real data sources
