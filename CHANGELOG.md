# Wildling Isle — Change Log

All notable changes to the game, newest first. Each entry corresponds to a
release merged to the live game.

---

## The Battle & World Update — 2026-07-18 (PR #32)

### Battle
- **Participation XP**: every Wildling that takes the field against a foe
  now splits that foe's XP evenly — swap once mid-fight and the two
  fighters earn 50/50. Tracked per enemy in trainer battles, so only those
  who actually faced each foe share in it

### Team
- **Move reorder**: the team submenu gained MOVES — pick a move, pick a
  slot, and they trade places. Set your favorite opener as slot one

### World
- The Everglade Sloughs finally got a campfire (southeast corner) — no
  more gator country without a place to rest
- Thirteen roaming trainers settled the Parklands: two per park (one
  easy, one tough, all replayable) plus a dockhand at the Gateway —
  matching the two-per-area standard of the older isles

### Types & Moves
- **Dual types**: 24 Wildlings now carry two types, Pokemon-style —
  Sylvarch is Mystic/Flora, Mammorime and Cragoram Frost/Stone, the
  elemental birds ride Gale, the mushroom line is Flora/Venom, Geyserun
  runs boiling Tide/Ember, and more. Damage multiplies across both:
  4x hits ("It's devastatingly effective!"), double-resists ("It barely
  leaves a mark..."), and weakness-cancelling combos all exist now
- **The bane rule**: no Wildling can ever learn a move of a type it is
  weak against (combined across both types; your own nature is exempt) —
  enforced everywhere moves are taught
- **Coverage affinities**: a few species keep bonus off-type song access
  at the tutor beyond their typing (Mammorime's Tide, Celestaur's Stone,
  Monolythe's Spark, Oraclaw's Frost)
- The tutor offers songs for both types, scrolls, and labels each song
- Battle matchup hints and the info screen understand dual types
- Cleaned two old violations: Cragoram and Mammorime carried Stone
  moves while mono-Frost; type-changing evolutions shed illegal moves

### Fixes
- Mammorime's frozen mass now wakes from a press on ANY of its tiles —
  it previously only answered at one exact spot, so most players found
  a silent wall of ice

---

## The Quality of Life Update — 2026-07-18 (PR #31)

### Sound & Music
- Full chiptune soundtrack: a two-voice sequencer (square-wave melody,
  triangle bass) with six original loops — title, home isle, Boothbay,
  Parklands, battle, and a dedicated legendary-battle theme
- Music picks itself by context and switches as you travel or fight
- Starts on the first tap/keypress; the SOUND ON/OFF button controls
  music and effects together

### Getting Around
- **Fast travel**: the campfire/cabin rest menu gained TRAVEL — warp to any
  fire or cabin in areas you've visited (pre-seeded from progression for
  existing saves)
- **Field map**: the C-cycle now ends on a three-isle pixel map — visited
  areas glow, trails connect them, a blinking marker shows your position;
  secret areas stay hidden until discovered

### Save Protection
- **BACKUP SAVE** at every campfire/cabin hands out your rescue code
- First-time wins over gatekeepers and rangers remind you backups exist

### Battle Depth
- **Matchup hints**: once a species is in your dex, moves show +/− against
  it and the info bar reads STRONG/weak
- **Keen Charm** (sealed cache, Thornwall Cliffs): crit chance 7% → 14%
- **Guard Pendant** (sealed cache, the Everglades): once per battle, the
  holder survives a knockout blow at 1 HP
- Item menu lists all held items and supports swapping

### Delight
- **Shiny Wildlings**: 1-in-200 spawns with fully shifted palettes, a
  sparkle entrance, and a star by their name; persist everywhere
- **Doc Bramble, collector**: rewards at 30 seen (300 coins), 60 seen
  (500 coins + 3 jam), 90 seen (1,000 coins + 5 jam), and a one-of-a-kind
  shiny gift for seeing all 104
- **Park weather**: snow over Denali and Glacier Crown, rain in the
  Everglades, heat across Saguaro — the matching element hits 20% harder

### Fixes
- Held items sitting in the bag were silently deleted on save load

---

## Parklands Phase 2 + Enhanced UX — 2026-07-17 (PR #30)

### The Great Parklands grows
- Three new parks continue the chain: **Denali Tundra**, **Saguaro
  Wastes**, **Glacier Crown**, plus the hidden **Deep Rime** ice cave
- **MAMMORIME**, the Frost legendary — "the glacier that walks" — sleeps
  behind a cracked ice wall only a ranger's badge can open
- Rangers Koda, Sierra, and Boreal guard badges 4–6
- Elemental birds return to every park at biome-appropriate levels
- New ice-wall tile for tundra and glacier interiors

### Battle feel
- **Critical hits**: 7% chance, 1.5× damage, a "A critical hit!" callout
  and a white screen flash
- **Typed attack animations**: every element hits with its own particle
  signature — embers rise, tide splashes, leaves flutter, sparks crackle,
  gale streaks sideways, rocks tumble, mystic rings bloom, frost shards
  fall, venom drips

### The dex doubles down
- **30 new species** — one full three-stage evolution line for every type
  (dex 74 → 104), seeded into wild pools across all three regions

### Pacing & balance
- The two grass patches nearest the starting cabin now guarantee gentle
  L3–4 encounters; two new standard patches compensate deeper in
- Moss Locket softened: mends 10% of max HP per turn (was 20%)
- **Frost/Tide rebalance**: chill is now exclusively Frost's (35%); Tide
  inflicts nothing; Frost moves run a hotter ladder (45/75/90) and Frost
  species became rare single-entry spawns, Mystic-style; evolved Frost
  forms no longer spawn wild
- Frost's attack animation upgraded to crashing icicle spears

---

## Parklands Phase 1 — 2026-07-16 (PR #29)

- **Region 3: The Great Parklands** — a US-national-parks-inspired
  landmass reached by ferry after becoming Harbor Champion
- New types: **Frost** and **Venom** (with poison status), wired through
  the full chart, tutor sets, and status system
- **Ranger Badges**: eight badges gate the region finale; badge screen on
  the C-cycle and at the Gateway ranger board
- First three parks: Yellowstone Vale, Everglade Sloughs, Yosemite
  Heights, with Rangers Solene, Murk, and Vespera
- Eight new species including bison, gator, and marmot lines
- Fixed the Gateway arrival trap (dock added) and hardened every map with
  traversability tests

---

## Earlier releases (highlights)

- **PR #28** — Hidden Bramble Hollow behind a false wall, home of the
  **MINOS** line: a neutral physical juggernaut that always strikes first
  and evolves into divine forms; kept the entrance truly hidden
- **PR #27** — A second, tougher roaming trainer in every area (14 total)
- **PR #26** — The **Moss Locket**: first held item, from the infinite
  supply box by Doc's cabin
- **PR #25** — Trainers announce their next Wildling after a KO and offer
  a free switch
- **PR #24** — App icon became Sylvarch, the isle's first legendary
- **PR #23** — Boothbay's redundant buildings repurposed: an all-type
  **Move Tutor** and old **Eldon**, keeper of the legendary **Primling**
- **PR #22** — Blacking out respawns at the nearest campfire or cabin
- **PR #21** — The **Bramble Bike** (double speed) and a scrollable shop
- **PR #20** — Seven replayable roaming trainers, one per area
- **PR #19** — Gold blazes mark area exits; return trails in Pinewood
- **PR #18** — Battle damage shown at animation contact, not compute time
- **PR #17** — Faint animation no longer plays on the trainer's next mon
- **PR #16** — Crisp rendering: canvas matched to device pixels
- **v0.7 and before** — Boothbay Isle postgame island, battle scenes and
  animations, move-learning choices, the obelisk, nicknames, the ranch,
  save codes, and the original three-area isle where it all began
