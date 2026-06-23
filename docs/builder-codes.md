# Builder Codes / ERC-8021 Attribution Research

Builder Codes provide an attribution layer for x402 payments on Base.

x402 CLI tracks Builder Codes as future registry metadata for x402-powered APIs, apps, and agent workflows.

## Current status

* Documentation only
* No real settlement integration
* No real payment execution
* No official affiliation

Builder Code support is research/planned only. x402 CLI does not currently append Builder Codes to real x402 settlement transactions.

## Context

Builder Codes use ERC-8021 Schema 2 and can be added to settlement transaction calldata for onchain attribution of x402 payment traffic to a specific app or project.

Reference: [Coinbase Builder Codes docs](https://docs.cdp.coinbase.com/x402/core-concepts/builder-codes)

## Planned metadata fields

```json
{
  "builderCode": "bc_example",
  "attributionStandard": "ERC-8021 Schema 2",
  "appAttribution": "planned",
  "serviceAttribution": "planned"
}
```

## Registry example

```json
{
  "name": "Weather API",
  "paymentProtocol": "x402",
  "network": "base",
  "asset": "USDC",
  "builderCode": "planned",
  "attributionStandard": "ERC-8021 Schema 2 research",
  "status": "demo"
}
```

## Planned command

```bash
x402cli builder-code <api>
```

Preview Builder Code attribution metadata for an indexed x402 API. Not live yet.
