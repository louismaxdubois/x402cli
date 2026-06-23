# API Metadata

x402 CLI documents payment and agent-oriented metadata for x402-powered APIs.

## HTTP 402 response metadata

When an endpoint returns HTTP 402, useful fields include:

| Field | Description |
|-------|-------------|
| `protocol` | Payment protocol (e.g. `x402`) |
| `network` | Target network (e.g. `base`) |
| `asset` | Payment asset (e.g. `USDC`) |
| `amount` | Price per request |
| `resource` | Protected resource path |
| `description` | Human-readable note |

Example: [examples/x402-response-example.json](../examples/x402-response-example.json)

## MCP-ready metadata

For future agent workflows, APIs may include additional fields:

| Field | Description |
|-------|-------------|
| `toolName` | Agent tool display name |
| `category` | Tool category |
| `payment` | Nested payment requirements |
| `mcpReady` | Readiness status (`demo`, `planned`, etc.) |
| `status` | Documentation status |

Example: [examples/mcp-metadata-example.json](../examples/mcp-metadata-example.json)

## Registry schema

Full registry entry schema: [registry-schema.md](registry-schema.md)

## Demo API

Sample 402 responses are available at [api.x402cli.xyz](https://api.x402cli.xyz).
