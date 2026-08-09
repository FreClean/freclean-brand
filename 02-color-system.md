# Color System

These are the canonical FreClean brand colors. `freclean-website`, `freclean-admin`, and `freclean-dapp` are already built against these exact values — this document is the source of truth they were derived from; if a color needs to change, change it here first and propagate.

## Primary palette

| Name | Hex | Use |
|---|---|---|
| FreClean Blue | `#0B72B9` | Primary brand color, links, primary actions |
| FreClean Blue Deep | `#084F80` | Hover/pressed states, dark accents |
| FreClean Green | `#2FAE60` | Secondary brand color, success states, growth/entrepreneurship contexts |
| FreClean Green Deep | `#1F7A44` | Hover/pressed states |

## Supporting palette

| Name | Hex | Use |
|---|---|---|
| Sun Gold | `#F4B93F` | Single-action highlights, warnings, focus rings — used sparingly, never as a primary color |
| Ink | `#0F2A2E` | Primary text color |
| Ink Soft | `#5B7A77` / `#45605F` | Secondary text |
| Surface | `#F5F9F8` / `#F6FAF9` | Page background |
| Line | `#D8E6E1` | Borders, dividers |

## The signature gradient ("the wipe")

```css
background: linear-gradient(100deg, #0B72B9 0%, #2FAE60 100%);
```

A diagonal blue-to-green streak, used as the signature FreClean visual motif — section dividers on the website, active-state indicators in the admin sidebar, and the payment-status stepper in the dApp. It represents a cleaning wipe passing across a surface. Use it for accents and dividers, not as a full-page background — it loses impact if overused.

## Accessibility

- Body text uses Ink (`#0F2A2E`) on Surface (`#F5F9F8`/white) — passes WCAG AA for normal text.
- Never place Sun Gold text on a white background for body copy — insufficient contrast. Gold is for accents (badges, focus outlines, small highlights) only.
- Focus states use a 3px Sun Gold outline across every FreClean interface, for consistency and visibility.

## What not to do

- Don't introduce a new primary color without updating this document and every consuming repository.
- Don't use Celo's own brand yellow (`#FBCC5C`, used only in `freclean-dapp` for a Celo-specific badge) as a general FreClean accent color — it belongs to Celo, not FreClean.
