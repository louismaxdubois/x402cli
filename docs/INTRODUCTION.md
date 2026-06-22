# Introduction

x402 CLI is an experimental developer tool for exploring **HTTP 402 Payment Required** payment flows on **Base** using **USDC**.

## What is x402?

x402 applies the HTTP 402 status code to modern API infrastructure. Instead of API keys or subscriptions, services can require **pay-per-request** micropayments before granting access.

Typical flow:

1. Client requests an API endpoint
2. Server responds with `402 Payment Required` + payment metadata
3. Client prepares payment (e.g. USDC on Base)
4. Client retries the request with proof of payment
5. Server returns `200 OK` with the resource

## What x402 CLI provides today

- **Website** at [x402cli.xyz](https://x402cli.xyz) — documentation, registry preview, terminal UI
- **Demo API** at [api.x402cli.xyz](https://api.x402cli.xyz) — endpoints returning real HTTP 402 JSON
- **Updates on X** — follow [@x402cli](https://x.com/x402cli) for progress and announcements
- **Planned CLI** — terminal commands for scan, inspect, registry, and flow simulation

## What it is NOT

- Not an official Coinbase, Base, or x402 product
- Not a payment processor or wallet
- Not a token or investment project

See [DISCLAIMER.md](DISCLAIMER.md).
