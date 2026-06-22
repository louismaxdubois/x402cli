# Commands Reference

> The installable CLI package is **planned**. Commands below describe intended behavior. Preview scan output on the [website scanner](https://x402cli.xyz/#live-terminal-demo).

## x402cli scan \<url\>

Probe an API endpoint and detect HTTP 402 Payment Required responses.

```bash
x402cli scan https://api.x402cli.xyz/weather
```

**Expected output (summary):**

```
402 Payment Required detected
Network: Base
Asset: USDC
Price: 0.001 USDC
Resource: /weather
Mode: x402
```

---

## x402cli inspect \<url\>

Parse full x402 payment requirement fields from a 402 response.

```bash
x402cli inspect https://api.x402cli.xyz/weather
```

**Fields parsed:**

- HTTP status
- Payment network, asset, amount, scheme
- Resource URL and payTo address

---

## x402cli registry

List x402-compatible APIs from the public registry.

```bash
x402cli registry
```

Browse the [registry preview](https://x402cli.xyz/registry) on the web.

---

## x402cli demo

Run a step-by-step simulation of the payment retry flow. **No real payment is executed.**

```bash
x402cli demo
```

---

## Current status

| Command | CLI | Web preview |
|---------|-----|-------------|
| `scan` | Planned | Scanner mock on homepage |
| `inspect` | Planned | Command preview tab |
| `registry` | Planned | Registry page |
| `demo` | Planned | Not linked publicly |
