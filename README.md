# Dust Lane

Pure Tower Defense prototype for the **Meta Horizon Creator Competition: Game Prototype** (Aug 17 – Sep 8, 2026).

**Genre:** Tower Defense & Strategy  
**Theme:** Vertical solar array / dust field  
**Tech:** Self-contained Three.js / HTML5, fixed portrait, no external network requests.

## Current Status
- ✅ Phase 1 complete: Playable foundation (lane, core, tower placement, enemies, restart)
- ✅ Phase 2 complete: Core loop (scrap economy, tower cost, 6 escalating waves, win/lose conditions)

## How to run locally
```bash
# Clone or download the files, then:
python3 -m http.server 8765
```
Open `http://localhost:8765` in a portrait / mobile viewport (or narrow browser window).

**Required local files for full run:**
- `index.html` (all game code)
- `vendor/three.min.js` (Three.js r160)

You can download Three.js with:
```bash
mkdir -p vendor
curl -L -o vendor/three.min.js https://cdn.jsdelivr.net/npm/three@0.160.0/build/three.min.js
```

## Constraints (enforced)
- Single-player
- Fixed portrait
- All game code in one readable `index.html`
- Libraries in `vendor/`
- Fully offline / no network requests while running

See `BUILD_LOG.md` for the full development record.

## Next
Phase 3: Multiple distinct tower types + stronger feedback.
