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

- **Repo:** `ssukin/art_game` on GitHub. Working branch: `paper-style-overhaul`. GitHub Pages serves `main`.
- **Files:** the whole game is one file, `index.html` (about 334 KB, canvas + plain JavaScript, no libraries, no image files). `README.md` is the player guide. `movement_test.html` is an old prototype kept for reference.
- **Look:** inspired by Super Paper Mario (paper cut-out characters, cardstock scenery, comic speech bubbles, gentle jokes). **No Nintendo characters or IP.**
- **Canvas:** 960×540. Ground line `G=440`.

---

## 3. Story (what's decided)

- The world is one big **sketchbook**, and every place is a page.
- **Sarah** is a young artist. Her paintbrush buddy is **Dab**.
- **Professor Monochrome ("Monty")** is the villain. Long ago he painted with **Grandma** and **Dab**. He went gray and now **tears pages out of the sketchbook world**. Each torn-out page becomes a **door** on the festival's second floor (room for six doors).
- **Grandma** went after Monty years ago and is **missing**. Restoring pages brings Sarah closer to finding her.
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
  - Dab recognizes the man in the rowboat; Mrs. Maple tells the Grandma/Monty story; the sketchbook is shown; a second door appears.
  - The festival is packed away (stage, sculptures, registration, bunting, Clay Corner booth). **Chef Crumb's Kitchen and Inka's Art Supplies stay open.** Mr. Biscuits sits outside the pet store. Closed shops say **ON VACATION**.
  - **Open shops have interiors** (walk in, talk to the keeper behind the counter): Paws & Claws (Polly: Dog Food, Bait), Odds & Ends (Mr. Tally: buys almost any non-key item), Lost & Found (Mr. Pocket: Old Sketch), Arcade (Pixel: "Stop the Smudge" mini-game), Alchemy (Madame Fizz: fish + seashell → Health Potion).
  - **Level 2 door** says "Coming soon" (a fourth-wall joke: the developers are still drawing it).
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

## 6. Next level: Level 2 (being planned, nothing built)

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
- **Levels:** `level` is 1 = Level 0 Part 1, 2 = Level 0 Part 2 / hub, 3 = Level 1. State objects: `l2` (festival + hub, `l2.hub`, `l2.hubStep` 0–3) and `l3` (coast).
- **Hub module** (search "HUB — coming home"): `returnHome()`, `hubInteract()`, Mrs. Maple, Quill/sketchbook, shops, arcade mini-game, cheats.
- **Shops module** (search "shop interiors"): `SHOPS`, `enterShop`, `shopInteract`, `drawShop`.
- **Fish/bait/store/saving module** (search "FISH TYPES, BAIT"): `FISH`, `rollFish`, `SELL`, `tally()`, `saveGame`, `applySave`, title menu, download/upload.
- **Checkpoints:** `checkpoint` (x), `checkpointY`, `checkpointScene`; R returns there.
- **Overlays that freeze the game:** `lvlUp`, `mini` (arcade), `book` (sketchbook), `titleMenu`, inventory.
- **Test hooks:** `window.__game` (getters for state plus helpers like `tele(x, scene)`, `teleY(x, y)`, `returnHome`, `saveGame`). Cheat panel must be opened in tests: `document.querySelector('details.cheats').open=true`.

---

## 8. Status

- Everything in sections 4–5 is built and tested, and saved in Sarah's local Game folder.
- **Not yet pushed to GitHub** since PR #37. Push only when Sarah says so.
