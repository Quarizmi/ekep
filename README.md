# EKEP — Exhaustive Keyword Extraction Process

> A continuously running toolset that discovers long-tail keywords from every source available — refreshed every hour.

EKEP is an open-source set of tools built by [Quarizmi](https://quarizmi.com) to generate long-tail keywords continuously. It mines every available source — your own account history, Google's keyword tools, organic search data, analytics, and the open web — and refreshes every hour, so new opportunities surface as soon as demand appears.

---

## Why long-tail?

Long-tail keywords are longer, more specific search terms. Each one has lower volume, but together they make up a large share of search demand — and they usually convert better and cost less than broad head terms. The hard part is finding them at scale, and finding them continuously. That's what EKEP does.

## Features

- **Exhaustive discovery** — pulls candidate keywords from every connected source, not just one tool.
- **Continuous refresh** — runs every hour to surface new long-tail terms as demand shifts.
- **Demand-aware** — how many new keywords appear each hour depends on the client, the industry, and current market demand.
- **Standalone or connected** — use it on its own, or feed its output into the rest of the Quarizmi suite.

## Data sources

| Source | What EKEP uses it for |
|---|---|
| Client historical data | Search terms and keywords that have already driven traffic and conversions |
| Google Keyword Planner | Keyword ideas, related terms, and volume estimates |
| Google Search Console | Queries the site already appears for in organic results |
| Google Analytics | On-site behavior and performance beyond the ad platform |
| Web crawling | New terms and phrasing discovered on the open web |

## How it works

```
 Sources ──► Extract ──► Expand ──► Deduplicate & filter ──► Long-tail keyword list
   ▲                                                                  │
   └───────────────────────── refresh every hour ◄────────────────────┘
```

## Getting started

> **Note:** The implementation language and setup steps are still being finalized. This section will be updated.

### Prerequisites

- Google Ads API access (developer token + OAuth credentials)
- Google Search Console API access
- Google Analytics API access
- _TBD: runtime and dependencies_

### Installation

```bash
git clone https://github.com/<org>/ekep.git
cd ekep
# TBD: install dependencies
```

### Configuration

```bash
# TBD: environment variables / config file for API credentials
```

### Running

```bash
# TBD: run command
```

## Part of the Quarizmi suite

EKEP works on its own, but it's also the engine at the start of Quarizmi's end-to-end paid-search system:

- **EKEP** — discovers long-tail keywords _(you are here)_
- **[Bidbot](../bidbot)** — decides bids and which keywords to turn on or off
- **[Usable](../usable)** — builds full campaigns with the user in the loop
- **[Magneto](../magneto)** — writes high-relevance ads for every keyword
- **[Health Checker](../health-checker)** — grades an existing Google Ads account (standalone)

## Use it yourself, or work with us

EKEP is free and open source — use it, fork it, adapt it. If you'd rather have it run for you, Quarizmi can set it up and operate it on your account. Get in touch at **[quarizmi.com](https://quarizmi.com)**.

## Contributing

Contributions are welcome. Please open an issue to discuss a change before submitting a pull request.

## License

Released under the [MIT License](LICENSE). © 2026 Quarizmi AdTech.
