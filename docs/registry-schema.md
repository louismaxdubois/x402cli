# Registry Schema

This schema describes how x402 CLI may represent x402-powered APIs inside the registry preview.

```json
{
  "name": "Weather API",
  "category": "Data",
  "endpoint": "https://api.example.com/weather",
  "network": "base",
  "asset": "USDC",
  "price": "0.001",
  "paymentProtocol": "x402",
  "mcpReady": "demo",
  "status": "demo",
  "description": "Example paid weather endpoint using HTTP 402."
}
```

## Fields

| Field | Type | Description |
|-------|------|-------------|
| `name` | string | Display name of the API |
| `category` | string | Category (Data, Finance, AI Agent, Content, etc.) |
| `endpoint` | string | API base URL |
| `network` | string | Blockchain network (e.g. `base`) |
| `asset` | string | Payment asset (e.g. `USDC`) |
| `price` | string | Price per request |
| `paymentProtocol` | string | Payment protocol (e.g. `x402`) |
| `mcpReady` | string | MCP readiness: `demo`, `planned`, or `not yet` |
| `status` | string | Entry status (e.g. `demo`) |
| `description` | string | Short description |

## Example file

See [examples/registry-schema.json](../examples/registry-schema.json).
