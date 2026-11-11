# LandLess — Design Directions

Recorded Nov 10, 2026, from the table sessions. Draft 3 is the rules; this document records the design shifts, the plain-language breakdowns, and tonight's generated chart so the work transfers to the PC build.

## Status

- Rules: Draft 3 (`book/LandLess-RPG-Draft-3.md`) is the current rules. The 2025 PDF is the archive. Draft 3 wins where they disagree.
- The LandLess Oracle space is the prototype. The GitHub mobile webpage is the real product Jordan owns.
- Teaching rule used throughout: plain words first, abbreviations only after the plain word. Jordan's own confusion during revisions is treated as useful data on the game's clarity — if the author can't hold a rule, a new player can't either.

## 1. The hidden-state mechanic (NEW — Nov 10)

The design shift from the Nov 10 table play.

- Paper and the app both track character stats and details. When they disagree, the app (the digital version) is the reference.
- Ship damage is hidden. The player tracks what they THINK the damage is on paper. The app holds the ACTUAL damage. The player must visit a mechanic to reveal the actual damage.
- Events go through the app. When a result happens, the app reveals the actual outcome. Example: a player takes 5 damage, thinks they have 1 hull left, but the actual damage was higher — the app reveals the ship is destroyed when the result lands.
- Design intent: the gap between what the player believes and what is true is itself the mechanic. Paper is the player's fallible record; the app is the arbiter.
- This applies to ship damage first. Whether it extends to other meters is an open decision.
- Open decision: which mechanic, and what it costs to reveal the actual damage.

## 2. Input system (NEW — Nov 10)

- When a dice or card result needs to be processed digitally, it comes in as input to the app.
- Moving to a tile: the app needs the input to build the map. Each map element needs an input.
- Cards: draw a physical card, then enter the suit and rank into the app (for example, 9 of Diamonds).
- Dice: enter the result by clicking or tapping the dice in the app (or typing the number).
- The app processes the input: it generates the map element, applies the result, and updates the true state.

## 3. The app (NEW plan — Nov 10)

- A mobile-focused webpage, hosted on GitHub, built on Jordan's PC. Used at the table while playing.
- Paper stays the primary surface (maps, sheets, tokens). The app is the DM and reference, and the holder of true state.
- The LandLess Oracle space is the prototype for the app's behavior; the GitHub page is the version Jordan owns and builds.

## 4. Rules breakdowns (plain language, from the Nov 10 teaching sessions)

### Session 1 — The game in one breath, and what a turn looks like

You are a Howling — an animal-like person with scavenged cybernetics — on a drowned Earth in the early 2600s. The oceans rose. Cities float on scrap. You live on a boat. You sail between floating places, scavenge, trade, survive. The Rivals race: two boats, first to get a ticket off the planet wins. A ticket costs 80 Scripts, the money. Or you find one in hand.

The game moves in phases. Morning, midday, evening, deep night — four phases make one day, which the book calls a cycle. In each phase, each boat does the same thing: say where you are heading, roll two six-sided dice for the sea, move as far as your boat goes, and play whatever place you land on. If both boats end up on the same hex, one interference card is drawn — the other boat gets in your way.

The sea roll — two dice, added together: 2, a ship stops you. 3, something stops you. 4, your boat strains and stops. 5, hard weather — half speed, and you lose 5 Thirst. 6 or 8, weather — half speed. 7, clear — full speed. 9, fair — full speed. 10, you find 2 scrap. 11, a hulk you can scavenge once. 12, flotsam worth 10 Scripts.

Your body's numbers: Toughness is your health, starts at 15. Hunger starts at 70. Thirst starts at 70. Rest starts at 80. Sanity starts at 50 (how steady your mind is). At the end of each day: Hunger drops 20, Thirst drops 20, Rest drops 50. A ration gives back 25 Hunger. A water gives back 25 Thirst.

The dice you need: two six-sided dice for the sea and most checks. Bigger dice — 8, 10, 12 sides — only when you take a big hit. The cards: one deck of 52 playing cards, jokers out. The cards build the world, answer yes-or-no questions, and decide some events. You draw them when the game tells you to.

Map legend: X means closed, a door that won't open. W means work, a yard or workshop. H means beds, somewhere to sleep. + means hazard, something dangerous. D means dock, where a boat waits. B is a bar. K is mechanical, machines and parts. T is trade, a shop.

### Session 2 — Character creation (Rivals quick build)

Seven steps, in order. You need two characters, one each.

1. One sentence. Who you are, and why you want off the water. In the full game this is a drawn origin card; tonight the sentence replaces it.
2. Skills. You start with Piloting 1, Scavenging 1, and one other skill at 1. Everything else is 0. The book has twelve skills, in four groups: fighting — Melee, Ranged, Demolitions; technical — Engineering, Hacking, Piloting; social — Barter, Persuasion, Medicine; field — Athletics, Stealth, Scavenging. When you try something risky, roll two six-sided dice and add the skill. 6 is routine. 8 is risky — fail and it costs you a segment or starts trouble. 10 is extreme — fail and you take harm or raise an alarm. Roll two sixes and you mark a tally beside the skill; when your tallies equal your skill level plus one, the skill goes up by 1 at your next full rest.
3. The meters. Toughness 15, Hunger 70, Thirst 70, Rest 80, Sanity 50, Bio-Energy 10 (fuel for your cybernetics), Battery 0, Radiation 0.
4. Feature Points — 6 to spend. Features are the animal and machine parts of your body. Gills and Webbing, 4 — you breathe water, and water doesn't slow you down. Raptor or Feline Claws, 3 — a natural weapon, always with you, and you're better at climbing. Bloodhound Olfaction, 3 — a sharp nose, Scavenging plus 1, and it teaches you the Heightened Alertness maneuver. Toughened Hide, 4 — plus 1 armour, and your Toughness max goes up by 2. Nocturnal Tapetum (night eyes), 2 — you ignore darkness penalties at night and in unlit wrecks. Two drawbacks give points back: Sunlight Sensitivity gives 2 back (clear midday sun makes your checks worse), Loner gives 2 back (you're worse at persuading and bartering).
5. Gear — the pack. Satchel (carries your things), rust-shank (your blade), tarp vest (what you wear for armour), 2 rations, 2 waters, 15 Scripts.
6. Escape card. Each draws one card before the boats, suit only. The app holds what the suit means.
7. Maneuvers. Only Bloodhound gives you one tonight (Heightened Alertness). Otherwise, none in the quick build.

The full game, for later, is a 9-step creation in chapter 2 — origin card draw, faction relationships, 10 Feature Points, skills, 2 maneuvers, 50 Closet Points of gear to buy. The quick build is the short version of that.

### Session 3 — Boats

Your boat is your home, your transport, and your health on the water. Hull is the boat's health. Armour Value is how much damage the hull ignores. Speed is how far it goes per watch. Then the hold (how much it carries) and the fuel tank.

You have 8 Boat Points. Pick a hull, spend the rest.

- Raft, 2 points. 10 hull, 0 armour, 1 hex per 2 watches. Hold 50 kg / 20 vol, no mod slots, no engine, no fuel.
- Skiff, 4 points. 20 hull, 1 armour, 1 hex per watch. Hold 150 kg / 60 vol, 1 mod slot, tank 10.
- Cutter, 7 points. 35 hull, 2 armour, 2 hexes per watch. Hold 300 kg / 120 vol, 2 mod slots, tank 10.
- Hauler, 8 points. 60 hull, 3 armour, 1 hex per watch. Hold 1000 kg / 500 vol, 3 mod slots, tank 10.

Leftover points: 5 fuel costs 1 point, plus 5 hull costs 1 point, a modification costs 2 points. The modification list is in chapter 10.

Fuel: 2 Scripts a unit at any dock. A powered hull spends 1 fuel per phase underway. At 0 fuel, a skiff, cutter, or hauler moves as a raft until it refuels. Rafts never spend fuel.

Speed per phase — a phase has 3 watches: skiff and hauler cover 3 hexes per clear phase, cutter covers 6, raft covers 1.

Quirk: draw one card after building. Hearts means extra bunks, somewhere to sleep aboard. Diamonds means a larger hold — add half the listed hold again. Clubs means a leak — lose 1 hull at the end of every cycle. Spades means a deck gun you cannot fire yet — write the slot down.

A hull you find is generated with two cards — the first suit is the hull (hearts raft, diamonds skiff, clubs cutter, spades hauler), the first rank is its condition (ace through 4 failing, 5 through 10 working, face sound). Failing hulls have three quarters of the listed hull points; sound hulls have plus 5 and one extra mod slot.

### Session 4 — Maps

Three scales, and you only ever use one at a time.

The globe is the world map: one flower, 217 hexes. Each hex on the globe is a region. You sail across the globe from region to region. The working grid is columns A to Q, rows 1 to 17, center I9. You only ink a hex you enter, buy a chart of, or someone swears they've been to. The corners of the grid are just paper — only the flower cells are real hexes.

The region is what a globe hex becomes when you enter it: 37 hexes in a flower, columns 1 to 7, rows A to G, center D4. The first time you enter a globe hex, you generate its region. First, place any secret that named this region, in the sector it named, and date the sheet with the cycle. Then draw four cards for the other places, minus one card per secret you already placed. Each card is a place: the suit says the kind — hearts is a berth, diamonds is a market, clubs is trouble, spades is closed. The rank says the size — ace through 4 is 3 local hexes on 1 region hex, 5 through 10 is 6 local on 2, a face card is 9 local on 3. Place them roughly by sector.

The place is the local cluster: when you walk into a place, you build its cluster out of small hexes, side by side. Deal one card per local hex to fill it. The card gives you a symbol (see the legend in Session 1). One hex on the outer edge is the dock, where the ship waits. Walking one local hex takes 1 Action Turn, and you have 4 Action Turns per watch.

From here, generate on discovery: a region gets drawn the first time you enter it, a cluster only when you walk into it.

### Corrections (Draft 3 wins)

- Leak (clubs quirk): 1 hull at the end of every cycle, not every phase.
- Spades quirk: a deck gun you cannot fire yet, not a refusal.
- Rest starts at 80 in the quick build (100 in the full game).
- Feature names are the book's: Raptor/Feline Claws, Gills and Webbing, Bloodhound Olfaction, Toughened Hide, Nocturnal Tapetum, Sunlight Sensitivity, Loner.
- Fuel: a powered hull spends 1 fuel per phase underway; at 0 fuel it moves as a raft; rafts never spend fuel.
- Checks: roll 2d6 and add the skill. 6 routine, 8 risky, 10 extreme. Two sixes is a tally.

## 5. Tonight's chart (generated Nov 10 by deck draw)

Grid: columns A–Q, rows 1–17, center I9. All draws from one shuffled 52-card deck, no jokers.

### Port Dundy — J12

Southern edge of the Howling pockets. Dundy is the secret of its region, sector S — write that down so it doesn't move. The region's other three places, roughly placed:

- JH — berth, 9 local on 3 region hexes — NE. A second city-sized anchorage in the same region.
- 9D — market, 6 local on 2 — W.
- 7C — trouble, 6 local on 2 — NW.

Dundy's cluster, 9 hexes (deal: QS, 6D, KC, QH, 7D, 8D, 9S, 4S, 10D):

```
X  W  X
W  H  W
+  W  X
      D (ship's dock, south edge)
```

A working port: mostly work yards, closed doors, one place to sleep, one hazard. Services run at the book's prices — fuel 2 a unit, beds 2 a phase, yard 5 per 5 hull.

### Start A — E9

Rhombus pocket, due west. The dock is the secret of this region, sector center, a 6-hex cluster, closed except the slip. The region's other three, roughly:

- 7S — closed, 6 local on 2 — NE.
- 6C — trouble, 6 local on 2 — SE.
- 8S — closed, 6 local on 2 — W.

The dock cluster — slip plus the deal (JS, 3S, JD, 6H, AS):

```
D  X  +
+  K  B
```

Slip is the D on the outer edge, the way out. The rest: closed hatch, hazard, mechanical bay, bar, hazard.

Path A to Dundy (5 hexes, southeast): E9 → F10 → G10 → H11 → I12 → J12.

### Start B — E14

Second Rhombus dock, southwest, far enough from A that the two rivals don't share water at the start. Dock secret, sector center. The region's other three:

- AH — berth, 3 local on 1 — NE.
- 2C — trouble, 3 local on 1 — E.
- 9C — trouble, 6 local on 2 — SW.

The dock cluster — slip plus the deal (QD, 4H, KS, 4C, 10H):

```
D  K  D
+  X  B
```

Slip is the outer D you leave from; the dealt D is a second berth inside the cluster.

Path B to Dundy (5 hexes, northeast): E14 → F14 → G13 → H13 → I12 → J12.

Both paths are 5 hexes. A skiff covers 3 per clear phase (two phases), a cutter covers 6 (one phase), a raft won't make it in a day. The sea roll governs the crossing.

## 6. Sheets

- ASCII character sheet and ASCII boat sheet (plain text, copy-pasteable into Google Docs, no wrapping). Jordan combined them into one hand-drawn sheet on Nov 10 — character and boat on the same page.
- The LandLess Oracle space mirrors the combined sheet: each rival's PLAY card is one character-and-boat card (meters on top, boat block below, hold in kg and volume, mods list, Boat Points budget line).

## 7. Open items

- Sessions 5–7 (deck, trouble, ports and people, the full game) are in the space's LEARN tab; fold them into the book and the app as needed.
- The cipher (chapter 11): a word-count code, with 6-pocket and 12-pocket log layouts. The sentence itself is not written here — see the book, and never read it aloud.
- The secret frame: see `book/SECRET-Rivals-Frame.md` — DM-only, reveal beats only on their triggers.
- The mechanic-reveal rule (section 1) needs a price and a place: which mechanic, what it costs to reveal actual damage.
- The space (LandLess Oracle) is the prototype; the GitHub mobile webpage is the real product.
