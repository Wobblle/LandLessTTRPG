LandLess — Wishlist v1
Drafted 2026-11-08 by Muse, from Draft 0 (2nd draft PDF, © 2025 Asleepius Games) and the decisions made Nov 8. Grok's contradiction pass and the novel manuscript are inputs this list references but doesn't restate — Muse hasn't seen either yet.
Rules of the build: the novel is lore canon. AI drafts, Jordan decides. New versions never overwrite Draft 0. Anything the tool invents that isn't in the book gets labeled house-rule, never canon.
0. The order of work
Oracle first — the bottleneck. Nothing playtests without it.
CC3 + CC5 — character creation unblocks.
Action cards starter set (20–30).
Playtest session 1 — fix the numbers from what actually breaks.
Tool core: Reader → Creation walkthrough → Oracle → Log.
Art and polish later.
1. Game mechanics — the book
Blockers (the game is unplayable without these)
CC3 — Howling Features. Tables CC3.A (animalic), CC3.B (cybernetic), CC3.C (negative traits) are referenced but missing. Need feature lists with FP costs against the 10 FP budget, descriptions, and mechanical effects. Character creation stalls at step 5 without this.
CC5 — Starting Closet. Referenced but missing. Need gear, weapons, and tools with CP prices against the 50 CP budget, plus weight, volume, and effects. Character creation stalls at step 8 without this.
Ch. VIII — Oracle mechanics. Indexed but not written. Need the actual yes/no oracle (proposal: the deck he already needs — suit = yes / no / yes-but / no-but, value = twist; Jordan's call), plus how oracle answers feed the story.
Action Cards — starter set. The resolution engine is explained; not one card exists. Need 20–30 cards with Effect Block Codes, per location / POI type.
Event tables — content. SV1 (Unconscious Events) is an empty 13×4 grid (suit themes defined, cells empty). SV2 (Death Events) says "SV3 needed" and SV3 doesn't exist. SV4 (radiation) and SV5 (weather) are headers and intros only. TE1 (Travel Events) is a framework (type + 1d6 intensity) with no entries. Fill all of them.
Rules to finish or fix
CC4 — Tactical Maneuvers. Table exists but the Quick Step / Bleed Attack rows are garbled. Rewrite.
CC1.B — Origin Snippet. The draft has a simplified example (range bands Ace–4 / 5–8 / 9–King per suit). Decide: full table, or confirm the bands as the final design.
Toughness / damage contradiction. The closing note (roll d(damage) and remove the result; ally pickup on a d6 roll of 6 → +d3 Toughness, once per fight) doesn't match the HP rules up front. One consistent rule.
Skills System chapter. Mechanics are deferred to a chapter that doesn't exist yet. Need skill checks, progression, and the Skill Prestige rules the trait system references.
Radiation / mutation. Mutation risk is currently "an Oracle-introduced narrative element." Decide: real mechanics, or explicitly narrative-only.
Weather (SV5). Needs the actual weather table, plus how weather acts as an Environmental Trait modifying Action Cards.
Lore to finish
Grok's contradiction list. Resolve each item; novel wins unless playability needs the RPG's version. Log every decision in lore-bible.md.
Novel lore → lore bible → RPG. Extract the deeper nuggets from the novel (history, places, named characters, the Wostouf contract) into the bible, then fold them into the RPG.
Factions as characters. Onyx Empire, Timberites, Rambas, Stillous Remnants are names plus one trait each. Faction standing is step 3 of character creation — each faction needs: what it wants, how it talks, what a deal with it looks like.
The Howling origin. Why do animal-people exist? Uplift? Gene-editing from the Nuclear Campfire era? The thing the player IS needs an answer.
"Howling" dual use. It's both the PC type and a faction. Rename the faction or clarify.
Retch. The survival chapter addresses a character named Retch. Decide: introduce him as the example character, or cut him.
Scope decisions (Jordan only)
Vehicles / bases / shops / banks. Described but thin. In the testable book, or later? Don't add systems until the core loop plays.
Cleanup pass. "Psh" typo in the time table, page-number placeholders everywhere, "surviver" spelling.
Playtest
Session 1 with the filled tables. Log what breaks. Numbers to watch: −20 Hunger/Thirst per Cycle, Rest −50 per Cycle, the escalating pass-out roll, the 10 FP / 50 CP budgets, the skill 0–12 range.
2. Tool UX — the oracle / manager
The tool directs, records, reminds, lets the player review, and generates world and story beats. The player rolls and draws; the tool interprets, looks up, and remembers. It never plays the game for them. Paper stays the source of truth if he prefers — the tool mirrors it.
Core (v1)
Reader. The whole book, searchable and cross-linked. Every rule carries a draft status (complete / partial / missing) so the player knows when the book itself can't answer.
Character creation, walked. The 9 steps in order. He draws physical cards and enters results; the tool applies CC1, CC2, CC4, CC6. Steps 5 and 8 flagged blocked until CC3 and CC5 exist.
Oracle. Ask a question, get an answer. Deck-based. Anything not from the book is labeled house-rule.
Log. Campaign journal (the book itself recommends one) plus a light tracker for Cycle / Phase and Hunger / Thirst / Rest / Sanity / HP. Applies per-Cycle depletion and flags thresholds.
Review. Campaign history and story beats, Cycle by Cycle.
Direct / remind. Session prompts: survival checks per Phase, rest tracking, what to do next.
Later
Event and item art. Small field-guide illustrations, not cutscenes.
Sound. Tiny terminal blips, toggleable.
Discord bot as a second surface. Community / shared campaigns only — never the core.
3. Style
The tool is an in-world artifact. A salvaged field terminal / ship's computer — the living book made literal.
The draft's own style guide: retro-futuristic brutalism, high-contrast monochrome, CRT amber and green, JSON schemas, bug-report styling.
Oracle voice: terse, procedural, slightly cold. A system, not a chatbot. The book already calls the player Howling and survivor — the tool talks like that.
Imagination aids, small. One sensory hook per event ("salt wind, diesel, a distant klaxon"). Small field-guide art. The player's imagination does the work; the tool gives it something to chew on. Never a wall of generated prose.
Phone-first, one-thumb layout, dark screen. One hand free for dice. Plays at night without killing night vision.
Version stamp on every page. Draft 0 → Draft 1, and so on. The tool and the book read the same files, so they never disagree.
4. Stack
Web tool, installable PWA, phone-first. Zero-install link sits next to the grid paper. Offline via PWA cache after first load.
Content as data. The book's tables as JSON / markdown in the repo — the single source of truth feeding both the book and the tool. Change a table once, both update.
Folder:
landless/
  book/         novel + rpg manuscripts, markdown
  lore-bible.md lore canon, extracted from the novel
  content/      tables, oracle, items — JSON, one source of truth
  app/          the PWA
  wishlist.md   this list
Build: Grok in Cursor for the app; local AI (Ollama / Beam while free) for finishing the documents.
Vercel: dropped for now. Pro trial decision Nov 21; hosting later only if the deploy loop earns it.
Not Godot for this tool (save Godot for Drifters — the feel there is the game). Not a Discord bot as the core (a chatroom is not a reading surface).
