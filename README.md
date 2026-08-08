# Canada Renewable Grid Explorer

An interactive, single-file web app that explains how nine different electricity sources — Wind, Solar, Hydro, Geothermal, Tidal, Biomass, Fossil Fuels, and Nuclear — actually get from raw resource to a home's outlet, using Nova Scotia's real grid as the running example.

**[Live demo →](https://tmugomba.github.io/renewable-grid-explorer/)**https://tmugomba.github.io/renewable-grid-explorer/

## Why I built this

Most public explainers on electricity generation stop at "here's how a turbine works." This tool tries to go one step further and show the whole chain — resource → generation equipment → step-up transformer → collector system → substation → transmission → distribution → home — with the actual voltages, real Nova Scotia projects, and the genuine controversies and trade-offs involved, instead of a sanitized textbook version.

It also doesn't pretend every source is simple or spotless. The Biomass tab covers the Point Tupper wood-sourcing fight. The Tidal tab is honest about how many FORCE demonstration turbines have failed. The Fossil Fuels tab tracks how many "closures" are actually fuel-switches to heavy fuel oil. The Nuclear tab is upfront that Nova Scotia has never had a reactor and explains, with real reasoning, why — rather than skipping the topic.

## What's inside

Each of the eight source tabs has two views:

- **Flow Diagram** — an animated SVG chain from resource to home. Click any stage (or use the legend) to select it, then press Enter or double-tap to zoom into a fully labelled close-up of that piece of equipment.
- **Development Flow** — a step-by-step walkthrough of how a real project like this gets sited, permitted, and connected to the grid in Nova Scotia, plus a timeline of an actual local project or, where relevant (Fossil Fuels, Nuclear), the real regulatory or structural story instead of a construction pathway.

A ninth tab, **General**, gives the national picture: Canada's 2023 generation mix, progress against climate targets, and a lifecycle-emissions comparison across all nine sources.

**Real projects referenced throughout:**
- Nova East Wind (proposed floating offshore wind, Goldboro)
- Mersey River Wind / Roswall Development (Liverpool)
- Muskrat Falls & the Maritime Link
- Point Tupper biomass plant
- FORCE tidal test site (Bay of Fundy)
- NS Power's coal fleet (Lingan, Point Aconi, Trenton) and its 2030 phase-out
- Point Lepreau, NB (Atlantic Canada's only nuclear reactor)

## Tech stack

Single-file HTML/CSS/JavaScript — no build step, no backend, no API keys, no dependencies. Deploys instantly to GitHub Pages by copying one file. All diagrams are hand-built SVG with SMIL animation; interactivity is vanilla JS with a single `state` object as the source of truth.

- **Fonts:** Space Grotesk (UI), JetBrains Mono (data/labels)
- **Design:** dark navy base, amber primary accent, cyan secondary accent, with a light-theme toggle
- **Accessibility:** every diagram stage is keyboard-navigable (Tab + Enter) and screen-reader labelled

## Running locally

There's nothing to install — clone the repo and open `index.html` in a browser.

```bash
git clone https://github.com/tmugomba/renewable-grid-explorer.git
cd renewable-grid-explorer
open index.html   # or just double-click it
```

## About the author

**Tendekai Mugomba**
Electrical Engineering student with hands-on solar PV analytics and energy data experience from a co-op in the operations team at Killam Apartment REIT. Building this portfolio ahead of a full-time job search in Nova Scotia's renewable energy sector.

- LinkedIn: [linkedin.com/in/tendekai-mugomba](https://www.linkedin.com/in/tendekai-mugomba)
- GitHub: [github.com/tmugomba](https://github.com/tmugomba)
