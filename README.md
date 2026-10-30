# Gearslinger 🤠

A juicy top-down 3D shooter: a steampunk cowboy with a six-shooter versus waves of clockwork robots in the desert.
Built with three.js as a single static page: no build step, and all sound effects are synthesized live.

## Play
Open `index.html` in a browser (needs internet for the three.js CDN), or visit the GitHub Pages site.

| Action | Keyboard / mouse | Gamepad |
|---|---|---|
| Move | WASD / arrows | Left stick |
| Aim | Mouse | Right stick |
| Shoot (hold) | Left click | RT |
| Steam dash (brief invulnerability) | Space / Shift | A / LB |
| Reload | R (automatic when empty) | X |
| Spin shot | E / right click | B / RB / LT |
| Pause · mute | Esc · M | Start |

## Enemies
- **Scuttler**: fast clockwork scorpion. Twitches, then lunges.
- **Tin Bandit**: keeps its distance, shows a red aim line, then fires slow shots. You can shoot its bullets out of the air.
- **Boilerback**: big steam brute. Hisses and glows, then charges. If it hits a wall or rock it gets stunned. Explodes when destroyed.

## Pickups
- **Twin Revolvers** (15s): a second gun in the other hand
- **Boom Rounds** (12s): bullets explode on impact
- **Pierce Rounds** (12s): bullets go through up to 4 enemies
- **Ricochet** (12s): bullets bounce off walls and rocks up to 3 times
- **Buckshot** (12s): every shot fires a 3-bullet spread
- **Steam Overdrive** (8s): double fire rate, no reloading
- **Brass Plating**: blocks one hit
- **Spin Shot** charge (max 3) · **Snake-oil Tonic** (+1 heart)

Timed powers stack. Crates and red steam tanks are destructible, and tanks chain-explode.

## Dev flags
- `?bot`: autopilot plays the game
- `?wave=N`: start at wave N
- `?sim=N`: fast-forward N seconds on load (for headless screenshots)
- `?pose`: line up every enemy and pickup next to the player
- `?give=pierce,rico,...`: start with these pickups
- `?touch`: force the touch layout

## GitHub Pages
Settings → Pages → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)`.
