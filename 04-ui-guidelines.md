# UI Guidelines

These patterns are already implemented in `freclean-website`, `freclean-admin`, and `freclean-dapp` — this document explains the reasoning so future work stays consistent, rather than each repo drifting independently.

## The "wipe" as a structural element, not decoration

The blue-to-green gradient (`02-color-system.md`) is used specifically for: section dividers, active-navigation indicators, and progress/status steppers. It should always mean "progress" or "structure" — never used purely decoratively, so it retains meaning when a user sees it.

## Status color language

One consistent color meaning is used everywhere a status appears (booking status, payment status, product lifecycle status):

| Meaning | Color | Example statuses |
|---|---|---|
| Positive / complete | Green | `confirmed`, `available`, `completed`, `verified` |
| In progress / neutral | Blue | `pending`, `requested`, `detected`, `assigned` |
| Caution / not yet real | Gold | `development`, `prototype`, `in_development`, `planned` |
| Negative | Red | `failed`, `expired`, `cancelled`, `discontinued` |

This mapping is implemented identically in `freclean-website`'s tag classes, `freclean-admin`'s `StatusBadge`, and `freclean-dapp`'s `StatusPill` / `PaymentStepper`. A new interface should reuse this mapping rather than invent a new one.

## Cards, radius, and shadow

- Border radius: 14px for cards, 999px (full pill) for buttons and tags.
- Cards: white background, 1px `Line` (`#D8E6E1`) border, no heavy drop shadow — FreClean's UI favors flat, high-contrast clarity over skeuomorphic depth.

## Accessibility baseline

- Every interactive element gets a visible focus state (3px Sun Gold outline — see `02-color-system.md`).
- Color is never the only signal for status — pair it with a text label (as in the status tables above), not a color dot alone.
- Reduced-motion is respected everywhere (`prefers-reduced-motion`) — already implemented in every front-end repo's global stylesheet.

## What not to do

- Don't design a new admin section or customer-facing page without checking this document and the existing component patterns in `freclean-admin`/`freclean-website` first.
- Don't invent a new status color meaning for a new feature — extend the existing four-color language instead.
