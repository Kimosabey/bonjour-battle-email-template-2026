# Bonjour Battle — registration email (2026)

Five design directions for the **Lingotran · Bonjour Battle Season 1** registration
email. Open the showcase, compare them at desktop and mobile, and pick one — we'll
then ship the production-ready, email-client-tested version of your choice.

## 🖼️ View the showcase

Once GitHub Pages is enabled (Settings → Pages → Source: `main` / root):

> **https://kimosabey.github.io/bonjour-battle-email-template-2026/**

Or open [`index.html`](index.html) locally in a browser.

## 🅰️–🅴 The directions

| | Direction | Feel |
|---|-----------|------|
| **A** | Editorial Light | Clean white layout with a coral top rule — calm, content-first. |
| **B** | Gradient Premium | Bold purple gradient hero — the most premium, branded feel. |
| **C** | Minimal Centered | Centered, cream, typographic — minimal with a big prize stat. |
| **D** | Dark Editorial | Dark plum theme — high-contrast and dramatic. |
| **E** | Event Ticket | Ticket-stub motif with perforation and a 3-column detail strip. |

**To decide:** reply with the letter (A–E) you want to ship.

## 📁 Structure

```
.
├── index.html      # Showcase gallery — desktop + mobile previews of all five (Pages entry)
├── emails/         # Self-contained sendable emails — pure HTML/CSS, no JavaScript
│   ├── a-editorial-light.html
│   ├── b-gradient-premium.html
│   ├── c-minimal-centered.html
│   ├── d-dark-editorial.html
│   └── e-event-ticket.html
├── source/         # Original design-canvas exports (.dc.html + support.js runtime)
└── reference/      # Brand guidelines + earlier template, for reference
```

## ℹ️ `emails/` vs `source/`

The `source/` `.dc.html` files are design-tool exports: they hide their own markup and
re-render it through React loaded from a CDN, so they appear **blank** without internet
or when opened via `file://`.

The `emails/` files are the same designs with that runtime stripped out — **pure HTML and
CSS**, nothing else. They render in any browser and any email client, and are the basis
for the production send.

---

© 2026 Lingotran Private Limited.
