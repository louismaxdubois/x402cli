# Commands

The installable CLI package is **planned** — not published yet.

The current public version provides a web-based terminal simulation, documentation, registry preview, and schema exploration at [x402cli.xyz](https://x402cli.xyz).

## Planned commands

### `x402cli scan <url>`

Scan an endpoint and inspect possible HTTP 402 payment requirements.

Example output: [examples/scan-output.txt](../examples/scan-output.txt)

### `x402cli inspect <url>`

Display x402 metadata, payment requirements, network, asset, and resource info.

Example output: [examples/inspect-output.txt](../examples/inspect-output.txt)

### `x402cli registry`

Browse indexed x402-compatible APIs.

Example: [examples/registry.json](../examples/registry.json)

### `x402cli registry export`

Export registry metadata as JSON for indexed x402 APIs.

### `x402cli registry inspect <api-id>`

Inspect detailed metadata for a listed x402 API.

Example: [examples/weather-api-detail.json](../examples/weather-api-detail.json)

### `x402cli mcp <api>`

Preview how an API could be documented for future MCP-ready agent workflows.

### `x402cli builder-code <api>`

Preview Builder Code attribution metadata for an indexed x402 API. ERC-8021 / settlement integration is research/planned.

Example: [examples/builder-code-metadata-example.json](../examples/builder-code-metadata-example.json)

### `x402cli demo`

Run a simulated x402 flow.

Example output: [examples/demo-flow.txt](../examples/demo-flow.txt)

## Status

| Command | Status |
|---------|--------|
| `scan` | Planned (web simulation only) |
| `inspect` | Planned (web simulation only) |
| `registry` | Planned (web preview only) |
| `registry export` | Planned |
| `registry inspect` | Planned |
| `mcp` | Planned (research) |
| `builder-code` | Planned (research) |
| `demo` | Planned (web simulation only) |
