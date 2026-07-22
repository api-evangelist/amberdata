---
name: Get asset prices and VWAP
description: Look up latest and historical global asset prices and volume-weighted average prices from the Amberdata Price API.
api: openapi/amberdata-price-openapi.yaml
operations: [spot-prices-assets-information, spot-prices-assets-latest, spot-prices-assets-historical, spot-vwap-assets-historical, spot-twap-pairs-historical]
generated: '2026-07-22'
method: generated
---

# Get asset prices and VWAP

Base URL: `https://api.amberdata.com/markets` — send the `x-api-key` header
and `Accept-Encoding: gzip` on every request. Data returns in the `{status,
title, description, payload}` envelope.

## Steps

1. **Discover priced assets** — `spot-prices-assets-information` (`GET
   /spot/prices/assets/information/`) to enumerate assets with price support.
2. **Latest price** — `spot-prices-assets-latest` (`GET
   /spot/prices/assets/{asset}/latest/`) for the current global price of an
   asset (e.g. `btc`).
3. **Price history** — `spot-prices-assets-historical` (`GET
   /spot/prices/assets/{asset}/historical/`) with `startDate`/`endDate` and a
   `timeInterval`.
4. **VWAP** — `spot-vwap-assets-historical` (`GET
   /spot/vwap/assets/{asset}/historical`) for volume-weighted average price
   series.
5. **TWAP (pairs)** — `spot-twap-pairs-historical` (`GET
   /spot/twap/pairs/{pair}/historical`) for time-weighted average price on a
   specific pair.

## Rules

- Asset ids are lowercase symbols (`btc`, `eth`); pairs are underscore form
  (`btc_usd`).
- Keep date windows within each endpoint's maximum range and paginate via
  `payload.metadata.next`.
- Use dated `api-version` headers to pin behavior in production integrations;
  watch https://docs.amberdata.io/changelog/api-changes for breaking changes.
