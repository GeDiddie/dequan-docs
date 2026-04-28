# Dequan Docs (Mintlify)

Public-facing product documentation for [Dequan](https://snipe.dequan.xyz). Built with [Mintlify](https://mintlify.com/).

## Local preview

```bash
cd docs-site
npx mintlify dev
```

Opens a local preview at `http://localhost:3000`. Hot-reloads on file changes.

If `mintlify` is not installed globally:

```bash
npm i -g mintlify
mintlify dev
```

## Structure

- `docs.json` — Mintlify config (theme, navigation, branding, anchors)
- `index.mdx` — landing page
- `quickstart.mdx`, `what-makes-dequan-different.mdx` — Welcome group
- `pump-zone/` — six pages on the spatial discovery surface
- `charts/` — chart engines, TQS, token detail tabs
- `execution/` — pre-warmup, adaptive fees/slippage, parallel landing, Lightning Wallet, Fast Mode
- `safety/` — non-custodial, honeypot, drain detection, surveillance, fees, key handling, anti-abuse
- `toolbox/` — wallet utilities (Burn Barrel)
- `tiers/` — Scout (free), Sniper, Apex (invite only)
- `referrals/` — program overview + payout mechanics
- `reliability/` — health indicators, latency transparency
- `resources/` — FAQ, glossary, changelog
- `logo/` — site logos (light/dark SVG)
- `favicon.svg` — browser tab favicon

## IP-safety rules for editing

This site is **publicly accessible**. When adding or editing pages, **never** include:

- Internal file paths or function names
- Specific cache TTLs, thresholds, or magic numbers
- Specific port numbers or service URLs (other than the public app)
- KMS key IDs or any infrastructure secrets
- Competitor names by name
- Exact algorithm formulas or weighting schemes

Frame all content as **user-facing capability** — what the user can do, see, or rely on — not implementation detail.

## Deployment

Mintlify supports two deployment modes:

1. **GitHub integration** — push to a connected repo; Mintlify auto-builds and serves.
2. **CLI deploy** — `mintlify deploy` from this directory after configuring credentials.

See the [Mintlify deploy docs](https://mintlify.com/docs/quickstart#deploying-your-changes) for current instructions.

## Brand

- **Primary cyan:** `#22D3EE`
- **Light cyan:** `#67E8F9`
- **Dark cyan:** `#0E7490`
- **Theme:** Maple
- **Voice:** Confident, technical, grounded. No marketing fluff. Show evidence, name trade-offs, give numbers when honest, admit limits when honest.
