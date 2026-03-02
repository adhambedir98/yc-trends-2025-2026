# YC Investment Trends 2025–2026

> Deep dive analysis of **815 YC companies** across 5 batches (Winter 2025 → Winter 2026)

🔗 **Live site:** [yc-trends-2025-2026.vercel.app](https://yc-trends-2025-2026.vercel.app)

## What's in here

A fully self-contained static web app that visualizes Y Combinator's investment patterns across recent batches — built for startup ideation and pattern recognition.

### Features
- **18 macro themes** with momentum indicators (Rising / Surging / Declining etc.)
- **50+ sub-themes** each with real example companies from the YC directory
- **Interactive charts**: company count bar chart, trend momentum bubble matrix
- **Ideation framework**: "White Spaces YC is betting on" vs "Crowded/Risky Territories"
- **Fully responsive** — works on mobile

### Key findings
| Theme | Count | Trend |
|---|---|---|
| AI Agents & Automation | 137 | Dominant |
| Vertical AI for B2B Workflows | 84 | Stable |
| Fintech | 81 | Stable |
| Developer Tools & Code Copilots | 68 | Maturing |
| AI Infrastructure & LLM Tooling | 68 | **Fastest Rising ↑↑** |
| Robotics & Physical AI | 65 | Rock Solid |
| Space Tech | 22 | **Surging ↑↑** |
| Energy & Grid Tech | 14 | **Comeback ↑↑** |
| EdTech & Research Tools | 25 | Declining ↓ |

### White spaces YC is betting on
- **AI Agents for Physical Industries** — factories, construction, logistics
- **AI Infra Below the App Layer** — evals, RAG, memory, observability
- **Voice AI in Regulated Industries** — healthcare, legal, finance phone calls
- **Energy Software for AI Demand** — grid software, data center power
- **Permitting & Regulatory Automation** — FDA, SEC, construction permitting

### Crowded/Risky territories
- Generic AI Dev Tools / LLM Wrappers
- Consumer Social Apps (2.2% of W26 vs 5.4% in Su25)
- Generic Sales AI / SDR Bots
- EdTech (generic)
- Basic AI Chatbots / Copilots

## Project structure

```
yc-trends-2025-2026/
├── index.html          # Main visualization page (self-contained)
├── README.md           # This file
└── data/
    └── companies.json  # Raw data: all 815 companies with archetype + sub-theme classifications
```

## Tech stack

- Vanilla HTML/CSS/JS — zero build step, zero dependencies beyond Chart.js (CDN)
- [Chart.js](https://www.chartjs.org/) for all charts
- Deployed on [Vercel](https://vercel.com) as a static site

## Data source

All data scraped from the [YC Company Directory](https://www.ycombinator.com/companies) filtered to batches W2025–W2026. Classifications (archetypes, sub-themes) generated programmatically via keyword matching against company descriptions and tags.

## Built with

Claude (Anthropic) — data extraction, classification, visualization, and deployment all done via browser automation.

---

*Last updated: March 2026*
