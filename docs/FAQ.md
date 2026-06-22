# FAQ

## Is x402 CLI usable today?

**Partially.** The website and demo API work for learning and exploration. The CLI package and real payment execution are not ready.

## Where is the live product?

- Website: [https://x402cli.xyz](https://x402cli.xyz)
- Demo API: [https://api.x402cli.xyz](https://api.x402cli.xyz)
- **Updates & progress: [https://x.com/x402cli](https://x.com/x402cli) (@x402cli)**

## Why isn't the website source on GitHub?

The deployable site runs on private hosting. This repo is the **public project hub** — docs, roadmap, and community — without publishing HTML/CSS source for trivial cloning.

## Is this an official Coinbase / Base project?

**No.** Independent experimental project. See [DISCLAIMER.md](docs/DISCLAIMER.md).

## Can I list my x402 API?

Submit form is a preview only. Backend coming in Phase 4. For early interest, open a GitHub Issue or contact [@x402cli](https://x.com/x402cli).

## When will the CLI be on npm?

No date committed. Follow this repo and the website changelog.

## Does the scanner make real HTTP requests?

Not yet. Homepage scanner is a **frontend mock**. Phase 2 adds real probing. Demo API at `api.x402cli.xyz` returns real 402 responses if you curl it directly.

## What stack does the website use?

HTML, CSS, Vanilla JavaScript, Apache `.htaccess`. No Node.js, React, or build step. See [ARCHITECTURE.md](docs/ARCHITECTURE.md).
