# Dividend Desk

A small, Vercel-ready research dashboard prototype for forecasting dividend amounts and dates, reviewing company guidance, comparing a simple forward-price scenario, and writing an analyst note.

## Demo data notice

The current screen uses **illustrative demo values**. They are not live market data or verified company forecasts. Forecast dates are estimates generated from a sample payment cadence. Do not use the figures for investment decisions or present them as company facts.

The app is deliberately frontend-only for this first pass. Company source links, filing-backed financial statements, actual event dates, and a point-in-time backtest still need a data source and validation before the results can be represented as research.

## Run locally

```bash
npm install
npm run dev
```

## Deploy to Vercel

Import this repository in Vercel. The framework preset is **Vite**; the build command is `npm run build` and the output directory is `dist`. No environment variables are needed for this demo.

## Included

- Company switcher for a small US and European coverage list.
- Four-payment schedule with estimated declaration, ex, record, and payment dates.
- Mechanical-growth and policy-adjusted amount scenarios.
- Payout-health display, dividend history visual, simple forward-price sensitivity, and analyst-note Markdown export.
- Backtest page showing the intended measures: amount MAPE and ex-date error in days.

## Before publishing research outputs

Connect a reliable source for issuer announcements, financial statements, dividend histories, and prices. Store the source and retrieval/publication dates beside each observation. Calculate backtests from point-in-time records and show sample size and forecast horizon. Treat the current backtest metrics as placeholders until those records are connected.
