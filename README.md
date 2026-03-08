# CableLoop

> **When** you have a drawer full of cables you can't identify, **you want** a quick way to recycle or rehome them responsibly — **so you can** stop adding to the 2 million tonnes of e-waste generated every year.

Most recycling guides stop at "take it to a centre." They don't tell you which cable you're holding, whether it's worth passing on, or where to actually go. CableLoop fills that gap with a three-step flow: identify, assess, act.

**Live demo**: [teamytastic.github.io/cableloop](https://teamytastic.github.io/cableloop/)

---

## What It Does

A guided flow, not a wall of information:

1. **Identify** — Pick your cable type from a searchable grid (USB-C, HDMI, Lightning, VGA, Thunderbolt, and 8 others)
2. **Assess** — Rate its condition: working, damaged, or unknown
3. **Act** — Get routed to drop-off locations, a mail-in kit, or doorstep pickup (10+ cables)

Working cables surface in the **Cable Exchange** — a community marketplace where you list what you have and find what you need. The exchange sits alongside recycling, not as an afterthought.

---

## What Makes It Different

**The copper/forest palette earns its keep.** Copper (#B87333) against forest green (#1B4332) on cream (#F5F1E3) isn't arbitrary — copper is literally what cables are made of. The palette makes the sustainability angle feel material rather than greenwashed. The noise texture overlay (3% opacity SVG fractalNoise) keeps the cream background from feeling sterile.

**Scroll animations that don't overstay their welcome.** Sections fade in with `cubic-bezier(0.16, 1, 0.3, 1)` — an expo ease-out that settles quickly instead of lingering. The hero illustration uses `cubic-bezier(0.34, 1.56, 0.64, 1)` (ease-out-back) for a subtle overshoot that reads as physical. Neither animation calls attention to itself.

**The nav hides when you scroll down, reappears when you scroll up.** Standard pattern, but it matters on a long single-pager — you don't lose the primary CTA.

**IBM Plex Mono for stat figures.** The impact numbers (2.5M cables, 847t e-waste, 98% material recovery) render in monospace. On a page about hardware and infrastructure, it fits.

**Zero dependencies.** The entire site — cable grid, condition flow, exchange tabs, modal system, scroll observer — is 1,849 lines of vanilla HTML/CSS/JS. No bundler, no framework, no CDN besides Google Fonts.

---

## Tech Stack

| Layer | Choice |
|-------|--------|
| Framework | Vanilla HTML/CSS/JS — single `index.html` |
| Fonts | Outfit (display) + IBM Plex Mono (accents) via Google Fonts |
| Animations | CSS keyframes + IntersectionObserver for scroll reveal |
| Deployment | GitHub Pages |
| Dependencies | Zero |

---

## Run Locally

```bash
open index.html
```

No build step. No install. Open the file.

---

## Current State

This is a design exercise and concept prototype — not a live service. The cable identifier, condition flow, and exchange UI are fully interactive. The drop-off locator, mail-in kit, and pickup scheduler open a postcode modal (no backend). Exchange listings are seeded with static data.

---

*Last updated: 2026-03-08*
