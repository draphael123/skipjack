# SKIPJACK

*A small boat · a quiet sea · a hold full of maybes.*

A cozy fishing-and-delivery game — Dredge minus the horror. Sail a little lathed-hull
launch around a procedurally generated archipelago: hunt fish shadows in the shallows,
win the timing ring, Tetris your catch into the hold, run delivery contracts between
island villages, and upgrade the boat until the night sea opens up.

**The sea keeps secrets but never punishes.** No damage, no cargo loss, no fail states —
the worst thing that can happen is a smaller payout.

## Play

Static site — serve the folder any way you like:

```
python -m http.server 5777
```

| Key | Action |
|-----|--------|
| WASD / arrows | sail |
| E | dock / cast |
| Space | hook (timing ring) |
| Tab | hold (cargo grid) |
| C | codex |
| Esc | pause |
| M | mute |

## Notes

- Single-page Three.js (r160 via CDN); all game code lives in `index.html`.
- Audio in `audio/` is CC0 from [OpenGameArt](https://opengameart.org) — see `audio/CREDITS.txt`.
- Save lives in `localStorage`. Each new sea is a fresh seeded archipelago; weather,
  wind, and what's biting change daily. Some fish only bite in the rain, at night,
  over sand — the codex is a puzzle box.

Built with Claude.
