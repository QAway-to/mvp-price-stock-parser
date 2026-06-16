# mvp-price-stock-parser

> Price and stock parser — scrapes product listings, builds SKU-level analytics, and flags restock and price-drop alerts.

A Next.js application that fetches product data from a configurable source URL, parses price and stock fields, computes per-SKU analytics (price history, availability rate), and surfaces actionable alerts. Falls back to bundled mock data when the source is unavailable.

## Features

- **Product table** — sortable list with current price, stock status, and SKU
- **SKU detail** — per-product page with price history chart and stock timeline
- **Alert engine** — flags price drops and low-stock items automatically
- **Source config** — change the target URL without modifying code
- **Fallback data** — bundled `prices.json` ensures the UI always renders

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Next.js (Pages Router) |
| Styling | Inline styles (dark theme) |
| Data | SSR scraping + mock JSON fallback |

## Getting Started

```bash
npm install
npm run dev   # http://localhost:3000
```

## License

MIT
