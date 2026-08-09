# Typography

## Type system

| Role | Typeface | Used for |
|---|---|---|
| Display | Space Grotesk (500/600/700) | Headings, logo wordmark pairing, section titles |
| Body | Inter (400/500/600) | Paragraph text, UI labels |
| Data / technical | IBM Plex Mono (500) | SKUs, wallet addresses, transaction hashes, status codes, timestamps |

All three are free, open-license Google Fonts — no licensing cost or restriction blocks their use anywhere, including print.

## Why this pairing

Space Grotesk gives FreClean's headings a modern, slightly technical character appropriate to a company that's both a physical service business and a Web3 payments adopter, without tipping into generic "AI product" branding. Inter is a highly legible, neutral workhorse for body text. IBM Plex Mono marks anything data-like (a SKU, a transaction hash) so it's visually distinct from prose — this is already in active use across `freclean-website`, `freclean-admin`, and `freclean-dapp`.

## Scale (digital)

| Element | Size | Weight |
|---|---|---|
| H1 | 34–54px (responsive) | 700 |
| H2 | 24–28px | 700 |
| H3 | 17–19px | 600 |
| Body | 16px | 400 |
| Small / label | 13–14px | 500 |
| Mono / data | 13–14px | 500 |

## Print

For printed materials (packaging, business cards, letterhead — see `templates/`), use the same three-typeface system. If a print vendor cannot source Space Grotesk, Montserrat is an acceptable substitute for headings only — never substitute the body or mono faces.

## What not to do

- Don't introduce a fourth typeface without a specific, documented reason.
- Don't use the mono face for body prose — it's reserved for data.
- Don't set the logo wordmark in live text using these fonts as a substitute for the actual logo file — see `01-logo-usage.md`.
