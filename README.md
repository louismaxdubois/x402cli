<p align="center">
  <img src="logo.png" alt="x402 CLI" width="160">
</p>

# x402 CLI

x402 CLI is an experimental discovery and testing layer for x402-powered APIs on Base.

It focuses on HTTP 402 payment inspection, API registry exploration, Base + USDC payment flow research, future MCP-ready agent workflows, and Builder Code / ERC-8021 attribution research.

> Status: early experimental development.

## Website

https://x402cli.xyz

## Community Token — $X402CLI

**$X402CLI** is the community token for x402 CLI — live on **Base**. It exists to help grow the ecosystem around x402 API discovery, builder tooling, and agent-ready payment workflows on Base.

Holding or trading $X402CLI is optional and not required to use the website, docs, or planned CLI. If you choose to participate, do your own research and only use funds you can afford to lose.

| | |
|---|---|
| **Network** | Base |
| **Symbol** | `$X402CLI` |
| **Contract** | `0x6fBEb18fc6Ab14b170EcfB21c9a2f2384b155bA3` |

### Trade $X402CLI

| Platform | Link |
|----------|------|
| BANKR | [bankr.bot/launches](https://bankr.bot/launches/0x6fBEb18fc6Ab14b170EcfB21c9a2f2384b155bA3) |
| GMGN.AI | [gmgn.ai/base/token](https://gmgn.ai/base/token/0x6fBEb18fc6Ab14b170EcfB21c9a2f2384b155bA3) |
| Uniswap | [Swap on Uniswap](https://app.uniswap.org/swap?chain=base&outputCurrency=0x6fBEb18fc6Ab14b170EcfB21c9a2f2384b155bA3) |
| Dexscreener | [Chart on Dexscreener](https://dexscreener.com/base/0x6fBEb18fc6Ab14b170EcfB21c9a2f2384b155bA3) |
| PancakeSwap | [Swap on PancakeSwap](https://pancakeswap.finance/swap?chain=base&outputCurrency=0x6fBEb18fc6Ab14b170EcfB21c9a2f2384b155bA3) |

Follow **[@x402cli on X](https://x.com/x402cli)** for token updates, launches, and project news.

## Repository Scope

This public repository contains documentation, examples, schemas, roadmap notes, and public project references.

The production website frontend source is not included in this repository at this stage.

## Current Focus

* x402 API discovery
* HTTP 402 Payment Required inspection
* Base + USDC payment flow exploration
* API registry metadata
* MCP-ready agent workflow research
* Builder Codes / ERC-8021 attribution research
* MPP / Tempo compatibility research

## Planned Commands

```bash
x402cli scan <url>
x402cli inspect <url>
x402cli registry
x402cli mcp <api>
x402cli builder-code <api>
x402cli demo
```

The installable CLI package is planned — not live yet. See [docs/commands.md](docs/commands.md).

Builder Code support is research/planned only. x402 CLI does not currently append Builder Codes to real x402 settlement transactions.

## Documentation

| Doc | Description |
|-----|-------------|
| [Overview](docs/overview.md) | Project overview and positioning |
| [x402 Flow](docs/x402-flow.md) | HTTP 402 payment flow |
| [Commands](docs/commands.md) | Planned CLI reference |
| [Registry](docs/registry.md) | API registry preview |
| [Registry Schema](docs/registry-schema.md) | Registry entry schema |
| [MCP-ready Workflows](docs/mcp-ready-workflows.md) | Agent workflow research |
| [Builder Codes Research](docs/builder-codes.md) | ERC-8021 attribution metadata |
| [MPP / Tempo Research](docs/mpp-tempo-research.md) | Future compatibility research |
| [API Metadata](docs/api-metadata.md) | Payment and agent metadata |
| [Roadmap](docs/roadmap.md) | Development phases |
| [Status](STATUS.md) | What works today |
| [Changelog](CHANGELOG.md) | Version history |

## Links

| Channel | Link |
|---------|------|
| Website | [x402cli.xyz](https://x402cli.xyz) |
| Demo API | [api.x402cli.xyz](https://api.x402cli.xyz) |
| Token ($X402CLI) | [Dexscreener](https://dexscreener.com/base/0x6fBEb18fc6Ab14b170EcfB21c9a2f2384b155bA3) |
| X (updates) | [@x402cli](https://x.com/x402cli) |
| GitHub | [louismaxdubois/x402cli](https://github.com/louismaxdubois/x402cli) |

Follow **[@x402cli on X](https://x.com/x402cli)** for development updates and announcements.

## Disclaimer

x402 CLI is an independent experimental project. It is not affiliated with Coinbase, Base, Coinbase Developer Platform, Tempo, Stripe, or any official x402, MCP, or MPP organization.

See [DISCLAIMER.md](DISCLAIMER.md) for the full notice.

## License

[MIT License](LICENSE)
