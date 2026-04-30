# TA prep slide deck

## Framework and hosting

| Choice | Decision |
|--------|----------|
| **Slide engine** | **Reveal.js 4.x** (CDN) — keyboard navigation, optional speaker notes, `?print-pdf` for print/PDF. |
| **Alternate** | Plain scroll/print deck in [`../docs/slides.html`](../docs/slides.html) (no JS dependency). |
| **Local use** | Open [`index.html`](index.html) in a browser (double-click or Live Server). Internet required once for CDN assets. |
| **Optional hosting** | Push this repo (or a copy of `slides/`) to GitHub and deploy on **Vercel** with framework **Other** / static root containing `index.html` — same pattern as the student assignment. |

## Print to PDF (Reveal)

1. Open `index.html?print-pdf` in **Chrome** or **Edge** (recommended for Reveal’s print layout).
2. Print → Save as PDF.

## Related docs (repo)

- [`../docs/deck-outline.md`](../docs/deck-outline.md) — locked slide order
- [`../docs/vercel-walkthrough-script.md`](../docs/vercel-walkthrough-script.md) — ~2–3 min deploy narration
- [`../docs/live-cobuild-prompt.md`](../docs/live-cobuild-prompt.md) — toy page Cursor prompt + fallback

## Files

- `index.html` — slide markup + Reveal init
- `css/theme.css` — course-adjacent accent and readability overrides
