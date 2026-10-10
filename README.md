# Ultimate Tic-Tac-Toe

A single-page, self-contained build of Ultimate Tic-Tac-Toe — nine tic-tac-toe boards nested inside one big board. Win three small boards in a row to win the game.

No build step, no dependencies, no server. It's one HTML file you can open directly or host anywhere static files are served (GitHub Pages, Netlify, S3, etc.).

## How it works

- The big board is a 3×3 grid of small boards, each a 3×3 grid of cells.
- Whichever cell you play in sends your opponent to the same-position board next (e.g. play in the top-right cell of a board, and they must play in the top-right board).
- If that target board is already won or full, your opponent is free to play in any open board.
- Win three small boards in a row (horizontally, vertically, or diagonally) to win the game. The winning line pulses and the rest of the board dims.

## Modes

- **2 players** — standard two-mark turns.
- **2v2 teams** — two teams of two, turns alternate Team 1 Player 1 → Team 2 Player 1 → Team 1 Player 2 → Team 2 Player 2. Either teammate's move counts as a move for their team's mark.

## Customise

Open the **Customise** panel below the board to change:

- **Colour theme** — 5 accent colours (Classic, Ocean, Forest, Berry, Mono), used for the active-board glow and highlights. Adapts automatically to light/dark mode.
- **Names** (2-player mode) — rename each player; shown in the status line (e.g. "⭕ Alice to move"). Leaving a field blank falls back to "Player 1" / "Player 2".
- **Symbols** (2-player mode) — each mark can be set to any of 11 emoji (⭕ ❌ 💧 🔥 🪨 🌀 ⚡ 🩸 💎 💥 ⭐). The two marks can't share a symbol — whichever one the other mark is using is greyed out in the picker.
- **Team setup** (2v2 mode) — each team picks a **colour family** (Red, Orange, Yellow, Green, Blue, or Purple), and the two teammates then each pick their own emoji from *within* that family, so every symbol on their side is naturally the right colour — no colour tinting involved, just curated sets of emoji that are already that colour. The two teams can't pick the same colour family. Each team and each of its two players can also be renamed.

## Running it

Just open `ultimate-tic-tac-toe.html` in a browser — no installation needed.

### Hosting on GitHub Pages

1. Put `ultimate-tic-tac-toe.html` in your repo (rename to `index.html` if you want it at the root of your Pages site).
2. Enable GitHub Pages for the repo (Settings → Pages → choose a branch/folder).
3. Visit the published URL.

## Tech

Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build tools, no external JS dependencies. Inter is loaded from Google Fonts for body text; headings use Consolas (falling back to Menlo/Monaco/Courier New/monospace on non-Windows systems).
