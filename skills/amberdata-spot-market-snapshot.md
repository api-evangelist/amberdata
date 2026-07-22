---
name: Get a spot market snapshot
description: Discover supported exchanges and pull tickers, trades, OHLCV, and an order-book snapshot for a spot instrument from the Amberdata Market Data API.
api: openapi/amberdata-market-openapi.yaml
operations: [get-market-exchanges, spot-tickers-historical, spot-trades-historical, get-historical-ohlc, spot-order-book-snapshots]
generated: '2026-07-22'
method: generated
---

# Get a spot market snapshot

Base URL: `https://api.amberdata.com/markets` — every request needs the
`x-api-key` header and `Accept-Encoding: gzip` (compression is required on
Market Data APIs). Responses arrive in the `{status, title, description,
payload}` envelope; the data is always under `payload`.

## Steps

1. **Discover markets** — `get-market-exchanges` (`GET
   /spot/exchanges/information`). Filter with `exchange` or `pair` query
   params to confirm the instrument is supported and see the data types
   available per market.
2. **Latest tickers** — `spot-tickers-historical` (`GET
   /spot/tickers/{instrument}`) with `exchange=<venue>`. Omit
   `startDate`/`endDate` for the most recent window.
3. **Recent trades** — `spot-trades-historical` (`GET
   /spot/trades/{instrument}`) with `exchange`, `startDate`, `endDate`.
4. **Candles** — `get-historical-ohlc` (`GET /spot/ohlcv/{instrument}`) with
   `exchange` and a `timeInterval` (e.g. minutes, hours, days).
5. **Order book** — `spot-order-book-snapshots` (`GET
   /spot/order-book-snapshots/{instrument}`) with `exchange` for bid/ask depth.

## Rules

- Instruments are lowercase underscore pairs (e.g. `btc_usd`); always pass the
  `exchange` parameter — On-Demand (UAO) keys are rejected without it (403).
- Paginate with `payload.metadata.next` (re-issue that URL with the same
  headers); some endpoints use a zero-based `page` param instead.
- Respect date-range caps per endpoint; chunk long windows client-side.
- 429 means rate limit (Trial 15/s + 20k/day, On-Demand 20/s + 250k/day,
  Enterprise 60/s) — back off. See errors/amberdata-problem-types.yml.
