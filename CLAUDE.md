# Minesweeper — CLAUDE.md

## What this is
Single-file 8×8 Minesweeper game. All code lives in `index.html` — HTML, CSS, and JS inline. No build step, no dependencies.

## Key files
- `index.html` — entire game (board logic + UI + styling)
- `README.md` — player-facing instructions

## Architecture
- Board: 2D array of cell objects `{ isMine, isRevealed, isFlagged, count }`
- Mine placement happens on first click (first-click safety — excludes clicked cell + neighbors)
- Flood-fill via BFS for empty cell regions
- Flag Mode toggle button for mobile; long-press also flags; right-click works on desktop
- Cell size is dynamic: `max(36px, (viewport - 32px) / 8)` — mobile responsive

## Hosted at
https://mannybarojas.github.io/minesweeper/

## Standards
- README.md required ✅
- CLAUDE.md required ✅
- GitHub Pages enabled ✅
- Mobile-friendly ✅
