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
  "builderCode": "planned",
  "attributionStandard": "ERC-8021 Schema 2 research",
  "status": "demo",
  "description": "Example paid weather endpoint using HTTP 402."
}
```

Builder Code fields are research/planned metadata only. x402 CLI does not attach Builder Codes to real settlement transactions.

See also: [Builder Codes Research](builder-codes.md)
