# Wildling Isle — Change Log

All notable changes to the game, newest first. Each entry corresponds to a
release merged to the live game.

---

## Save Codes on Mobile — 2026-07-18 (PR #36)

### Fixes
- **Save codes on mobile**: CODE used to drop the ~300+ character save
  code into a `window.prompt()` box — a single-line field that's
  essentially unusable for select-and-copy on a phone. It's now a real
  in-game overlay: the code sits in a large, word-wrapped, pre-selected
  textarea, gets copied to the clipboard automatically the moment it
  opens, and a dedicated **COPY** button is right there if the
  automatic copy didn't take (with a "Copied to clipboard!"
  confirmation). Loading a code got the same treatment — **PASTE** a
  code into the box and tap **LOAD**, no more typing into a tiny prompt

---

## The World Update — 2026-07-18 (PR #35)

### The character pass — no more squares
Six parks were rebuilt from the same mirror-box template into places
with real shape:
- **Yellowstone Basin**: terraced hot-spring pools behind two ridge
  walls with offset gaps — wind through the terraces
- **Everglade Sloughs**: mostly open water now, crossed by a creaking
  boardwalk ring with grass islands — rain on the planks
- **Yosemite Heights**: three sheer wall bands with offset breaks — an
  honest switchback climb to Vespera's gate
- **Denali Tundra**: braided ribbons of ice snake across the tundra
- **Saguaro Wastes**: scattered saguaro cacti (a brand-new tile) among
  dune mounds
- **Glacier Crown**: jagged crevasse lines to thread on the way to the
  cracked ice

### More rivals on the road
Seventeen new roaming trainers — every area now fields one more, from
Picnicker Berry in the meadow (you stepped on her blanket) to
Crownstone Keeper Frost at the summit. All replayable; total roster
now fifty

### Gateway Basecamp — the hub becomes a village
- **The Ranger General Store**: Golden Orbs (double-charm catch odds),
  Cinder Salts (the game's first revive), Repel Whistles (150 quiet
  steps), and the Prism Bell (7,500c held item — shinies come twice as
  often while anyone carries it)
- **The Nursery**: board up to two Wildlings; they earn a quarter share
  of XP from every battle you win while boarding. The building opens
  the full storage screen — team, ranch, and nursery side by side, one
  press to move anyone between them. Pickup fee scales with levels
  gained
- **The Master Tutor** (the old visitor lodge): ten exclusive songs —
  one per type, each with a real effect (draining Lifebloom, guaranteed
  chill Deep Freeze, the Bulwark Hymn stance...) at 1,200c apiece.
  Zero overlap with the Boothbay tutor
- The hub itself became a village: lodge row, store, nursery pens,
  flower plaza around the ranger board, and the postmaster now does his
  rounds by the south lawn

### Balance
- **Stooping Gale buffed** (95 pow, was 90; +15% crit, was +5%): the
  new Master Tutor's Slipstream (Gale, +10% crit) was mathematically
  outcritting Skywarden's own signature move despite being purchasable
  by anyone. Stooping Gale now clearly leads its type on both power and
  crit, and a permanent regression test checks every legendary
  signature against every master song so no future addition can quietly
  outclass one again

---

## Parklands Phase 4: The Summit — 2026-07-18 (PR #34)

### The Summit
- **THE SUMMIT** crowns the region: a snowbound peak above the Great
  Rim with elite wilds (L60–64), two trainers, and the crown-stone camp
- **SUPERINTENDENT VANCE** — the region finale. Five elite Wildlings at
  L61–64, and the gate itself refuses anyone carrying fewer than all
  eight Ranger Badges
- Victory names you **PARK WARDEN** — the title marks your save file
  and the badge hall
- Ranger Talus's trail north now truly opens after the eighth badge

### Battle
- **Divine Horns** (Celestaur's signature) now gores true: +10% critical
  hit chance on top of the base rate — and it stacks with the Keen Charm
- **Every legendary now carries a one-of-a-kind signature move:**
  - *Verdant Reign* (Sylvarch, Mystic 85): drains half the damage dealt
    back as HP — the forest reclaims
  - *Glacial March* (Mammorime, Frost 80): chills without fail — the
    cold is not optional
  - *Stooping Gale* (Skywarden, Gale 90): never misses and carries a
    +5% crit edge — the dive is true
  - *First Law* (Primling, Wild 110): the hardest-hitting move in the
    game — the oldest word
- **Titan Stance** (the Minos line, learned at 14): raises the user's
  Attack AND Defense by 50%, stackable twice per battle — unmovable,
  then unstoppable. The move menu explains buff moves in plain words

### Interface
- **Move inspection**: the Wildling info screen gained a move cursor —
  up/down highlights each move and a description bar explains exactly
  what it does ("+10% crit chance", "drains 50% of damage as HP",
  "always chills the target", "25% chance to shock"...). Moves with
  special effects glow gold in the list
- The battle move bar and the learn-a-move prompt show compact effect
  tags too, so nothing special hides behind a name

---

## Parklands Phase 3 — 2026-07-18 (PR #33)

### The old growth and the great rim
- Two new parks extend the chain past Glacier Crown: **REDWOOD EXPANSE**
  (walk among giants) and **THE GREAT RIM** (a mile of stone below the
  railing, heat shimmering off the ledges)
- **Rangers Sequoia and Talus** guard badges 7 and 8 — all eight Ranger
  Badges are now earnable; the Superintendent's summit trail teases at
  the top of the Rim
- **SKYWARDEN**, the Gale/Mystic legendary — "the wind that watches" —
  circles the Rim's high aerie. The perch only answers to the eighth
  badge, and the whole aerie responds (lesson learned from Mammorime)
- Six new natives: Wapituft → Thornelk (the walking thicket), Scavren →
  Condorge (Gale/Stone canyon shadow), Mossgrizz (the forest that
  growls), and Echowing (the voice in the dark rim). Dex 104 → 111
- Four new roaming trainers, campfires, weather, and elemental birds in
  both parks; the field map grew two nodes
- **The Gateway visitor lodge is now a Move Tutor** — full song access
  without sailing back to Boothbay

### Fixes
- Rangers Vespera (Yosemite) and Sequoia (Redwood) could be walked
  around via the open row beside their gates — the passes are now true
  chokepoints, and a permanent test guarantees every gatekeeper
  actually blocks a road
- Entering the Great Rim from Redwood dropped you at the top of the
  park, face-to-face with Ranger Talus — arrivals now land at the
  south entrance like every other park

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
