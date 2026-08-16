# Dust Lane – Build Log

**Competition:** Meta Horizon Creator Competition – Game Prototype  
**Genre:** Tower Defense & Strategy  
**Approach:** Pure Dust Lane (vertical solar/dust lane)  
**AI Tool:** Grok (xAI)

---

## Session 1 – 2026-08-16

### Decisions locked
- Genre: Pure Tower Defense (no hybrid systems)
- Theme: Vertical solar array / dust field
- Core loop: Place defenses → survive escalating waves → earn scrap → upgrade/place more
- Constraints enforced from day one: single-player, fixed portrait, fully self-contained, single readable index.html, vendor/ for libraries

### Phase 1 completed
**Goal:** Playable foundation

What was built:
- Fixed portrait canvas (phone-shaped)
- Vertical lane visual + core at bottom
- One basic tower type that can be placed by tapping the lane
- Enemies spawn at top and move toward the core
- Towers deal damage to enemies in range
- Core takes damage and is destroyed → game over + restart
- Basic UI (core health, status text, restart)
- Three.js loaded from local vendor/ folder
- No external network requests

**Playable result:** Player can place towers, watch enemies path down the lane, see the core take damage, and restart when the core is destroyed.

---

## Session 2 – 2026-08-16 (continued)

### Phase 2 completed
**Goal:** Core loop with economy, waves, win/lose

What was added:
- Scrap currency (start with 40, +8 per kill, +15 inter-wave bonus)
- Tower cost = 25 scrap (placement is now a real decision)
- 6 distinct waves with escalation (more enemies, faster spawn)
- Clear win condition (survive all 6 waves)
- Wave counter and scrap display in top bar
- Proper restart that resets economy and waves

**Playable result:** Full place → survive wave → earn scrap → place more → next wave loop works end-to-end. Player can win or lose a complete session.

### GitHub
- Repository created: https://github.com/Mototown/dust
- README and BUILD_LOG pushed

### Next
Phase 3 – Tower variety (3–4 distinct roles) + stronger visual/audio feedback.
