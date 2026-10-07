# Ultimate Tic-Tac-Toe

A single-page, self-contained build of Ultimate Tic-Tac-Toe — nine tic-tac-toe boards nested inside one big board. Win three small boards in a row to win the game.

No build step, no dependencies, no server. It's one HTML file you can open directly or host anywhere static files are served (GitHub Pages, Netlify, S3, etc.).

## How it works

- The big board is a 3×3 grid of small boards, each a 3×3 grid of cells.
- Whichever cell you play in sends your opponent to the same-position board next (e.g. play in the top-right cell of a board, and they must play in the top-right board).
- If that target board is already won or full, your opponent is free to play in any open board.
- Win three small boards in a row (horizontally, vertically, or diagonally) to win the game.

## Modes

- **2 players** — standard X vs. O turns.
- **2v2 teams** — two marks, two players per side, alternating: Team 1 → Team 2 → Team 1 → Team 2, so each side's players take turns on their team's mark.

## Customize

Open the **Customize** panel below the board to change:

- **Color theme** — 5 accent colors (Classic, Ocean, Forest, Berry, Mono), used for the active-board glow and highlights. Adapts automatically to light/dark mode.
- **Symbols** — each mark can be set to any of 11 emoji (⭕ ❌ 💧 🔥 🪨 🌀 ⚡ 🩸 💎 💥 ⭐). The two marks can't share a symbol — whichever one the other mark is using is greyed out in the picker.

## Running it

Just open `ultimate-tic-tac-toe.html` in a browser — no installation needed.

## Tech

Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build tools, no external JS dependencies. Fonts (Space Grotesk, Inter) are loaded from Google Fonts via CDN link tags.
