# Darkland — Project File

*Last updated: 2026-06-06*

This is the plan and the "what's been built so far" notebook for the game.
It's written in plain language (no code-speak) so you can always pick it back up.

---

## 1. The Big Picture

- **Project name:** Darkland
- **Game name shown on screen:** *DARKLAND* (title screen, browser tab, and subtitle all match the project name)
- **Type of game:** Mobile **base-building zombie shooter** (with survival/RPG systems underneath). North star: *the best mobile base-building zombie shooter*.
- **Setting:** A dark, post-apocalyptic wasteland. You scavenge and build by day, then defend against zombie hordes by night.
- **How it runs:** A single web page (an `.html` file). You double-click it and it opens in any web browser. **No install, no internet, no server needed.**
- **Plays on:** Phone (touch controls) and computer (keyboard).

---

## 2. How You Play It

**On a phone (touch):**
- Left joystick = move around
- **FIRE button** (big red, bottom-right) = shoot/attack — **hold it down to keep firing**. It shows your equipped weapon and live ammo count.
- LOOT button = search for supplies
- USE button = use an item
- Menu (☰, top-right) = inventory, crafting, map, quests, base, **build mode**, and **settings**

**On a computer (keyboard):**
- W A S D = move
- Z (hold) = fire/attack
- X = loot
- E = use
- I = inventory
- C = crafting
- M = map

---

## 3. What's Already Built (the game's systems)

The game already has a lot working. Here's everything that's in there:

- **A living world** drawn in an "isometric" style (a tilted 3D-looking top-down view), with day/night, weather, lighting, and sound.
- **Movement & combat** — walk around, attack enemies, take damage, die, respawn.
- **Shooter-feel gunplay** *(added 2026-06-06)* — bullet tracers streak to targets, recoil kicks the screen, muzzle flash + smoke, and a white impact flash on each hit. Hold FIRE to keep shooting; guns use ammo. Sound effects for shots/turrets/building/bosses.
- **Night hordes / base-defense loop** *(added 2026-06-06)* — every night at 8 PM a horde rises and pours in from all sides, growing tougher each night. A top banner tracks how many remain; surviving rewards caps, XP, and supplies. The loop: scavenge & build by day, defend by night.
- **Boss Nights** *(added 2026-06-06)* — every 5th night a scaled-up boss joins the horde with its own alert.
- **Build Mode** *(added 2026-06-06)* — place defenses anywhere: **walls** (block zombies), **turrets** (auto-fire, boss-priority), **spikes** (damage on contact), **floodlights** (light the night). Structures have health, can be destroyed, and save with the game.
- **Settings menu** *(added 2026-06-06)* — audio volumes, screen shake, damage numbers, blood & gore, FPS, left-handed mode, joystick sensitivity, vibration, fullscreen, reset progress — all saved between sessions.
- **Main character** *(redrawn 2026-06-06)* — a stitched **burlap voodoo doll** survivor (per `game/design-references/player-reference.jpeg`): golden sackcloth body, glowing red hollow eyes & torn glowing mouth, rope at neck/waist, satchel pouch, stick-bundles strapped on, bloody barbed-wire hatchet. Animates with a walk shamble and aims its weapon toward enemies.
- **Survival meters** — things like health you have to manage to stay alive.
- **Enemies** — zombies, walkers, runners, plus tougher ones like Boss Zombie, Boss Raider, Mutant, Toxic Z, Rifleman, Heavy, Scavenger. Each zombie type now has its own walk: runners scurry, mutants stomp, walkers shuffle.
- **Looting** — search containers and bodies to find supplies.
- **Inventory** — a bag system to hold and use what you find.
- **Crafting** — build items at a crafting bench from raw materials.
- **Base building** — set up and upgrade a home base: storage, medical station, generator, water purifier, farm, **plus defenses (auto-turret, perimeter wall, spotlight)**. Base upgrades now persist across reloads.
- **Quests** — goals to chase (see list below).
- **Leveling up** — earn XP, gain levels, get stronger.
- **Random world events** — surprises that pop up as you play (see list below).
- **Save system** — the game automatically remembers your progress in the browser.

### Places in the world (zones)
Ashvale · Dustfall · Rustvale · Toxic Bog · Deadwood · Fort Despair · Vault 17 · Refinery 9 · Iron Works · New Dawn · Outpost Echo · Safe House

### Quests already in the game
- First Steps — Explore Ashvale and survive
- Thin the Horde — Kill 10 enemies
- Fort Cache — Find the military cache
- Daily Hunt — Kill 5 enemies today
- Scavenger — Loot 3 containers

### Random events already in the game
- Supply Drop — a cargo plane drops military supplies
- Wounded Survivor — offers caps for bandages
- Raider Toll, Trader Caravan, Radiation Storm, Hidden Bunker

### Items already in the game
- **Weapons:** Knife, Hatchet, Machete, Iron Pipe, Pistol, Rifle, Shotgun, Compound Bow, Plasma Rifle
- **Ammo:** 9mm Ammo, Rifle Ammo, Shells
- **Armor:** Rag Armor, Leather Armor, Combat Armor, Metal Armor, Hazmat Suit
- **Healing:** Bandage, Med Kit, Stimpak, Antidote, Rad-X
- **Food & drink:** Canned Food, Cooked Meat, MRE, Stale Bread, Soda, Water, Pure Water
- **Materials:** Wood, Scrap Metal, Cloth, Leather, Chemicals, Electronics, Gunpowder, Fuel
- **Money:** Caps
- **Base parts:** Crafting Bench, Generator, Water Purifier, Medical Station, Storage Room, Farm, Lockpick
- **Defenses (base upgrades):** Auto-Turret, Perimeter Wall, Spotlight
- **Buildable structures (Build Mode):** Wall, Turret, Spikes, Floodlight

---

## 4. The Files (where everything lives)

```
Darkland/
├── README.md                         <- Quick intro + how to play
├── PROJECT.md                        <- THIS FILE (the full plan & progress)
├── game/
│   ├── darkland.html                 <- ▶ THE GAME — open this to play (latest)
│   ├── design-references/            <- Art references Sean provided
│   │   ├── player-reference.jpeg     <- The burlap voodoo-doll main character
│   │   ├── zombie-reference.png
│   │   └── world-reference.png
│   └── older-versions/               <- Earlier drafts, kept for safety
│       ├── darkland-v1.html
│       ├── darkland-v3.html
│       └── darkland-v4.html
├── backups/                          <- Timestamped safety copies of the game
│   └── DARKLAND_GAME_original.zip     <- Untouched copy of your original upload
└── DARKLAND_GAME.zip                 <- Your original zip (left in place)
```

**To play:** open `game/darkland.html` in any web browser.

---

## 5. The Vision (Sean's goal for the game)

Make Darkland feel like a **real, eerie, creepy zombie survival game** where you can:
- Explore just about anywhere in the world
- Survive with realistic-feeling movement
- Fight zombies that look and move like the real undead
- **Build your own base** by collecting supplies
- **Level up** by killing enemies

### Roadmap to get there
| Pass | Goal | Status |
|------|------|--------|
| 1. Eerie atmosphere | Grim cold tint, screen-edge darkness, drifting ash, low-health blood pulse | ✅ DONE |
| 2. Creepier zombies | Rotting flesh, sunken glowing eyes + halo, gore/blood stains | ✅ DONE |
| 2b. Match reference art | Pale ashen skin, blank white eyes, torn blue bloody shirt, hunched clawing pose, snarling teeth (from Sean's uploaded reference) | ✅ DONE |
| 2c. Richer world detail | Keep grim wasteland mood but add detail (Sean's world reference): scattered ground debris + bones, fuller gnarled trees, cold god-ray light shafts | ✅ DONE |
| 3. Shambling walk | Uneven lurching/limping so zombies move like the undead | ⬜ next |
| 6. World structures | Stone ruins, a tomb/dungeon "ENTER" doorway, a glowing portal (from world reference) | ⬜ planned (bigger) |
| 4. Deeper exploration | Walk into buildings / find interior loot | ⬜ planned |
| 5. Base & leveling polish | Clearer rewards for scavenging and killing | ⬜ planned |

## 6. Open Questions / Decisions To Make

1. ✅ ~~The name~~ — decided: **Darkland** (fixed everywhere in the game).
2. ✅ ~~A permanent shareable link?~~ — done: published via **GitHub Pages**. Forever-link: **https://seanosgood2-oss.github.io/Darkland/**
3. **Where should the game eventually live long-term?** (GitHub Pages is live now. App store later?)

---

## 6. Session Log

- **2026-06-06** — Opened your uploaded zip. Found a working browser-based survival RPG with 4 versions. Organized files into a clean folder layout, picked the latest version as the main game, archived the older ones, backed up the original zip, and wrote this project file.
- **2026-06-06** — Renamed game to **Darkland** everywhere. Set up a clickable play link via a local web server. **Fixed two crash bugs** (`vpT` undefined in the tile grid, and `drawFire` → `tl_drawFire`) that were causing a blank map. Verified the game runs error-free using an automated headless-browser test (with screenshots).
- **2026-06-06** — Began the eerie-zombie vision. **Pass 1 (atmosphere):** added an always-on grim cold tint, drifting ash motes, a screen-edge darkness vignette (tunnel vision), and a red blood-pulse when health is low. **Pass 2 (zombies):** sickly grey-green rotting flesh, sunken eye sockets with pulsing glowing-eye halos, facial rot blotches, and blood stains/drips on the torso. Both passes tested error-free with close-up screenshots.
- **2026-06-06** — Fixed four gameplay bugs reported by Sean (all verified with automated browser tests):
  1. **Combat did no damage** — melee only hit a narrow cone in front. Now melee auto-faces the nearest in-range zombie so swings reliably connect; reduced knockback so enemies stay in reach.
  2. **Item bar blocked the view** — moved the hotbar from the lower-middle to a compact bar at the very bottom-center (and raised it above the joystick layer so it stays clickable).
  3. **Trapped in base on respawn** — added a `findClearTile` helper that respawns the player on open ground beside the base instead of inside a wall.
  4. **Character hard to see** — camera now centers the character near the middle of the screen; made the player bigger (1.1→1.25) and added a soft blue glow ring at their feet.
- **2026-06-06** — Sean uploaded a lush forest **world reference** and chose **"dark wasteland + this detail"**: keep the grim creepy mood but add richness. Added a deterministic ground-detail scatter (grass-blade clumps, pebbles, twigs, dry dead patches, hairline dirt cracks, rare stray bones), rebuilt trees with layered clumpy canopies + gnarled trunks + bare dead branches + cold rim-light, and added pale **cold god-ray light shafts** slanting across the scene. Verified day + zoomed screenshots, error-free. Reference images saved in `game/design-references/`.
- **2026-06-06** — Published Darkland to a **permanent shareable link** via GitHub Pages (**https://seanosgood2-oss.github.io/Darkland/**) so it can be played on a phone and shared without a running work session. Added a root `index.html` that redirects to the game, committed the game files (kept bulky backup zips local-only via `.gitignore`). Confirmed the on-screen name already reads **DARKLAND** everywhere user-facing (cleaned up one stale `WASTELAND ZERO` code comment).
- **2026-06-06** — Sean uploaded a realistic crawling-zombie reference and chose to have the game's zombies **redrawn in the game's style to match it** (rather than dropping in the photo). Updated the zombie art: pale ashen-grey flesh, blank milky-white glowing eyes (toxic = green), torn blood-stained blue shirt with ragged tears showing flesh, a forward hunch, long gnarled arms reaching forward with splayed grasping claws, and a snarling toothy mouth. Verified with a zoomed close-up screenshot, error-free.
