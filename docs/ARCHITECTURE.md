# Architecture Overview

High-level structure of the x402 CLI project. **Website source is hosted privately** — this document describes the system, not deployable files.

```
┌─────────────────────────────────────────────────────────────┐
│                     x402cli.xyz (website)                    │
│  Static HTML / CSS / JS · Apache · cPanel shared hosting   │
├─────────────────────────────────────────────────────────────┤
│  index      Landing, scanner mock, registry preview         │
│  docs       Documentation                                   │
│  commands   CLI command reference                           │
│  registry   API registry preview + filters                  │
│  submit     API submission form (frontend mock)             │
│  roadmap    Public roadmap                                  │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│               api.x402cli.xyz (demo API subdomain)           │
│  PHP · returns HTTP 402 + JSON payment requirements         │
├─────────────────────────────────────────────────────────────┤
│  /weather  /market  /agent  /content  /data                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼ (planned)
┌─────────────────────────────────────────────────────────────┐
│                   x402cli CLI (planned)                       │
│  Terminal tool · scan · inspect · registry · agent output    │
└─────────────────────────────────────────────────────────────┘
```

## Design principles

- **No build step** — vanilla HTML/CSS/JS for maximum shared-hosting compatibility
- **Frontend mock first** — validate UX before real endpoint probing
- **Developer-first** — terminal aesthetic, clear docs, agent-ready output (planned)
- **Honest scope** — experimental, not affiliated with Coinbase/Base

## Network & assets

| Layer | Technology |
|-------|------------|
| Website | HTML5, CSS3, Vanilla JS |
| Routing | Apache `.htaccess` clean URLs |
| Demo API | PHP 7.4+ |
| Chain | Base (planned payment research) |
| Asset | USDC |

## Security model (current)

- No user accounts
- No wallet integration on website
- Submit form does not POST to server
- Demo API returns 402 only — no payment execution

See [SECURITY.md](../SECURITY.md).
