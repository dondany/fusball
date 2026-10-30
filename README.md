# Gearslinger 🤠

A juicy top-down 3D roguelike shooter: a steampunk cowboy with a six-shooter versus waves of clockwork robots in the desert.
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

## The run
- **Draft:** after every wave, pick 1 of 3 permanent upgrade cards (common / rare / legendary). Rerolling costs scrap.
- **Scrap:** brass cogs burst out of wrecked robots and crates. Walk near them, or they get vacuumed up when the wave ends.
- **Tinker's Wagon:** every 3rd wave, spend scrap on hearts, Brass Plating, spin charges and extra upgrades.
- **Elites:** from wave 4, some enemies spawn with a golden aura. They're bigger and tougher, and drop triple scrap.
- Your build shows bottom-left during play and on the game-over screen.

There are 22 upgrades, including Akimbo, Dynamite Tips, Second Wind, Steam Burst, Last Chamber, Trick Shot, Drill Bits and Big Iron.

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
- `?give=pierce,akimbo,...`: start with these pickups/upgrades (upgrade ids are in `UPGRADES`)
- `?shopstop`: with `?bot`, stop at the shop instead of auto-buying
- `?touch`: force the touch layout

## GitHub Pages
Settings → Pages → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)`.
