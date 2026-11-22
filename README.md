# Nightshift Chess

A responsive personal chess tutor built from the V4 chess application and the approved Nightshift interface.

## Interfaces

- **Desktop:** fixed analysis workspace with the board and tutor panels visible together; persistent move-history and game-library dock.
- **Tablet:** landscape two-column board and analysis layout.
- **Phone:** bottom navigation for Board, Coach, Scan, Game and Library, with saved-game access in the Library tab.

## Chess functionality

The V4 game logic is retained, including practice/tutor and game modes, move hints, selectable sides and computer strength, candidate lines and prediction prompts, two-sided position scanning, resignation options, saved games, replay navigation, iteration branches, PGN export and post-game analysis.

The custom chess pieces are inline SVGs. The site loads chess.js and the Stockfish browser engine from their public CDNs.

## Game storage

Saved games and the local practice rating are stored in the browser on the current device. They are not automatically synchronised to GitHub or a cloud account. Export important games as PGN for a portable backup.

## Deployment

The Deploy Nightshift Chess to GitHub Pages workflow validates the required V4 interface elements and inline JavaScript, then publishes the root index.html with GitHub Pages whenever the app changes on main.

**One-time setup for a new repository:** open Settings → Pages → Build and deployment, set Source to **GitHub Actions**, and save. Then run the Deploy Nightshift Chess to GitHub Pages workflow from the Actions tab (or re-run the latest deployment). This first-time Pages activation is a repository setting and is not created by the workflow token.

Live site: https://thundercreast.github.io/chess101/
