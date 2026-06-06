# Darkland

A dark, post-apocalyptic **mobile base-building zombie shooter** that runs in any web browser — no install needed.

## ▶ How to play
Open **`game/darkland.html`** in a web browser (just double-click it).

- **Phone:** left joystick = move · **FIRE** (hold to keep shooting) · LOOT · USE · Menu (craft/map/quests/base/**build**/**settings**)
- **Computer:** WASD = move · Z (hold) = fire · X = loot · E = use · I = inventory · C = craft · M = map
- **Survive the night:** at 8 PM a **horde** rises — gun it down to earn caps, XP, and supplies. Every **5th night is a Boss Night**.
- **Build defenses:** ☰ Menu → Build Mode → face a spot and tap to place walls, turrets, spikes, and floodlights.
- **Settings:** ☰ Menu → Settings (or the title screen) for audio, controls (incl. left-handed mode), display, and more.

## 📒 The plan
See **[PROJECT.md](PROJECT.md)** for the full plain-English outline: what's built, the world, items, quests, and what's next.

## ✅ Latest progress (2026-06-06)
**Turned Darkland into a real base-building zombie shooter.**

*Shooter feel:*
- Bullet tracers, recoil screen-kick, muzzle flash + smoke, and a white impact flash on every zombie hit. Hold FIRE to keep shooting.
- Sound effects added: gunshots, turret zaps, the build "ka-chunk," and a deep tone when a Boss Night begins.

*Threat & hordes:*
- **Night hordes / base-defense loop:** at 8 PM a horde rises and pours in from all sides — tougher each night. A banner tracks how many are left; survive to earn caps, XP, and supplies.
- **Boss Nights:** every 5th night a scaled-up boss joins the horde with its own alert.
- **Better zombie animation:** zombies used to look like crawling spiders (they were drawn with 4 arms). Now they shamble on two reaching arms, with per-type gaits — runners scurry, mutants stomp, walkers shuffle.

*Base building & defenses:*
- New base modules: **Auto-Turret** (auto-fires, boss-priority), **Perimeter Wall** (armor near base), **Spotlight** (lights the base at night).
- **Build Mode:** place **walls, turrets, spikes, and floodlights** anywhere — walls block zombies, turrets gun them down, spikes shred them, floodlights light the dark. Everything has health and saves with your game.
- Fixed a bug where base upgrades were wiped on reload.

*Controls & options:*
- **Uncrowded controls:** big round FIRE button (shows weapon + live ammo), tidy round USE/LOOT buttons, hotbar on its own row.
- **Full Settings menu** (title screen + in-game): SFX/ambient volume, screen shake, damage numbers, blood & gore, FPS counter, **left-handed mode**, joystick sensitivity, vibration, fullscreen, and reset progress. All preferences are saved.

*Main character:*
- **New player look:** redrawn as a creepy stitched **burlap voodoo doll** to match Sean's reference (`game/design-references/player-reference.jpeg`) — golden sackcloth body, glowing red hollow eyes & a torn mouth glowing inside, rope at neck/waist, a satchel, stick-bundles strapped on, and a bloody barbed-wire hatchet. Keeps the walk shamble, weapon aiming, and a soft glow so you can spot yourself in the dark.

**Next ideas:** turret/weapon upgrade trees · more zombie types & special abilities · a permanent shareable GitHub Pages link.

> ℹ️ A temporary "click-to-play" web link can be created during a work session, but it only works while that session is running. For a permanent shareable link, ask about setting up a free GitHub Pages site.

---

### How we work together (notes for the AI helper)
- Sean does not code — explain everything in plain, no-code terms.
- This is a game-building project.
- When Sean says **"end and save"**, update this `README.md` and `PROJECT.md` with whatever changed that session.