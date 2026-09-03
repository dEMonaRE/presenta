# presenta

## Decks

- [copilot-lens](./copilot-lens/copilot-lens-lt.md)

## Prerequisites

- VS Code (1.85+)
- Marp for VS Code extension by Marp Team: https://marketplace.visualstudio.com/items?itemName=marp-team.marp-vscode

Optional for CLI export:

- Node.js 18+
- @marp-team/marp-cli

Install with:

```bash
npm install -g @marp-team/marp-cli
```

## Presenting the deck

 The practical workflow is:

1. Open the deck file in VS Code, for example [copilot-lens/copilot-lens-lt.md](./copilot-lens/copilot-lens-lt.md).
2. Use the Marp preview button in the editor toolbar, or run `Marp: Open Preview` from the Command Palette.
```
  npx -y @marp-team/marp-cli copilot-lens-lt.md -o copilot-lens-lt.pdf
```
3. The preview renders the slide deck live while you edit.
4. To present, open that preview in a browser and switch the browser to full-screen mode. Then move between slides with arrow keys, Page Up/Page Down, or Space.
5. If you want a single shareable presentation file, use `Marp: Export Slide Deck (HTML)` or `Marp: Export Slide Deck (PDF)` and open the exported file in a browser.

In short: Marp does not add a separate PowerPoint-style presenter mode; the normal flow is preview in VS Code or browser, then present in browser full screen. That is the real equivalent of the PowerPoint slideshow experience.
