# EGA Trek (reconstruction)

A browser remake of **EGATrek**, Nels Anderson's 1988 shareware DOS game. EGATrek was itself one of the best PC versions of the 1971 mainframe *Star Trek* game. This remake keeps the 16-color EGA look, the typed command console and the turn-based tactics.

The whole game is one self-contained `index.html` with no dependencies and no build step. It runs offline because the font is embedded in the page.

## Play

- **Locally:** open `index.html` in any modern browser.
- **GitHub Pages:** in the repo, go to *Settings → Pages*, set the source to the `main` branch at `/ (root)`, and the game will be served at `https://<user>.github.io/EGAtrek/`.

## Mission

You command the starship ENDEAVOR. Krellan invaders are spread through an 8×8 galaxy of quadrants, and each quadrant is an 8×8 grid of sectors. You have to destroy all of them before the stardate deadline. Along the way you protect your starbases, answer distress calls and try not to blow up anything friendly.

## Commands

Commands can be shortened to their first letter. Coordinates are given as column, then row, from 1 to 8.

| Command | Action |
|---|---|
| `M x y` | Move by impulse to a sector in this quadrant |
| `W x y` | Warp to another quadrant (costs energy and time) |
| `P n` | Fire phasers with *n* energy, split across all enemies (strength falls off with distance) |
| `T x y` | Fire a photon torpedo at a sector (`T` alone locks onto the nearest enemy while the computer works) |
| `S n` | Set shields to *n* (the energy comes from your reserves) |
| `D` | Dock at an adjacent starbase to refuel, rearm and repair |
| `O` | Orbit an adjacent planet to mine dilithium for energy |
| `L` | Long-range scan of the surrounding quadrants |
| `R n` | Rest *n* days to repair and recharge (only when no enemies are present) |
| `X` | Fire the experimental death ray (can backfire) |
| `H` / `?` | Show help |
| `Q` / `N` | Quit / start a new game |
| `Esc` | Boss key |

If you type a command without its arguments, the game prompts you for them. Clicking a sector or a galaxy-chart cell adds its coordinates to the command you are typing. The up and down arrow keys scroll through your command history.

## Features

- Five skill levels, from Ensign to Admiral
- Three enemy classes: Raiders, Cruisers and Warlords. Warlords roam between quadrants and besiege starbases.
- Distress calls from starbases under siege and from freighters under attack. Reach them before the deadline for bonus points.
- A torpedo that hits a star can set off a nova, and novas can chain from star to star.
- Black holes throw your ship to a random quadrant.
- Eight ship systems that can be damaged, each with its own effect: warp, impulse, phasers, torpedoes, shields, short-range sensors, long-range sensors and computer
- A score breakdown and a rating at the end of the game

## Credits

- The original EGATrek is © Nels Anderson / Arcanum Computing. This project is an independent fan reconstruction written from scratch. It contains no original code or assets and uses its own names.
- The VT323 font is by Peter Hull and is used under the SIL Open Font License 1.1 (see `fonts/OFL.txt`).

## License

The game code is under the MIT License (see `LICENSE`). The font is under the OFL.
