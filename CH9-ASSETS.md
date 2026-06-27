# ECLIPSE — Chapter 9 "The Long Road Home" — Asset checklist

All files go in `assets/` next to `index.html`, using these **exact** filenames. Everything shows a
graceful placeholder until the file exists, so you can add art in any order and playtest immediately.
Keep the painted, top-down 16:9 look for rooms, and full-frame painted images for cinematic beats.

---

## 1. Room backgrounds (16:9, top-down)
| File | Room / use |
|---|---|
| `ch9-title.png` | Chapter title art |
| `ch9-watchtower.png` | The siren watchtower (top-down) — used as the siren mini-game backdrop |
| `ch9-road-bg.png` | Seamless **vertically-tiling** road for the driving game (dark forest highway) |
| `ch9-hotel-lobby.png` | Hotel lobby |
| `ch9-hotel-kitchen.png` | Hotel restaurant/kitchen |
| `ch9-hotel-corridor.png` | Guest-room floor (the 4 rooms + manager's door) |
| `ch9-hotel-basement.png` | Basement / generator room |
| `ch9-hotel-manager.png` | Manager's office (with the safe) |

---

## 2. Cinematic / story-beat images (full-frame painted)

**Opening (Whitehall → escape):**
- `ch9-lena-story-1.png` — Lena describing the green-land town / cottages
- `ch9-lena-story-2.png` — the valley's traps & floodlights / refugees
- `ch9-lena-story-3.png` — Lena's father, killed by the soldiers (flashback)
- `ch9-saddie-grief.png` — Saddie breaking down, can't leave Salaar
- `ch9-dakie-carries-salaar.png` — Dakie carrying Salaar on his shoulders, Lena comforting Saddie
- `ch9-escape-1.png` — fighting through the white halls
- `ch9-escape-2.png` — cutting the locks, freeing the captive women
- `ch9-captives-freed.png` — the freed women gathered behind them

**Siren:**
- `ch9-siren-discover.png` — Dakie discovering the emergency siren / watchtower
- `ch9-siren-overrun.png` — thousands of infected swarming Whitehall (the win beat)

**Highway → driving:**
- `ch9-highway-arrive.png` — reaching the cracked, silent highway
- `ch9-highway-bodies.png` — dead bodies and abandoned cars on the road
- `ch9-highway-car.png` — the car they pick to drive
- `ch9-fuel-out.png` — the car dying on the shoulder, out of fuel
- `ch9-broken-bridge.png` — the collapsed bridge (used in the bridge puzzle header art if you want)

**Hotel:**
- `ch9-hotel-see.png` — first glimpse of the abandoned hotel in the dark/rain
- `ch9-hotel-enter.png` — pushing open the hotel doors in the rain

**Night confession + siege:**
- `ch9-confession-1.png` — Dakie & Saddie by torchlight, Salaar's coat nearby
- `ch9-confession-2.png` — the confession; Saddie silent, crying, unable to answer
- `ch9-siege-start.png` — the horde arriving, drawn by the restored power

**Grief (NEW):**
- `ch9-salaar-burial.png` — Dakie, Saddie & Lena burying Salaar on a hill above the burning compound; Saddie placing something personal on the grave

**Ending:**
- `ch9-dawn.png` — morning after the siege, the hotel damaged, infected gone
- `ch9-home.png` — green fields, windmills, cottages with chimney smoke (first glimpse of home)

---

## REGISTRY / MASTER-KEY PUZZLE — exact art content (so it's solvable)

The puzzle is **fully visual now** — no spoilers in dialogue or journal. The player reads the four
room fragments (each has a NUMBER + a guest comment with a keyword) and the front-desk master ledger
(a maintenance checklist whose word ORDER gives the sequence). Reading the ledger order and swapping
each keyword for its room's number gives the code **2751**. For this to work, please make the art say:

| File | Number (red stamp) | Guest comment keyword |
|---|---|---|
| `ch9-registry-1.png` | **2** | "...the **COTTAGE** by the lake was full, so he took this room." (Daniel Harper) |
| `ch9-registry-2.png` | **7** | "The **WINDMILL** can be seen from the eastern window." (Margaret Lewis) |
| `ch9-registry-3.png` | **1** | "Walks the **FIELD** every morning before dawn." (Robert Kane) |
| `ch9-registry-4.png` | **5** | "The **CHIMNEY** needed repairs last winter." (Helen Moore) |

- `ch9-master-registry.png` — the open front-desk ledger. Its maintenance checklist must list the four
  words **in this order**: **COTTAGE → WINDMILL → CHIMNEY → FIELD**. (That order → 2, 7, 5, 1 → **2751**.)
  Keep it subtle and authentic, as you described — it shouldn't look like a puzzle.

*(All four fragments + the ledger are now saved as **zoomable bag items** — open the BAG, tap one to view it full-screen, so you can line them up and work out 2751 yourself.)*

---

## BROKEN-BRIDGE RECONSTRUCTION — image list (the redesigned game)

The bridge is now image-driven: a top-down yard you scavenge (each spot shows its own picture and gives
a hard, tempting set of choices — pick wrong **3 times** and the whole salvage restarts), then a
step-by-step build that shows the crossing forming. Generate these (placeholders show until added):

**The yard + each searchable spot (top-down):**
- `ch9-bridge-yard.png` — the whole maintenance yard near the collapsed bridge (the overview shown first)
- `ch9-bridge-truck.png` — crashed highway recovery truck (has the **tow rope**)
- `ch9-bridge-van.png` — maintenance van pinned by a girder (has the **car jack**)
- `ch9-bridge-depot.png` — repair-depot storage cage of road plates (has the **steel planks**)
- `ch9-bridge-genstation.png` — generator/fuel station with abandoned cars (fill the **fuel can**)
- `ch9-bridge-sedan.png` — roadside sedan (optional supplies — and traps)
- `ch9-bridge-shed.png` — utility shed (optional supplies — and traps)
- `ch9-bridge-pickup.png` — stripped pickup (a **trap** — nothing good here; tempts you into mistakes)

**The construction, step by step (top-down: left side ▮ gap ▮ right side):**
- `ch9-bridge-build-1.png` — steel planks laid across the gap
- `ch9-bridge-build-2.png` — jack set under the centre
- `ch9-bridge-build-3.png` — tow rope lashed to the anchors
- `ch9-bridge-build-4.png` — fuel/winch tensioning it
- `ch9-bridge-done.png` — the finished crossing (used while the SUV tests it)

**Items (you said you've made planks etc. — these are the bag/choice thumbnails):**
`ch9-item-rope.png`, `ch9-item-jack.png`, `ch9-item-planks.png`, `ch9-item-fuelcan.png` (already listed above).

*(The kitchen food puzzle — "light the burners in the right order" → smoked salmon — is drawn on-screen,
so it needs **no images**.)*

---

## HOTEL GENERATOR + PREPARE-THE-HOTEL SIEGE — image list (now built)

**How it works now:** restore the generator (find fuel can + battery + fuse → seat all three → throw the
breakers in order, lowest amperage to highest). Power flickers on → **prep phase**: walk the hotel and
physically secure it — **barricade the lobby doors** (couch/desk/bookshelf — pick one), **board the
kitchen window**, **chain the basement service door**, **post Lena** upstairs or with the survivors.
Then barricade the lobby doors and "begin the night." The **siege is a chain of events** that play out
from exactly those choices (no waves, no menu), and survivor count decides the good vs. grim ending.

**Required new item art:**
- `ch9-item-fuse.png` — the ceramic fuse (the third generator part)

**Reused (no new files needed):** the generator scene uses `ch9-hotel-basement.png`; the siege events
reuse `ch9-siege-start.png`, `ch9-hotel-kitchen.png`, `ch9-hotel-basement.png`. So it already works.

**Now ALL WIRED IN (drop the files in `assets/` and they appear):**
- `ch9-prep-lobby-couch.png`, `ch9-prep-lobby-desk.png`, `ch9-prep-lobby-shelf.png` — shown when you barricade the lobby with that piece
- `ch9-prep-window-boarded.png` — shown when you board the kitchen window
- `ch9-prep-basement-chained.png` — shown when you chain the service door
- `ch9-lena-lookout.png` — shown when you post Lena upstairs
- `ch9-siege-lobby.png`, `ch9-siege-kitchen.png`, `ch9-siege-basement.png`, `ch9-siege-roof.png` — each siege breach event
- `ch9-siege-genfail.png` — the mid-siege generator failure / restart in the dark
- `ch9-generator-restore.png` — the repaired generator roaring to life (shown when power comes back)
- `ch9-night-begins.png` — **(NEW)** the calm before the storm: doors shut, Lena on the stairs, generator glow, infected silhouettes in the dark forest. Plays as the first beat of the night, before the confession.
- `ch9-item-food.png` — the cooked salmon now pops up full-screen when you win the kitchen burner game.

---

## 3. Item images (popup + bag thumbnails)
- `ch9-item-fuelcan.png` — fuel can (also the collectible on the road)
- `ch9-item-battery.png` — batteries (flashlight)
- `ch9-item-food.png` — tinned food
- `ch9-item-medicine.png` — first-aid kit
- `ch9-item-blanket.png` — blankets
- `ch9-item-rope.png` — tow rope (bridge part)
- `ch9-item-jack.png` — car jack (bridge part)
- `ch9-item-planks.png` — metal planks (bridge part)
- `ch9-road-obstacle.png` — a road hazard (wreck/rock/barricade) for the driving game
- `ch9-car-wreck.png` — wrecked car (bridge-search flavor, optional)

**Master-key registry / clue art (one per guest room — recommended, per your idea):**
- `ch9-registry-1.png` — Room 2's fragment / registry page
- `ch9-registry-2.png` — Room 7's fragment / registry page
- `ch9-registry-3.png` — Room 1's fragment / registry page
- `ch9-registry-4.png` — Room 5's fragment / registry page

*(In-game the 4 rooms hold digits 2, 7, 1, 5; the lobby registry reveals the order **1-7-5-2** = the master key. If you draw each registry page with its number clearly stamped, the puzzle reads great.)*

---

## 4. Reused / already in your assets (no new files needed)
`enemy-zombie.png` (siren-game infected sprites), all existing `sfx-*.mp3`, the music beds, and the
`ch8` audio system. The siren/basement/kitchen use the existing tense "scary" track automatically.

---

## 5. Optional new audio (tell me and I'll wire it)
- `ch9-music.mp3` — a Chapter 9 ambience loop (road / hotel)
- `ch9-engine.mp3` — engine loop for the driving game
- `ch9-siren.mp3` — the wailing siren loop for the watchtower game

---

## Chapter 9 mini-games (for reference)
1. **Siren Defense (watchtower)** — tap CRANK to keep power up, tap infected to shoot them off the tower; the longer it screams the higher CHAOS climbs. Fill CHAOS to 100% to bury Whitehall; lose if the siren is destroyed.
2. **Survival Driving** — auto-forward, steer L/R (keys/joystick/drag), fuel drains and speeds up over time, dodge wrecks (health), grab fuel cans, reach 0 km. Lose on fuel-out or health-out.
3. **Broken Bridge** — search 3 wrecks for jack / planks / rope, then assemble in the right order (lift → span → lash).
4. **Hotel (Resident-Evil hub)** — explore lobby/kitchen/corridor/basement/manager with a **flashlight + battery** you must manage (F key or the on-screen LIGHT button). Gather food, medicine, batteries, blankets.
5. **Power Routing (priorities)** — the generator only carries 5 units; choose which systems to power (lights/doors/elevator/kitchen). Choices carry into the siege (e.g. Security Doors pre-seal a door).
6. **Master Key** — 4 room fragments + the registry order → enter **1752** to open the manager's office (and the safe → shotgun).
7. **Siege (3 waves)** — spend barricades/traps/guards across 3 entrances, then survive 3 escalating waves. Keep enough survivors alive for the good ending; lose too many for the grim variation.
