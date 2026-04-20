# CableLoop

Identify any cable in your drawer, then recycle, rehome, or list it in three steps.

**[Live demo](https://teamytastic.github.io/cableloop/)**

```bash
open index.html
```

Pick a cable type → rate its condition → get routed to a drop-off, mail-in kit, or doorstep pickup.

---

## Identify

Select from 13 cable types in a searchable grid: USB-C, HDMI, Lightning, VGA, Thunderbolt, and more. The grid filters as you type.

## Assess

Rate condition as working, damaged, or unknown. Working cables unlock the Cable Exchange path alongside recycling.

## Act

Three disposal routes appear based on condition:

| Route | When |
|-------|------|
| Drop-off locator | Any cable, any condition |
| Mail-in kit | Single cables, damaged welcome |
| Doorstep pickup | 10+ cables at once |

## Cable Exchange

Working cables surface in a community marketplace. List what you have and browse what others are offering. Exchange sits alongside recycling — not buried in a footer.

---

## Technical

- Zero dependencies — 1,849 lines of vanilla HTML/CSS/JS
- Copper/forest/cream palette: copper (#B87333) is literally what cables are made of
- Scroll reveal via `IntersectionObserver` with expo ease-out — settles quickly, no lingering
- Nav hides on scroll-down, reappears on scroll-up — CTA stays reachable

**Note:** This is a design prototype. The drop-off locator and pickup scheduler open a postcode modal with no backend. Exchange listings are static seed data.
