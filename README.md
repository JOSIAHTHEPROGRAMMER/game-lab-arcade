# Game Lab Arcade

A collection of five browser-based HTML5 games, built as student projects, with a single landing page (`index.html`) that links out to all of them.

**[Play it live](#deploying-to-github-pages)** once deployed, or just open `index.html` in a browser.

## The games

| Game               | File                      | Genre                              |
| ------------------ | ------------------------- | ---------------------------------- |
| **Trap Dungeon67** | `dungoun-adventures.html` | 2D action-platformer / bullet hell |
| **Hungry Rabbit**  | `hungry-rabbit.html`      | Asymmetric horror                  |
| **Pixel Fury**     | `pixel-fury.html`         | 1v1 fighting game                  |
| **Color Chaos**    | `color-chaos.html`        | 2D territory shooter               |
| **F3 Racing 2026** | `f3-racing-2026.html`     | Arcade racing                      |

### Trap Dungeon67

A one-life, one-hit dungeon crawler inspired by _Trap Dungeon 2_ and _Metal Slug_. Fight through spike traps, rolling boulders, and chainsaws to reach a two-phase bullet-hell boss at the end of each level. Combat is fluid and mid-air, closer to _Dead Cells_ than a stiff platformer.

- **Controls:** WASD to move/jump/duck, Q for consumables, E for abilities, R to reload

### Hungry Rabbit

An experiment goes wrong in a research lab, and an infected rabbit turns violent. Choose a side: play as the rabbit hunting scientists through the lab, or as a scientist trying to neutralize or hide from it. Rounds run on a timer with stamina management, cloning, and emergency backup calls.

- **Controls:** Arrow keys to move, Space for your special ability (attack or chemical defense)

### Pixel Fury

A one-on-one fighting game in the tradition of _Street Fighter 2_ — countdown, "FIGHT," scrolling arena, and a full punch/kick/block moveset with a victory pose to close out the match.

- **Controls:** Player 1 — Arrow keys to move, 1/2/3 to punch/kick/block. Player 2 — WASD to move, U/I/O to punch/kick/block

### Color Chaos

A 2D, _Splatoon_-inspired shooter. Pick a color, cover the map in it, and hold more territory than the other player when time runs out.

- **Controls:** Player 1 — Arrow keys to aim, N/M to shoot. Player 2 — WASD to aim, Z/X to shoot

### F3 Racing 2026

Pixel-art formula racing with pit stops and retro NPC mechanics, blending _F1_-style handling with _Mario Kart_-style power-ups. Built for local multiplayer, three laps per race.

- **Controls:** WASD to drive, B for power-ups

## Running locally

No build step or server required — these are static HTML files.

1. Clone the repo:
   ```bash
   git clone https://github.com/JOSIAHTHEPROGRAMMER/game-lab-arcade.git
   cd game-lab-arcade
   ```
2. Open `index.html` in a browser (double-click it, or right-click → Open With → your browser).
3. From the hub page, click into any game.

If a game needs to load its own assets (images, sound files, etc.) via `fetch`, some browsers block that over a plain `file://` link. If a game looks broken when opened directly, serve the folder locally instead:

```bash
python3 -m http.server 8000
```

then visit `http://localhost:8000` in your browser.

## Deploying to GitHub Pages

1. Push this folder to a GitHub repository, with `index.html` and all five game files at the repo root (or in a `docs/` folder — see below).
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Pick the branch (usually `main`) and the folder (`/root` or `/docs`), then **Save**.
5. GitHub will give you a URL shortly after:
   ```
   https://josiahtheprogrammer.github.io/game-lab-arcade/
   ```
6. That URL loads `index.html` automatically, so the arcade hub becomes your homepage with links to every game.

## Project structure

```
.
├── index.html              # Arcade hub — links to all five games
├── dungoun-adventures.html # Trap Dungeon67
├── hungry-rabbit.html      # Hungry Rabbit
├── pixel-fury.html         # Pixel Fury
├── color-chaos.html        # Color Chaos
├── f3-racing-2026.html     # F3 Racing 2026
└── README.md
```

## Credits

Built as student projects. Add your name(s) and course/class info here.
