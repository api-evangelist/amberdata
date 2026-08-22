# Amberdata (amberdata)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Amberdata delivers institutional-grade digital asset and blockchain data through its REST API at https://api.amberdata.com. Coverage spans spot market data (prices, OHLCV, tickers, trades, order books), derivatives across futures and options (funding rates, open interest, liquidations, implied volatility, Greeks), DeFi (DEX trades and lending), and on-chain blockchain data (blocks, transactions, addresses, tokens, transfers), plus low-latency WebSocket streaming.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/amberdata/refs/heads/main/apis.yml)

## Tags

- Crypto
- Blockchain
- Market Data
- Digital Assets
- Derivatives
- DeFi
- On-Chain

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Amberdata Spot Market Data API

Spot market data across supported exchanges - reference rates, prices, OHLCV, tickers, historical trades, and order book snapshots and events for any traded pair (e.g. eth_usd, btc_usd).

- **Human URL:** [https://docs.amberdata.io/reference/spot-reference](https://docs.amberdata.io/reference/spot-reference)
- **Base URL:** `https://api.amberdata.com`

#### Tags

- Spot
- Market Data
- Prices
- OHLCV
- Trades
- Order Books

#### Properties

- [Documentation](https://docs.amberdata.io/http/http-api-fundamentals)
- [API Reference](https://docs.amberdata.io/reference/spot-reference)
- [OpenAPI](openapi/amberdata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/amberdata-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/amberdata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amberdata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amberdata Derivatives API

Futures and options market data and analytics - OHLCV, tickers, trades, open interest, funding rates, liquidations, long/short ratio, order books, plus options implied volatility, Greeks, term structure, and skew.

- **Human URL:** [https://docs.amberdata.io/reference/futures-exchanges-reference](https://docs.amberdata.io/reference/futures-exchanges-reference)
- **Base URL:** `https://api.amberdata.com`

#### Tags

- Derivatives
- Futures
- Options
- Funding Rates
- Open Interest
- Implied Volatility

#### Properties

- [Documentation](https://docs.amberdata.io/http/analytics/derivatives/instruments-information)
- [API Reference](https://docs.amberdata.io/reference/futures-exchanges-reference)
- [OpenAPI](openapi/amberdata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/amberdata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amberdata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amberdata DeFi API

Decentralized finance data covering DEX pair prices, trades and liquidity (e.g. Uniswap V3), and lending protocol, asset, and wallet position metrics.

- **Human URL:** [https://docs.amberdata.io/reference/defi-reference](https://docs.amberdata.io/reference/defi-reference)
- **Base URL:** `https://api.amberdata.com`

#### Tags

- DeFi
- DEX
- Lending
- Uniswap
- Liquidity

#### Properties

- [Documentation](https://docs.amberdata.io/reference/defi-reference)
- [OpenAPI](openapi/amberdata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/amberdata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amberdata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amberdata On-Chain API

On-chain blockchain data across supported networks - blocks, transactions, addresses (balances, token balances, transactions), tokens (information, transfers, holders), and account balances, sourced from Amberdata's own full nodes from the genesis block forward.

- **Human URL:** [https://docs.amberdata.io/docs/transactions](https://docs.amberdata.io/docs/transactions)
- **Base URL:** `https://api.amberdata.com`

#### Tags

- On-Chain
- Blockchain
- Blocks
- Transactions
- Addresses
- Tokens

#### Properties

- [Documentation](https://docs.amberdata.io/docs/transactions)
- [OpenAPI](openapi/amberdata-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/amberdata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amberdata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Amberdata WebSocket Streaming API

Low-latency real-time WebSocket streaming over a JSON-RPC 2.0 subscribe interface for spot trades and prices, DEX data, and on-chain events, authenticated with the x-api-key header.

- **Human URL:** [https://docs.amberdata.io/real-time/websocket-getting-started](https://docs.amberdata.io/real-time/websocket-getting-started)
- **Base URL:** `wss://ws.web3api.io`

#### Tags

- WebSocket
- Streaming
- Real Time
- Low Latency

#### Properties

- [Documentation](https://docs.amberdata.io/real-time/websocket-getting-started)
- [API Reference](https://docs.amberdata.io/reference/ws-connection)
- [AsyncAPI](asyncapi/amberdata-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/amberdata.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/amberdata.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/amberdata)
- [LinkedIn](https://www.linkedin.com/company/amberdata)
- [Website](https://www.amberdata.io)
- [Documentation](https://docs.amberdata.io)
- [Plans](plans/amberdata-plans-pricing.yml)
- [Rate Limits](rate-limits/amberdata-rate-limits.yml)
- [Fin Ops](finops/amberdata-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
