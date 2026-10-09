# Executive KPI Influence Dashboard

A static HTML dashboard for exploring directional, conceptual relationships between executive KPIs across business functions.

## Overview

This project is designed for leadership and strategy teams who want to explore how executive KPIs may influence one another across functional areas such as finance, operations, technology, security, marketing, HR, and procurement.

The application is intentionally lightweight and deployment-friendly:

- it uses plain HTML, CSS, and vanilla JavaScript
- it has no build step or package installation
- it works well as a GitHub Pages static site

## Included views

### 1. KPI Influence Explorer
The main page in [index.html](index.html) provides:

- KPI search by name
- filtering by executive function
- incoming and outgoing relationship lists
- a local influence network around the selected KPI
- a ranking view for the most connected KPIs
- a conceptual model note clarifying that these are not measured causal claims

### 2. Full Correlation / Heatmap View
The secondary page in [correlation.html](correlation.html) provides:

- a full executive-level relationship matrix
- animated directional flow styling
- a function-by-function heatmap of relationship intensity
- click-to-drill-down detail for selected function pairs
- a side panel showing the underlying KPI relationships behind each cell

## Data model

The project models a set of executive KPIs grouped into eight functions:

- Finance
- Operations
- Technology
- Security
- IT
- Marketing
- Human Resources
- Procurement

The relationships are directional and conceptual. They are intended for exploration, discussion, and portfolio-level storytelling rather than statistical proof.

## Files in this project

- [index.html](index.html) — main executive KPI explorer dashboard
- [correlation.html](correlation.html) — full heatmap and animated correlation view
- [README.md](README.md) — project documentation

## How to run locally

Because this is a static site, you can run it with any local web server.

### Option 1: Open directly
Open [index.html](index.html) in a browser.

### Option 2: Serve locally
```bash
cd /home/andrewsjohnsamuel/Projects/c-suite-kpis
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## GitHub Pages

This project is suitable for GitHub Pages because it is a static frontend with no dependency installation or build pipeline.

Typical setup:

1. Push the repository to GitHub
2. In the repository settings, enable GitHub Pages
3. Use the root folder or the project folder as the published source
4. Open the generated GitHub Pages URL

## Main use cases

This dashboard is useful for:

- executive workshop exploration
- leadership discussions about KPI dependencies
- strategic portfolio mapping
- prototyping relationship views before connecting to live data

## Important note

The relationships shown are hypotheses for discussion, not measured correlations or definitive cause-and-effect evidence. They should be validated with KPI owners, historical trends, and business context before using them for decisions.

## Technology stack

- HTML5
- CSS3
- Vanilla JavaScript

## Example workflow

1. Open the KPI explorer and search for a metric
2. Review upstream and downstream drivers
3. Switch to the full heatmap view for high-level function-to-function patterns
4. Click a heatmap cell to inspect the specific KPI pairs behind that relationship
