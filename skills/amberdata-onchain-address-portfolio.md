---
name: Profile an on-chain address
description: Retrieve native and token balances, portfolio value, and transaction history for a blockchain address from the Amberdata Blockchain API.
api: openapi/amberdata-blockchain-openapi.yaml
operations: [address-balances, get-address-tokens, portfolio, get-address-transactions, get-historical-account-balances]
generated: '2026-07-22'
method: generated
---

# Profile an on-chain address

Base URL: `https://api.amberdata.com/blockchains` — send the `x-api-key`
header on every request, plus the `x-amberdata-blockchain-id` header where
documented to select the network. Data returns in the `{status, title,
description, payload}` envelope.

## Steps

1. **Native balance** — `address-balances` (`GET /addresses/{hash}/balances`)
   for the address's current native-asset balance.
2. **Token holdings** — `get-address-tokens` (`GET
   /addresses/{hash}/token-balances/latest`) for current ERC-20/token
   balances.
3. **Portfolio value** — `portfolio` (`GET /addresses/{address}/portfolio`)
   for the priced portfolio view of the address.
4. **Transactions** — `get-address-transactions` (`GET
   /addresses/{hash}/transactions`) with `startDate`/`endDate` for history.
5. **Balance history** — `get-historical-account-balances` (`GET
   /addresses/{hash}/account-balances/historical`) to chart balance over time.

## Rules

- 404 means the address does not exist on the selected blockchain — verify
  the address and network before retrying.
- Blockchain endpoints accept `validationMethod=none|basic|full` to attach
  block-validation proof data when you need verifiable results.
- Paginate with `payload.metadata.next` or the `page` parameter; respect the
  10 MB response cap (400 = narrow the query).
