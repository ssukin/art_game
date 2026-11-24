# Sarah and the Fading World: Story and Handoff Notes

This file gives an AI (or a person) picking up the project everything needed to keep working on it: the plot, what's built, how the code is organized, and how Sarah (the game's creator) likes to work. The player-facing walkthrough is in `README.md`.

---

## 1. How Sarah likes to work (read this first)

- **Don't change the game until she says to.** If she asks for suggestions, ideas or a brainstorm, only suggest. Build only when she clearly asks ("start build", "add …", "make it so …").
- **Never push to GitHub on your own.** Only push or merge when she says so. "Push" means: commit on a branch, open a PR, merge into `main`, then check that `index.html` on `main` matches the local file.
- **Only send emails when she specifically asks.**
- **Test every change** in a real browser (Playwright) before handing it over, and look at screenshots.
- **Save to her local folder for testing:** `C:\Users\sarah\OneDrive\Documents\ChatGPT\Game`. Her test link is `file:///C:/Users/sarah/OneDrive/Documents/ChatGPT/Game/index.html`. After saving, check the file sizes in the folder match.
- **Keep ideas simple.** She dislikes over-built plot ideas and invented lore. Don't add new story facts that she hasn't agreed to. When unsure, ask.
- She plays the game and reports specific fixes. Make exactly those, don't redesign around them.
- Update `README.md` whenever gameplay changes.

---

## 2. The project

- **Repo:** `ssukin/art_game` on GitHub. Current working branch: `claude/project-thread-eqpv2o` (Chapter 2-1). The older `paper-style-overhaul` branch is fully merged. GitHub Pages serves `main`. Sarah's rule: push to the working branch as you go, but never merge into `main` until she says so.
- **Files:** the whole game is one file, `index.html` (about 334 KB, canvas + plain JavaScript, no libraries, no image files). `README.md` is the player guide. `movement_test.html` is an old prototype kept for reference.
- **Look:** inspired by Super Paper Mario (paper cut-out characters, cardstock scenery, comic speech bubbles, gentle jokes). **No Nintendo characters or IP.**
- **Canvas:** 960×540. Ground line `G=440`.

---

## 3. Story (what's decided)

- The world is one big **sketchbook**, and every place is a page.
- **Sarah** is a young artist. Her paintbrush buddy is **Dab**.
- **Professor Monochrome ("Monty")** is the villain. Long ago he painted with **Grandma** and **Dab**. He went gray and now **tears pages out of the sketchbook world**. Each torn-out page becomes a **door** on the festival's second floor (six doors, all visible from the first visit).
- **Grandma** is connected to Dab and Monty's past. She is **not missing**, and Sarah is not searching for her (Sarah decided this on 2026-11-23).
- **The Great Sketchbook** in the library tracks the six pages/doors and which are restored.
- Monty is glimpsed before any reveal: a gray figure on a far hill (Level 0 Part 1 storm), a gray-gloved hand in the sky tear (Part 2), and a figure in a gray top hat rowing away with a tiny squid after the Level 1 boss.

### Story points that need Sarah's decision (open)

- **Why Monty went gray.** The game and README currently say **Mr. Biscuits (the cat judge) gave Monty's festival painting a terrible review**, and that's what turned him gray. **Sarah said this is wrong.** It appears in Mrs. Maple's hub dialogue and the README "story so far" paragraph. Ask Sarah what the real reason is before changing it.
- **Quill** (a librarian added outside the library who shows the Great Sketchbook after Level 1). Sarah asked "who is Quill?" and may not want this character. Mrs. Maple could show the sketchbook instead. Confirm before changing.

---

## 4. Game structure (hub and spokes)

- **Level 0 = the town (the hub).**
  - **Part 1: Home and the road.** Bedroom → road → storm, a gray crying flower, Smudges → Mrs. Maple's house → free **Dab** from Grandma's chest → restore the flower → Town Gate Key → gate.
  - **Part 2: The Festival.** Orchard + registration → festival → optional art contest (make a **Ball of Clay** or **Lopsided Teapot** at Potter Pat's **Clay Corner**) → free **Mr. Biscuits** from the jungle gym with butter → Brie's chase → find **Nib** (pencil buddy, Q jabs) → beat **Prickles** → contest results (Juniper's painting looks like Sarah and Dab) → sky cracks, Smudge fight → Mrs. Maple's **balloon dog** floats Sarah up to the **second floor** → unlock the first door.
  - Side areas: the lake (Waffles the dog, fishing), the hole into **Undertown** (bar, Grimy Grotto, shops, a dinosaur fossil stuck in the dirt, a sewer tunnel), Chef Crumb's recipes, Inka's balloons, the library roof chest and sky clouds with a fairy.
- **Second floor:** a long sky walkway with 6 door slots, `DOOR_SLOTS=[3380,3000,2620,2240,1860,1480]`. Gus's elevator is at the left end.
- **Level 1 = the Watercolor Coast** (door 1, right end).
  - **1-1 Beach:** Marina the hermit crab (trades 3 Seashells for the Shell Shield, blocks 2 hits), digging with Dab (Heart Necklace = **Red gem**), Tide Flats, hidden dock painted back with Dab, shipwreck chest = **Reel** (fishing-pole buddy), fish until you hook the **Blue gem**.
  - **1-2 Gray Lighthouse:** vertical climb, moving and crumbling platforms, ink drips, hidden **Green gem**, boss **The Blot** (giant ink squid). Light the lamp with Red, Green and Blue to restore the coast.
  - The lamp's beam points home. Dab explains that a whole page shines its light back through its door like a bookmark. Sarah rides the beam home.
  - **Replayable** from its door: no boss, gems already in place, ride the beam home at the top.
- **Back in town after Level 1:**
  - The beam drops Sarah out the page door. Gus's fixed elevator brings her to the ground floor. Gus explains the festival is over and some shops have reopened.
  - (Old notes said Dab and Mrs. Maple tell the Grandma/Monty story here. Sarah removed that on 2026-11-24.)
  - The festival is packed away (stage, sculptures, registration, bunting, Clay Corner booth). **Chef Crumb's Kitchen and Inka's Art Supplies stay open.** Mr. Biscuits sits outside the pet store. Closed shops say **ON VACATION**.
  - **Open shops have interiors** (walk in, talk to the keeper behind the counter): Paws & Claws (Polly: Dog Food, Bait), Odds & Ends (Mr. Tally: buys almost any non-key item), Lost & Found (Mr. Pocket: Old Sketch), Arcade (Pixel: "Stop the Smudge" mini-game), Alchemy (Madame Fizz: fish + seashell → Health Potion).
  - **Gus** gives the welcome-home speech (festival over, shops reopened, take the new fishing pole to the lake). Then **Mrs. Maple** comes over and asks Sarah to pick up the clay delivery through the second door whenever she's ready (`l2.clayErrand`). Sarah decided (2026-11-24): no Grandma / Professor Monochrome story after Chapter 1. Quill and the sketchbook are optional now.
- **Level 2 door** (door 2) is unlocked once Level 1 is done and leads to Chapter 2-1 once Mrs. Maple has given the errand. Doors 3–6 are padlocked.
  - Still closed on purpose: Grimy Grotto, orchard apples, the mysterious gate.

---

## 5. Systems

- **Buddies:** Dab (Q reveals hidden doodles and paints things back), Nib (Q jabs), Reel (fishing). E swaps.
- **XP and levels:** creatures give XP; on level up the game freezes with confetti, +5 max health and a full heal. A **Journal** tab tracks creatures.
- **Fishing:** lake has Lake Perch / Sunfish / Catfish / Golden Koi; sea has Sea Perch / Sea Bass / Pufferfish / Swordfish. **Bait** (Polly, 3 for 5 coins) makes bites faster and rare fish likelier.
- **Selling:** Mr. Tally at Odds & Ends; prices are listed in the README.
- **Saving:** only at **Save Blocks** (Sarah's choice; no autosave). Saved to the browser (localStorage key `sarah-fading-world-save-v1`). On reload: Continue / New Game. Continue puts you at the last Save Block. **Download save / Load save file** buttons back up to a `.json` file.
- **Inventory ("Pockets"):** Items, Key Items, Buddy, Journal, Hints. Opening it freezes the world.
- **Admin cheats:** a collapsed "Admin Cheats Only" panel under the game with jump-to buttons for testing (Level 0 parts, hub, Level 1 sections, shop, clear save, coins, level up).

---

## 6. Level 2

### Chapter 1 hoops (added 2026-11-24, Sarah's idea)
Past the shipwreck, the old rock run was replaced by Reel hoops on poles (same look as the 2-1 ferry hoops). A gray sign on the last rock is revealed by Dab as a picture-only hint, with no other written hints. There are 3 pull hoops over open sea (Q hooks one and pulls Sarah to hang from it, Down drops, grip slips after about 2.6s), then a swing hoop over an unjumpable pit before the lighthouse (hook in mid-air, pump with Left/Right, Up/Q lets go). The lighthouse door moved to x=6330. Cheat: "L1: hoops before the lighthouse".

### Chapter 2-1: The Road to the Clay Store (built)

Built from Sarah's `walkthrough.docx` (in her local Game folder). Summary: landing with the return door (TO TOWN) → secret chest to the left (20 coins + Health Potion) → villager (gray-clay hint) → faded sign at the fork (Dab) → peek at a walled-off chest → pottery yard (two rows of tipping shelves, cracked pots you stomp or head-bump) → narrow passage with clay creatures (stomp or jab) and crumbling ledges → downhill rolling clay road with shelter platforms → hidden nook (crawl under the footprint shelter; Dab doodle stairs; 10 coins + Bait ×3) → collection pit crossed on cracked planks → canal ferry (Reel hooks the ferry's ring to call it; from the ferry, Reel hooks the hoop on the other bank to pull across; works both ways; gulls swoop during the crossing) → far bank (fishing dock with canal fish, coins under the canal-side steps, faded staircase restored by Dab) → upper village climb over a pit on crumbling slabs → wide landing fight → uphill delivery lane (balls roll toward Sarah) → teapot gang (revenge for the broken pots; dialogue choices; most answers fight now, but deny twice and blame the person at the beginning of the floor and the fight comes after the store and ends 2-1) → courtyard → Clay Store (dialogue choices with the Shopkeeper, Clay Order key item) → the gray-hatted stranger tears away the return door, seen in a "far below" inset → shopkeeper points past the kilns → "Chapter 2-1 complete!". Sarah stays in 2-1 afterward; the path past the kilns is still being drawn.

- Sarah's decisions: Nib only jabs unless a creature's spec says it flips (clay creatures do NOT need flipping, per her 2026-11-24 change); teacup and teapot monsters take 2 hits (crack, then break), the gang's big teapot 5 and its teacups 3; no shovel yet; the left chest has 20 coins.
- Sarah's playtest changes (2026-11-24): fewer signs, and sign text must fit its board; less explaining of what to do in each section (especially the delivery road); dialogue choices with the Shopkeeper; **Monty is not named in 2-1** (he's just a mysterious stranger in a gray top hat); the ferry is crossed by hooking a hoop on the far bank, both ways; gulls like Chapter 1's during the ferry; **no Save Blocks in 2-1, and never save without a Save Block** (respawn checkpoints only); more and longer cracking/falling platform sections.
- Mrs. Maple's hub story (which named Monty) was removed on 2026-11-24. The Lost & Found **Old Sketch** still names Monty and Grandma.
- Still to plan: Chapter 2-2 and beyond (where Monty went, the shovel, digging, clay puzzles).

### Older Level 2 notes (before the walkthrough)

Sarah wants it to include **digging** and a **clay** mechanic that ties back to the festival's Clay Corner (where you could make a Ball of Clay or Lopsided Teapot). Keep it simple. Latest simple draft (not approved yet):

- **The Clay page:** a page Monty tore out, dried out and gray.
- **2-1 Dig Site:** find a **shovel** (an item, not a buddy). Dig mounds for clay and coins; dig through soft dirt.
- **2-2 Clay Cave:** clay puzzles (fill a gap, press a heavy button). Your festival clay piece helps (the ball rolls onto a button, the teapot pours water to soften dried clay). If you didn't make one, a pottery wheel in the cave lets you make it.
- **Boss:** a big gray clay creature; dig out its weak spots. Then a Monty glimpse and ride home.
- **Open questions for Sarah:** Is the festival piece the main solution or a shortcut? Should the shovel also unlock digging in town (e.g., the Undertown dinosaur fossil)?

---

## 7. Code map (index.html)

- **Drawing helpers:** `cut(build, fill, opts)` paper shapes; `sprite(cx, footY, w, h, draw, opts)`; `npc(name, x, face, dy)`; `LOOKS` (character looks); `NPC_X` / `SCENE_NPCS` (speech bubble positions); `iconArt(name)` item icons; `shopFront(...)`, `booth(...)`.
- **Dialogue:** `start(pages, done)`; each page is `[speaker, text, choices?, onPick?]`.
- **Inventory:** `addItem`, `useOne`, `removeItem`, `has`, `count`; item text in `INFO`; `KEY_ITEMS`.
- **Scenes:** `scene` = bedroom, resident, outside, orchard, festival, lake, under, shop, beach, lighthouse. `goScene(name, x, y)`. Interactions are in `getInteract()` → per-scene `…Interact()` functions returning `[label, fn]`.
- **Levels:** `level` is 1 = Level 0 Part 1, 2 = Level 0 Part 2 / hub, 3 = Level 1, 4 = Level 2 (Chapter 2-1). State objects: `l2` (festival + hub, `l2.hub`, `l2.hubStep` 0–3) and `l3` (coast).
- **Hub module** (search "HUB — coming home"): `returnHome()`, `hubInteract()`, Mrs. Maple, Quill/sketchbook, shops, arcade mini-game, cheats.
- **Chapter 2-1 module** (search "CHAPTER 2-1"): scene `clay` (the long village page) and `nook`. The ground there has slopes and cliffs, so it comes from `CL_FLOOR` / `floorAt(x)` instead of `G`, with gaps in `CL_GAPS`. Platforms `CL_PLATS`, pots `CL_POTS`, coins `CL_COINS`, creatures `CL_FOES`, clay-ball chutes `CL_SPAWN`, state `l4` (saved via `CL_KEEP`). The Clay Store interior reuses the shop system (`SHOPS.clay`).
- **Shops module** (search "shop interiors"): `SHOPS`, `enterShop`, `shopInteract`, `drawShop`.
- **Fish/bait/store/saving module** (search "FISH TYPES, BAIT"): `FISH`, `rollFish`, `SELL`, `tally()`, `saveGame`, `applySave`, title menu, download/upload.
- **Checkpoints:** `checkpoint` (x), `checkpointY`, `checkpointScene`; R returns there.
- **Overlays that freeze the game:** `lvlUp`, `mini` (arcade), `book` (sketchbook), `titleMenu`, inventory.
- **Test hooks:** `window.__game` (getters for state plus helpers like `tele(x, scene)`, `teleY(x, y)`, `returnHome`, `saveGame`). Cheat panel must be opened in tests: `document.querySelector('details.cheats').open=true`.

---

## 8. Status

- Everything in sections 4–6 is built and tested, and saved in Sarah's local Game folder.
- Chapter 2-1 is on the branch `claude/project-thread-eqpv2o`, not merged into `main`.
