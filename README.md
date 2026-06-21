# Amberdata (amberdata)

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
