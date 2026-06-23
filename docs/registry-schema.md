# Registry Schema

x402 CLI v0.3 registry entries use a structured metadata schema for documenting x402-powered APIs.

## Core fields

| Field | Description |
|-------|-------------|
| `id` | Stable registry identifier (e.g. `weather-api`) |
| `name` | Human-readable API name |
| `category` | Data, Finance, AI Agent, Content, etc. |
| `endpoint` | HTTPS endpoint URL |
| `network` | Payment network (e.g. `base`) |
| `asset` | Payment asset (e.g. `USDC`) |
| `price` | Per-request price string |
| `paymentProtocol` | e.g. `x402` |
| `mcpReady` | `demo`, `planned`, or research status |
| `builderCode` | Builder Code attribution status |
| `attributionStandard` | e.g. ERC-8021 research |
| `status` | e.g. `demo` |
| `description` | Short API description |

## Example entry

```json
{
  "id": "weather-api",
  "name": "Weather API",
  "category": "Data",
  "endpoint": "https://api.x402cli.xyz/weather",
  "network": "base",
  "asset": "USDC",
  "price": "0.001",
  "paymentProtocol": "x402",
  "mcpReady": "demo",
  "builderCode": "planned",
  "attributionStandard": "ERC-8021 research",
  "status": "demo",
  "description": "Example paid weather endpoint using HTTP 402."
}
```

## Public registry export

Full demo export: [examples/registry.json](../examples/registry.json)

See also: [Registry Metadata Layer](registry-metadata-layer.md) · [API Detail Pages](api-detail-pages.md)

Builder Code fields are research/planned metadata only. x402 CLI does not attach Builder Codes to real settlement transactions.

See also: [Builder Codes Research](builder-codes.md)
