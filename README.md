# presenta

Public, self-contained Marp deck for the c-lens team lightning talk (August 2026, ~15 minutes).

Single artefact: [`c-lens-lt.md`](./c-lens-lt.md). One optional asset: [`c-lens-hero.png`](./c-lens-hero.png) referenced as background on two slides.

No build step. No package.json. No co-author lines. Edit the markdown, view the result.

## What is this?

A Marp / Markdown slide deck that introduces c-lens, a small local Java CLI that reads IDE verbose logs and counts GitHub Copilot tokens locally with the same BPE the server uses. Audience: developers. Length: 13 slides, 15 minutes including a live terminal demo.

The deck goes from why this matters through architecture, installation, a hands-on demo break, two real-world scenarios, an IT-policy concerns-and-answers table, and a Q&A slide with links.

## Prerequisites

- VS Code (any recent version, 1.85+)
- Marp for VS Code extension by Marp Team, see marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode

Optional, for command-line export to PDF, HTML, PPTX:

- Node.js 18+
- @marp-team/marp-cli (install with npm install -g @marp-team/marp-cli or invoke ad-hoc with npx)

## Quick start

1. Clone the repository.

```bash
git clone https://github.com/dEMonaRE/presenta.git
cd presenta
```

2. Open `c-lens-lt.md` in VS Code.

3. Click the Marp preview icon in the top-right corner of the editor (or Ctrl+Shift+V then Ctrl+Shift+P and pick Marp: Open Preview). The deck renders live as you type.

4. To export to a shareable file, open the VS Code command palette (Ctrl+Shift+P) and run one of:

- Marp: Export Slide Deck (HTML)
- Marp: Export Slide Deck (PDF)
- Marp: Export Slide Deck (PPTX)

Exports land next to the source markdown file by default.

## Editing the slides

Frontmatter at the top of `c-lens-lt.md` controls theme, color, and layout:

```yaml
---
marp: true
theme: gaia
class: invert
paginate: true
size: 16:9
backgroundColor: "#0f1117"
color: "#e6e6e6"
---

Slide separators are three dashes (---) on their own line. Two blanks above and below keep things readable.

For full Marp syntax reference: marpit.org/marp.

## Files

| File | Purpose |
|------|---------|
| `c-lens-lt.md` | The deck. The only thing you edit. |
| `c-lens-hero.png` | Hero illustration, used as background on two slides. Replace freely with another 16:9 PNG (3200x1800 master recommended). |
| `README.md` | This file. |
| `.gitignore` | Standard ignore rules so local exports (*.pdf, *.html, *.pptx) never get committed. |

## Tip

If you generate a PDF or HTML export during a talk, drop the file in this folder and serve it from any static host. The deck is fully offline-capable. The only network round-trip Marp performs is theme CSS fetch on first open, then everything is cached.

## License

MIT.
