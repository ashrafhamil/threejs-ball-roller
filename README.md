# Ball Roller

A small Three.js physics game. Roll a ball down sloped platforms, over hills, across gaps to the green goal pad. 8 levels of increasing difficulty.

**Play:** open `index.html` in any browser, or the deployed URL.

## Controls
- **WASD / Arrows** — roll
- **SPACE** — jump (on ground) / start / next level
- **R** — restart level

## Mechanics
- Discrete platforms with per-platform slope (`sx`, `sz`) — gravity is projected along the incline, so the ball accelerates downhill and slows uphill.
- Optional gaussian **hills** (`bumps`) displace the platform surface; physics follows the real surface normal.
- Banked ramps drift the ball sideways; gaps must be jumped; dog-leg turns must be steered.

## Levels
1. Narrow winding descent + 90° dog-leg
2. Up-ramp → crest (with a mound) → jump the gap → goal
3. Steep banked S-drop → jump up to elevated goal
4. Double dog-leg zigzag with rolling mounds
5. Opposite banked drops (S-drift) into a sunken goal
6. Jump gauntlet — precision hops across gaps onto small pads (one domed)
7. Narrow banked drift + big gap + dog-leg turn
8. Final — steepest, narrowest, banked both ways, bumps, multi-jump climb to peak

## Stack
Single static `index.html`. Three.js 0.160 via CDN import map. No build step.
