# API Reference — api.x402cli.xyz

Demo HTTP 402 endpoints for x402 CLI. **Not a real payment processor.**

Base URL: `https://api.x402cli.xyz`

## Gateway info

```http
GET /
```

Returns JSON listing available demo endpoints.

---

## Payment endpoints

All return **HTTP 402** with x402-style JSON body.

| Endpoint | Price | Category |
|----------|-------|----------|
| `GET /weather` | 0.001 USDC | Data |
| `GET /market` | 0.002 USDC | Finance |
| `GET /agent` | 0.005 USDC | AI Agent |
| `GET /content` | 0.001 USDC | Content |
| `GET /data` | 0.001 USDC | Data |

### Example

```bash
curl -i https://api.x402cli.xyz/weather
```

```json
{
  "x402Version": 1,
  "error": "Payment Required",
  "accepts": [{
    "scheme": "exact",
    "network": "base",
    "maxAmountRequired": "1000",
    "resource": "https://api.x402cli.xyz/weather",
    "asset": "USDC"
  }]
}
```

Amount `1000` = 0.001 USDC (6 decimals).

---

## Notes

- `payTo` address is a placeholder (`0x000...000`)
- Deployed separately on subdomain document root
- Website scanner mock does not call these endpoints yet (Phase 2)
