# ECLIPSE — Images & Audio to generate (chapter polish pass)

Drop all files in `assets/`. Anything missing falls back gracefully, so you can add in any order.
Exact filenames matter.

═══════════════════════════════════════════════════════════════════════
## 1. CHAPTER‑END SCREENS (painted background, one per chapter)
The end‑of‑chapter "Continue" page will use these as a full‑frame background (no more wall‑of‑text).
- `ch1-end.png` — the survivors leaving the lab platform into grey dawn
- `ch2-end.png` — the car pulling out of downtown onto the open road
- `ch3-end.png` — Saint Mary's hospital behind them at dusk
- `ch4-end.png` — climbing out of the subway into the ruined city
- `ch5-end.png` — leaving the lit tower / carnival behind
- `ch6-end.png` — the river camp at first light (after Lena)
- `ch7-end.png` — escaping the farmhouse, fields ahead
- `ch8-end.png` — slipping away from the betrayed safe‑zone
- `ch9-end.png` — the hotel/forest road behind, the village gate ahead
(Chapter 10 already has its own "TO BE CONTINUED" art plan.)

═══════════════════════════════════════════════════════════════════════
## 2. CINEMATIC INTROS (replacing the old "Begin" title screens)
Each chapter opens on a short painted cinematic instead of a press‑to‑begin card.

**Chapter 2 — "How they reached downtown"**
- `ch2-intro-1.png` — Dakie & Saddie fleeing the lab district on foot, smoke behind
- `ch2-intro-2.png` — crossing a wrecked overpass into the downtown skyline
- `ch2-intro-3.png` — ducking into the parking structure as infected wander the street

**Chapter 3 — "How they reached Saint Mary's" (Saddie is hurt)**
- `ch3-intro-1.png` — night streets; Saddie limping, hand pressed to a bleeding side
- `ch3-intro-2.png` — Dakie spotting the hospital's red cross sign through the rain
- `ch3-intro-3.png` — the two stumbling through the hospital doors

**Chapter 4 — "How they reached the subway"**
- `ch4-intro-1.png` — a street collapse forcing them underground
- `ch4-intro-2.png` — descending a dead escalator into the dark station
- `ch4-intro-3.png` — the platform: stalled train, scattered belongings

**Chapter 5 — "Following the lights"**
- `ch5-intro-1.png` — Saddie on a rooftop seeing distant lit‑up towers/lights on the horizon
- `ch5-intro-2.png` — the trio deciding to follow the lights (hope of survivors)
- `ch5-intro-3.png` — creeping past a horde, hiding in shadow from the infected

═══════════════════════════════════════════════════════════════════════
## 3. PER‑SCENE CINEMATICS (inside chapters)
**Chapter 3**
- Candle room: `ch3-candles-1.png`, `ch3-candles-2.png` — Saddie noticing the arranged candles / the meaning
- Pharmacy bandaging: `ch3-bandage-1.png`, `ch3-bandage-2.png` — Dakie cleaning & wrapping Saddie's wound, quiet and tender

**Chapter 4**
- Piano scene: `ch4-piano-1.png`, `ch4-piano-2.png` — the dim room, the piano, the letter on the stand

**Chapter 5**
- Height fear: `ch5-height-1.png`, `ch5-height-2.png` — Saddie frozen at the edge, breathing hard, Dakie steadying her

**Chapter 6** (if you want stills for Lena's vanishing)
- `ch6-lena-gone-1.png`, `ch6-lena-gone-2.png` — the empty camp where Lena was, the silent radio

═══════════════════════════════════════════════════════════════════════
## 4. AUDIO
**Per‑chapter theme music (loops):**
- `ch2-music.mp3` — downtown tension
- `ch3-music.mp3` — hospital dread
- `ch4-music.mp3` — subway unease
(ch5–ch9 already have themes; ch10 has `ch10-music.mp3`.)

**Scene songs:**
- `ch3-bandage.mp3` — soft, intimate piece for the pharmacy bandaging scene
- `ch4-piano.mp3` — the piano puzzle melody (if not already added)
- `ch10-defense.mp3` — village‑defense music (plays from the defense hub to chapter end)
- `ch10-romance.mp3` — plays only in Saddie's room (knock → confession → hug → LOVERS)

═══════════════════════════════════════════════════════════════════════
## NOTES
- The relationship stage shown top‑right advances one step per chapter:
  Strangers → Acquaintances → Allies → Companions → Friends → Confidants → Attached → Smitten → Unspoken → Lovers.
- Health and medkit counts now carry across chapters (no auto‑refill, no replay inflation).
- Keypads, the menu button, and minigame UIs are being made fully phone‑responsive.
