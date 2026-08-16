# Dust Lane

Pure Tower Defense prototype for the **Meta Horizon Creator Competition: Game Prototype** (Aug 17 – Sep 8, 2026).

**Genre:** Tower Defense & Strategy  
**Theme:** Vertical solar array / dust field  
**Tech:** Self-contained Three.js / HTML5, fixed portrait, no external network requests.

## Current Status
- Phase 1 complete: Playable foundation (lane, core, tower placement, enemies, restart)
- Phase 2 in progress: Core loop (scrap, costs, waves, win condition)

## How to run locally
```bash
cd dust-lane
python3 -m http.server 8765
```
Open `http://localhost:8765` in a portrait / mobile viewport.

## Constraints (enforced)
- Single-player
- Fixed portrait
- All game code in one readable `index.html`
- Libraries in `vendor/`
- Fully offline

See `BUILD_LOG.md` for the development record.
