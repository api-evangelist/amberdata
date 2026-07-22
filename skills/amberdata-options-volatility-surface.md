---
name: Analyze options volatility
description: Pull implied-volatility surfaces, term structures, and the volatility index for a crypto asset from the Amberdata Derivatives Analytics API.
api: openapi/amberdata-derivatives-openapi.yaml
operations: [derivatives-information-instruments, derivatives-volatility-delta-surfaces-constant, derivatives-volatility-term-structures-constant, derivatives-volatility-index, derivatives-volatility-implied-vs-realized]
generated: '2026-07-22'
method: generated
---

# Analyze options volatility

Base URL: `https://api.amberdata.com/markets/derivatives` — send the
`x-api-key` header and `Accept-Encoding: gzip` on every request. Data returns
in the `{status, title, description, payload}` envelope.

## Steps

1. **Discover instruments** — `derivatives-information-instruments` (`GET
   /analytics/instruments/information`) with `exchange` (e.g. `deribit`) and
   `currency` (e.g. `BTC`) to enumerate active options instruments.
2. **Delta surface** — `derivatives-volatility-delta-surfaces-constant` (`GET
   /analytics/volatility/delta-surfaces/constant`) with `exchange` +
   `currency` for the constant-maturity implied-vol surface across deltas.
3. **Term structure** — `derivatives-volatility-term-structures-constant`
   (`GET /analytics/volatility/term-structures/forward-volatility/constant`)
   for forward volatility at constant days-to-expiration.
4. **Volatility index** — `derivatives-volatility-index` (`GET
   /analytics/volatility/index`) for the exchange/currency vol index series.
5. **Context** — `derivatives-volatility-implied-vs-realized` (`GET
   /analytics/realized-volatility/implied-vs-realized`) to compare implied
   against realized volatility.

## Rules

- Derivatives analytics are Enterprise-tier data; a 403 means the endpoint is
  outside the key's subscription — do not retry, escalate to the account owner.
- Use `startDate`/`endDate` windows within each endpoint's documented maximum
  range; paginate via `payload.metadata.next`.
- TradFi variants of these analytics exist under `/tradfi` suffixed paths
  (e.g. `tradfi-volatility-delta-surfaces-constant`) for tokenized-equity and
  traditional underliers.
