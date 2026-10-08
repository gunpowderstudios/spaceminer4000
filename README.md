# Space Miner 4000

A small retro vector browser game: **FLY → LAND → MINE → UPGRADE → ESCAPE → REPEAT** across five planets.

Play: https://gunpowderstudios.github.io/spaceminer4000/

## Controls
| Phase | Controls |
|---|---|
| Flight / Lander / Escape | ◀ ▶ rotate · ▲ thrust · Space / ● fire (flight) |
| Surface | ◀ ▶ walk · ▲ jump · Space / ● fire |
| Upgrade | ↑ ↓ select · Space buy · Enter launch · or tap |

## v0.8.0 — "Fair, Feel & Flow"
- Fixed 60 Hz timestep: same speed on 60/120/144 Hz screens
- Invulnerability frames + single `damage()` — no more 2–3 hull lost to one rock
- Difficulty no longer depends on screen width (flight timed in seconds, cavern gap in fixed units)
- Flight: ~36–48 s trip with progress bar, rocks arrive in waves, flying forward gets you there sooner, gold ore rocks drop gems, gas rings now +6 fuel
- Lander: pad off to one side, rough terrain, pad shrinks per planet, green/red readouts, altitude, out of fuel = engine dead, top boundary
- Surface: start beside your ship, shoot ore to crack out gems, facing direction, O₂ timer replaces hidden fuel drain, exit hint
- Escape: new cavern per planet (seeded), longer on later planets, rising lava
- Upgrades: Refuel option, laser now helps in space, keyboard support, matching hitboxes, proper launch button, no score for buying, new ship no longer shows damage
- Feel: screen shake, engine particles, continuous thrust sound, low-fuel / O₂ alarms, landing chime, pad beacons
- Fixes: held key no longer skips game-over screen, safe localStorage, cavern explosion draws the cavern, aliens stay in bounds, surface particles in world space
- Tracks furthest planet reached
