# Ramen Rush: The Great Ramen Festival 🍜

A fast, cute, single-file arcade game. Steer your bowl as **Rin**, catch the
good noodles, dodge the fish, grab power-ups, and fill your bowl across **8
festival stages** — win the **Golden Ladle**!

> No build step, no dependencies, no assets. One `index.html` — just open it
> in a browser and play. Works with keyboard, mouse, or touch.

## Play

Open `index.html` in any modern browser (or run a quick local server):

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

**Controls**
- `← →` / `A D` / mouse / finger — steer the bowl.
- `Space` / `Enter` — start, skip intro, pause.
- `P` — pause.

## The Festival (Story Mode)

Eight stages, each with its own flavor and rising difficulty:

| # | Stage | Twist |
|---|-------|-------|
| 1 | Shoyu Opening | warm-up crowd |
| 2 | Shio Breeze | a little faster |
| 3 | Miso Swirl | more hungry fish |
| 4 | Tonkotsu Rush | power-ups matter |
| 5 | Matsutake Mist | a fragrant slow… then it isn't |
| 6 | Spicy Firebreak | fast drops, lots of fish |
| 7 | Golden Hour | the crowd is on its feet |
| 8 | **GOLDEN LADLE** | the boss gauntlet 🏆 |

Fill the **bowl meter** before the clock hits zero. Miss too much or catch
too much fish and you lose a life. Clear all 8 to win the **Golden Ladle**.

## Endless Mode 🌊

No timer, no goal — just survive. The broth only gets faster, and the score
climbs in endless "levels." Beat your high score.

## Ingredients & Power-ups

- **Catch (good):** 🥚 🥩 🎍 🍄 🌸 🧅 🍜 🥕 — fill your bowl + score.
- **Dodge (bad):** 🐟 🪨 🕸️ 🧂 — cost a life.
- **Grab (power-ups):**
  - 🧲 **Magnet** — pulls good + power items toward you
  - ⏳ **Slow-Mo** — the broth slows down
  - 🛡️ **Shield** — blocks a bad hit (stacks to 2)
  - ✨ **2× Score** — double points
  - 🌊 **Big Broth** — wider catch zone
  - 🌈 **Rainbow** — 3× points for a few seconds

Chains build a **combo** multiplier; hitting a bad item resets it.

## Features

- 8-level story mode with per-stage story lines + a boss stage
- Endless mode with its own difficulty curve
- 6 power-ups, combos, score multipliers
- A **leaderboard** (top 5, with names) for each mode — stored locally in
  your browser (`localStorage`), no server needed
- Particles, confetti, screen shake, chiptune-style sound (Web Audio API)
- Responsive scaling + keyboard / mouse / touch input
- Zero dependencies, zero build — one file

## Project structure

```
.
├── index.html    # the entire game (HTML + CSS + JS, single file)
├── README.md
└── LICENSE
```

Everything lives in `index.html` on purpose: it's a toy, and it should be
trivial to open, share, and embed.

## License

MIT — see `LICENSE`.
