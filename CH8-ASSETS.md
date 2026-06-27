# ECLIPSE — Chapter 8 "Betrayal" — Asset checklist

All files go in the `assets/` folder next to `index.html`, using these **exact** filenames.
Everything fails gracefully (shows a "loading…" placeholder) until the file exists, so you can
add them in any order and playtest immediately.

Style note: keep the same painted, top-down 16:9 look as Ch6/Ch7 for room backgrounds, and
full-frame painted images for the cinematic beats.

---

## 1. Room backgrounds (16:9, top-down)

| File | Room |
|---|---|
| `ch8-title.png` | Chapter title art |
| `ch8-approach.png` | Dakie & Salaar approaching the white house through the trees |
| `ch8-lab.png` | Medical lab — tanks, sample racks, glass |
| `ch8-barracks.png` | Armoury wing / barracks with the wide balcony |
| `ch8-balcony.png` | The shooter view — looking DOWN from the balcony to the ground (zombies fall top→bottom across this) |
| `ch8-dungeon.png` | The dungeon (barred gate, Saddie's cell) with a generator-room doorway on the right |
| `ch8-generator.png` | Generator room with the breaker panel |

**Reused from Ch7 (already in your assets — no action needed):**
`ch7-kitchen.png`, `ch7-armory.png`, `ch7-whitehouse.png`, `ch7-akm.png`

---

## 2. Cinematic / story-beat images (full-frame painted)

**Opening + guard:**
- `ch8-arrive.png` — arriving at the gate / first look inside
- `ch8-guard-welcome.png` — guard smiling, welcoming them
- `ch8-guard-shock.png` — guard's face: shock for a heartbeat when Saddie is described
- `ch8-guard-smile.png` — the sinister smile that follows
- `ch8-lab-intro.png` — guard leading them into the lab

**Lab:**
- `ch8-sample1.png` — sample A (also reused as the extracted-vial item)
- `ch8-sample2.png` — sample B
- `ch8-sample3.png` — sample C
- `ch8-sample4.png` — sample D
- `ch8-lab-page.png` — the page nailed to the wall ("WE ARE ONE…", contains the 3‑3‑0)

**Barracks → balcony:**
- `ch8-barracks-reveal.png` — military men panicking, loading guns
- `ch8-crossbow-pickup.png` — being handed the crossbows (also reused as the crossbow item)
- `ch8-zombies-approach.png` — the horde dragging toward the wall (used before/after the shooter)
- `ch8-guard-meal.png` — guard telling them "good shooting… go eat"

**Kitchen:**
- `ch8-captive-tell.png` — a captive woman telling them what happened
- `ch8-dakie-fear.png` — Dakie & Salaar, fear/panic as they realize it's Saddie
- `ch8-dakie-anger.png` — their faces turning to rage

**Armory:**
- `ch8-armory-banging.png` — guard banging on the armory door (used for the timer + the kill scene)

**Escape → dungeon:**
- `ch8-shoot-guard.png` — Dakie shooting the guard
- `ch8-run-dungeon.png` — running down to the dungeon, out of bullets
- `ch8-dungeon-reunion.png` — Saddie crying with joy seeing them (reused for the hug/gate-open beat)

**Ending:**
- `ch8-hug.png` — Saddie hugging Dakie tight; Lena's first real smile
- `ch8-salaar-cover.png` — **(NEW)** Salaar throwing himself in front of Saddie, arms wide, shielding her (the moment before the shot)
- `ch8-salaar-shot.png` — Salaar is hit and folds
- `ch8-dakie-guns.png` — Dakie grabbing the AKM/M416 from the bag and firing
- `ch8-salaar-death.png` — Salaar's head on Saddie's lap, his last words
- `ch8-lena-place.png` — Lena, tears on her face: "Guys… I know a place"

---

## 3. Audio

**Already used (reused from your existing assets — no new files required):**
`sfx-click`, `sfx-thud`, `sfx-shoot`, `sfx-hurt`, `sfx-success`, `sfx-door`, `sfx-unlock`,
`sfx-pickup`, and `sfx-alarm` (plays as the guard hammers the armory door).
Background music reuses the existing tense/`scary` bed during the shooter, armory and dungeon.

**New audio — NOW WIRED IN (just drop the files in `assets/`):**
- `ch8-music.mp3` — Chapter 8 ambience loop (plays during calm exploration: lab, kitchen, barracks)
- `ch8-banging.mp3` — fist-on-door banging loop; plays the whole time the armory 2:00 timer runs
- `ch8-grief.mp3` — **(NEW)** the emotional track for the ending. Starts the instant Salaar shields Saddie and plays through the rest of the scene to the chapter-end card.

---

## 4. Optional / not currently used by the code

These are referenced loosely or were in your brief but the matching mini-game is self-contained
(abstract), so they're **optional polish**, not required:
- `ch8-gate.png`, `ch8-generator-intro.png` (declared but no beat shows them yet)
- separate `rifle` / `magazine` / `bullets` item art — the magazine-loading puzzle is drawn with
  clean on-screen graphics, so it doesn't need image files. If you generate them I can swap them in.

---

## Mini-games in Chapter 8 (for reference)
1. **Water-sort (lab)** — 3 tubes, 2 colours, 1 empty; ≥4 moves; pure-colour win.
2. **Crossbow shooter (balcony)** — zombies fall top→bottom; aim + click/tap, reload between bolts, limited bolts with partial recovery; headshots instant-kill, body shots stagger; fail = wall HP hits 0 (retry the wave, not the chapter).
3. **Poison detection (kitchen table)** — limited test strips, find & eat 3 safe dishes; wrong = HP loss.
4. **Magazine loading (armory)** — 2:00 timer, flip each round the right way, load 10, insert mag, charge handle; fail = guard kills you, chapter restarts (3 deaths = death screen).
5. **Power grid (generator)** — throw breakers in the right order (A→C→D, B is fried); wrong = sparks, resets.

Armory door code this chapter: **330** (from the lab wall).
