# Sarah and the Fading World

A small, self-contained 2D browser game prototype. It uses one HTML file, simple canvas drawings, and no external libraries or downloaded art assets.

## Play

Open `index.html` in a desktop browser, or upload it to a GitHub repository and enable GitHub Pages.

## Look and feel

The game is styled as a paper-craft adventure: characters are flat cut-outs with white paper borders that flip paper-thin when they turn around, the world is built from blocky cardstock hills and patterned ground blocks, and everyone talks in comic speech bubbles. Everything is still drawn in code on a canvas, with no downloaded art.

## Controls

- **A/D** or **Left/Right arrows**: move
- **W** or **Up arrow**: jump, or climb up Mrs. Maple's ladder
- **S** or **Down arrow**: climb down the ladder
- **Space**: activate nearby doors, chests, signs and people; advance dialogue
- **Q**: Buddy power — with Dab, sniff out hidden doodles (they burst into coins)
- **I**: open or close Sarah's Pockets (inventory)
- **E**: swap equipped buddy (once you have more than one)
- **R**: return to the last Save Block
- **Arrows / W / S + Space**: pick an answer when a conversation gives you choices

A pink **!** appears over Sarah when she's next to someone she can talk to (people and flowers). The on-screen Activate button works like Space (and becomes **Continue** during dialogue). You can also click the screen to advance dialogue.

## Sarah's Pockets

The inventory has four pockets: **Items**, **Keys**, **Buddy** (Dab) and **Hints** (current goal plus a checklist of what you've done). Use the arrow keys to pick a slot, **Tab / Q / E** to switch pockets, and **Space** to use an item (the Health Potion restores your health). Mouse clicks work too.

## Structure: hub and spokes

The town is **Level 0**, the hub you keep coming back to. It has two parts: **Part 1** (Sarah's home and the road) and **Part 2** (the festival). High above the festival is a long **second floor** with room for six doors. Each door leads to a standalone level (a "spoke"). **Level 1** is the Watercolor Coast. Later, returning to the hub after a level, and Gus's fixed elevator up to the second floor, will be added.

## Level 0 — Part 1: Home and the road

Sarah starts in her bedroom (the bed is bouncy). Open the wardrobe, then walk into the Health Potion and Road Chest Key to pick them up. Open the front door with Space, then press Space again to go outside. On her first exit Sarah notices a gate that appeared overnight — locked, with the art festival on the other side.

Along the road: a mailbox with a letter from the Festival Committee and a flower that tells her the fountain is spraying the wrong way. Use the Road Chest Key on the chest to release a **Turnip**. Jump into the fountain's upward stream to ride it up and grab **Grandma's Chest Key**. The Save Block saves your progress and restores health. Another flower gives Sarah three coins. Climb the art crates onto Mrs. Maple's roof for the **Festival Pin**.

Past Mrs. Maple's house, lightning rips the sky. One flower at the far end of the road turns gray and starts crying, and ink **Smudges** appear — stomp them for a coin, or lose 1 health if they touch you. Grab the ladder leaning against the tree and bring it to Mrs. Maple, who sets it against her shelf. Climb up and use Grandma's Chest Key to free **Dab**, Sarah's paintbrush little buddy.

Bring Dab to the gray flower to restore its color. It gives Sarah the **Town Gate Key**. Return to the gate at the far left and unlock it to finish Part 1, then press Space to continue to Part 2.

## Level 0 — Part 2: The Festival Fiasco

**The orchard.** Part 2 starts in the town orchard: a sign that says "The Orchard" and four apple trees (apples out of reach for now). A path in the orchard leads to the lake, where a lakeside tree has 5 coins in its branches, so you can earn the entry fee before registering. Walk left out of the orchard to go back to the (cleared) Level 1 road. If you skipped the Festival Pin on Mrs. Maple's roof, it's still there. At the end is the **Registration table**. Entry costs 5 coins, or it's free if you're *wearing* your Festival Pin (Pockets → Key Items → Festival Pin → Wear). The Registrar notices whether you're wearing it. You can also **Try bargaining**: guess her favorite color. Cyan gets you in free (she's a CMYK girl, even on a screen). Any other color earns the same joke, and you still pay. Bargaining works once. If you walk in wearing the pin, she still gives you the color quiz for fun and makes the CMYK joke. Then she tells Sarah about the art contest. The same Registrar takes your contest entry later.

**The main story:**
1. **Arrive.** Townsfolk recognize Dab from the old stories and wonder whether Sarah is the legendary adventurer. Mr. Umber teaches the hiding trick (hold Down/S by a crate).
2. **Contest (optional).** Make a Ball of Clay or a Lopsided Teapot at the Clay Corner (or make nothing) and bring it to the Registrar. Entering wins 20 coins "for trying."
3. **Free Mr. Biscuits.** His head is stuck in the jungle gym. Sneak a curl from Brie's butter swan (2 Butter Pats) and grease him free.
4. **The chase.** Brie chases you. Jump crates, duck behind them, and choose "Sorry." when caught (refuse twice and you get a buttery slap).
5. **Find Nib.** Dab's Q by the art-supply stand reveals a doodle staircase up to Nib the pencil (Q jabs).
6. **Prickles.** A tall, spiky creature blocks the stage. You can't jump over him or on him, and touching him hurts. The waiting crowd points you to something sparkling by the Weather Station (Nib). The crowd (and Mr. Biscuits, once freed) waits on this side of him. Prickles has a health bar and takes two Nib jabs. Then everyone walks to the stage, the cat hops onto the judge's seat, and the results begin; the cloth falls away before the painting is revealed.
7. **Results.** Juniper's painting looks a lot like Sarah and Dab. The prophecy!
8. **Finale.** The sky cracks. Smudges drain the painting, and a door falls way up onto the festival's **second floor**: a long sky walkway running from the top of Gus's elevator shaft to above the stage, with room for six level doors (the Level 1 door is the first, at the right end; the elevator will arrive at the left end once Gus fixes it). One Smudge drops the Smudgy Key (if you miss it, Mrs. Maple hands it over). Mrs. Maple hurries over towing the **balloon dog** on a string and ties it to Sarah's backpack. One hop and the dog floats Sarah all the way up to the second floor, then slips loose. A Save Block sits right before the door. Unlock the door to continue.

**Around town (optional):**
- **The lake** (door in the orchard): chicken coop, a sign ("Eggs: friends of the dog only") and Waffles the dog, who won't let you in but would love dog food. A **Fishing Area** sign stands on the dock, but nobody has a pole to spare yet — Sarah finds Reel in Level 1. (With Reel, press Space at the end of the dock to cast; when the bobber is yanked under you have 2 seconds to press Space.) Falling off the dock costs 1 health and puts Sarah back on the dock.
- **The hole** near the entrance. Its sign is faded gray until Dab (Q) restores it: "Dig crew entry here." Jump over the hole, or fall in to reach **Undertown**, a full underground floor with a bar (pick up the **Town Map**), the Grimy Grotto club (a bouncer won't let you in), a closed Potter's Studio, Lost & Found, Arcade, a crooked-roofed Alchemy shop with a bubbling cauldron, a sewer tunnel, and a dinosaur skeleton stuck in the dirt (dig skills coming someday). A trampoline bounces you back up.
- **Chef Crumb** cooks from recipe cards: a glowing card near the Clay Corner (Turnip + Butter Pat → Health Potion) and the Cheese recipe (2 Butter Pats → Cheese Wedge, +3 health).
- **Balloons and the sky:** Inka sells balloons for 5 coins (next jump twice as high). The Library roof chest has a Turnip, the Cheese recipe and 15 coins. From the roof, four coin clouds lead to a one-time fairy (+5 max health and a full heal). After she leaves, a Smudge guards the top cloud.
- **Gus** is fixing the elevator to the second floor (a future hook). Shops are "Closed for Festival" with joke signs, including a Pet Store (dog food, someday), the Hatter's and a Toy Shop. Next to the butter swan are a balloon dog and a melting ice duck.

**Little buddies:** Dab (Q finds hidden doodles), Nib (Q jabs) and Reel (fishing). Swap with E or in the Buddy pocket.

**Pockets:** Items (things you use up), **Key Items** (important things you can't get rid of: keys, the Town Map, recipe cards, the Festival Pin), Buddy, **Journal** and Hints.

## Level 1 — The Watercolor Coast

Unlocking the first door on the festival's second floor leads into Level 1. It's split into sub-levels, each with a title card.

**1-1: The Watercolor Coast.** Sarah lands face-first on a beach that's still wet paint, with the colors running into the sea.
- **Marina**, a hermit crab who runs (and is) the Shell Shack, says the sand and sea are full of treasure. She trades **3 Seashells for her Shell Shield**: use it from Pockets and a bubble blocks the next **2 hits**, then breaks away.
- With Dab equipped, **Q** reveals buried treasure as pink X marks; stand on one and press Space to dig. You'll find Seashells, coins, and a **Heart Necklace** with a big red heart-shaped gem: the **Red gem**.
- Past the digging beach are the **Tide Flats**. The tide goes out for about 6 seconds, then rolls in and stays in for a few seconds. Run across while it's out, or wait it out on one of the two tall rocks. Get caught on the flats when the water's up and the tide sweeps you back to the last safe spot (-1 health). There are four rocks along the way, and treasure to dig on the flats, too.
- After the flats, the old dock out to the shipwreck has faded away. Use Dab (Q) to paint it back, then run along it (watch the gulls overhead) and hop across the rocks to the **shipwreck**. The treasure chest on its deck turns out to be **Reel**, the fishing-pole buddy. He explains the lighthouse lamp is failing and needs three gems: **Red, Green and Blue**.
- Fish from the back of the shipwreck (Reel can also fish off the hidden dock, the rock two to the left of the boat, and the rock just to its right). You'll catch between 1 and 5 Sea Perch, then hook the **Blue Gem**. Falling in the sea costs 1 health.
- With Red and Blue in hand, hop across a longer run of rocks (six of them, at different heights) past the boat to the sand where the lighthouse stands.

**1-2: The Gray Lighthouse.** Every few seconds an ink drip falls from somewhere above (it hurts if it hits Sarah, and about 1 in 10 turns into a Smudge where it lands). A tall vertical climb (extra-long, with a new stretch above the big landing) with static and **moving platforms**, plus **cracked shelves** that shake and crumble about a second after you land on them (they grow back after 3 seconds). Several are on the main path, including a run of three right before the top, and the Save Block before the boss sits on the solid shelf just after them. (blue, with ◀ ▶ or ▲▼ arrows) The only Save Block in Level 1 sits on the last platform before the boss deck; otherwise your checkpoint is the start of the beach, then the lighthouse entrance.
- The **Green Gem** is hidden in a painted-over gray nook high on the left, above the big landing. Getting there: ride a lift up, step onto a cracked ledge that crumbles a second after you land on it, then jump onto a moving bar that's packed with Smudges. You have to land on top of them to make room. Once you're in the nook, use Dab (Q) to reveal the gem. The Smudges on the bar come back if you return to the landing.
- At the top: a **Health Potion**, then the boss, **The Blot**, a giant ink squid. Jab its tentacles with Nib when they slam down (a slam that lands on Sarah costs 2 health), dodge falling ink drops (watch their shadows; about 1 in 10 turns into a **Smudge** on the deck) and stomp its head when it rises over the railing (1 damage per stomp). It has a health bar.
- Set the three gems in the lamp to light the lighthouse and bring the coast's colors back. If the Green Gem is missing, drop down the gap on the left of the deck to go find it.

**New creatures:** Sidecrabs (stomp only when their claws are down), Gulls (swoop to steal a coin; hit them while they're low to get it back), Hermit Smudges (too hard to stomp until Nib flips them over; then stomp or jab again).

## Back in town after Level 1 (the hub)

When the lamp is lit, its beam swings up to point at the sky, right where Sarah fell in. Dab explains that when a page is whole again, its light shines back through the door it came from, like a bookmark showing the way home. Sarah steps into the beam, the "Level 1 complete!" screen appears, and **Press Space to head home to town** carries her up through the inky dark and out through the page door onto the festival's second floor. A "Level 0 — Back in Town" title card appears.

**Replaying Level 1.** The Level 1 door on the second floor (marked ✓ LEVEL 1) can be entered again. The replay starts on the beach with the coast already in full color: Reel is with you, the three gems are already in the lamp and The Blot is gone. Creatures, treasure, the tide flats, the hidden dock and the lighthouse climb are all there to play. At the top of the lighthouse, step into the beam to ride home.

**The story so far.** The world is one enormous sketchbook, and every place is a page. Long ago Sarah's Grandma, a young painter named Monty and Dab kept every page colorful. After Mr. Biscuits gave Monty's festival painting a terrible review, Monty went gray, became **Professor Monochrome**, and started ripping pages out of the world. Every torn-out page becomes a door. Grandma went after him years ago and never came home. Every page Sarah stitches back in brings her closer to finding Grandma.

The Professor is glimpsed three times before the reveal: a gray figure on a far hill during the first storm (Part 1), a gray-gloved hand poking out of the tear above the stage (Part 2), and a figure in a gray top hat rowing away with the tiny squid after The Blot (Level 1).

**Coming home, step by step:**
1. The beam drops Sarah out of the page door, and **Gus's newly fixed elevator** carries her straight down to the ground floor. Gus explains that the festival is over and some shops have opened up again. Dab recognizes the man in the rowboat. (Ride the elevator back up to the second floor any time.)
2. **Mrs. Maple**, at the far right end of town, tells the story of Grandma, Monty and the sketchbook world.
3. **Quill**, outside the library, shows **The Great Sketchbook**: the Watercolor Coast page is back, five pages are still torn out. Then a second door thuds onto the second floor.
4. The town opens up to explore.

**Doors on the second floor.** The Level 1 door can be replayed (see above). The new Level 2 door says "Coming soon": the page is still being drawn by the game's developers.

**Things to do in town now:** The festival is over: the registration table, sculptures, contest stage, bunting and booths are packed away (except Chef Crumb's kitchen and the Art Supplies booth, which stay open). Mr. Biscuits the cat now suns himself outside the pet store. Shops that are closed have an **ON VACATION** sign.

Open shops have an **OPEN!** sign. Press Space at the door to **go inside**, walk up to the counter and talk to the shopkeeper behind it. Press Space at the EXIT door to leave.
- **Paws & Claws pet store:** Polly sells Dog Food for 4 coins (bring it to **Waffles** at the lake and he trades you 3 **Fresh Eggs**) and **Bait ×3 for 5 coins**.
- **Odds & Ends general store** (the old Toy Shop, near the festival entrance): Mr. Tally buys almost anything in your Pockets except key items. Pick an item to sell one (use **More items** to page through), or **Sell all fish**. Prices: Lake/Sea Perch 3, Sunfish 6, Sea Bass 6, Pufferfish 8, Catfish 15, Swordfish 20, Golden Koi 40, Seashell 4, Turnip 5, Fresh Eggs 2, Health Potion 6, Shell Shield 8, Lopsided Teapot 6, Cheese Wedge 4, Ball of Clay 3, Dog Food 2, Balloon 2, Butter Pat 2, Bait 1.
- **Chef Crumb's Kitchen** still cooks from recipe cards, and **Inka's Art Supplies** still sells balloons.
- **Fishing** at the lake works now that Sarah has Reel. If you have Bait, each cast uses one: fish bite faster and rare fish show up much more often.
- **Undertown shops** are open (go inside each one):
  - **Lost & Found:** Mr. Pocket hands over the **Old Sketch** ("The Three of Us": Grandma, Monty and Dab).
  - **Underground Arcade:** Pixel's **Stop the Smudge** mini-game (1 coin to play; press Space when the Smudge is in the box; 2 coins per bullseye over 3 rounds).
  - **Alchemy Shop:** Madame Fizz brews a **Health Potion** from any fish plus 1 seashell (or 3 coins instead of the shell).
- Still closed for later: the Grimy Grotto, the orchard apples and the mysterious gate.

## Fish

| Lake (town) | How rare | Sea (Watercolor Coast) | How rare |
|---|---|---|---|
| Lake Perch | common | Sea Perch | common |
| Sunfish | uncommon | Sea Bass | uncommon |
| Catfish | rare | Pufferfish | uncommon |
| Golden Koi | very rare | Swordfish | rare |

On the coast, the Blue Gem still turns up within your first 1–5 catches.

## Saving

The game **saves in your browser only when you use a Save Block**. When you open the game again you get **Continue** or **New Game**. Continue puts you back at your last Save Block with everything you had at that moment: pockets, coins, buddies, XP and level progress. Anything you did after that save (fish caught, things bought or sold) isn't kept unless you save again. New Game wipes the browser save.

A browser save only lives in that one browser on that one computer, and clearing browsing data erases it. For a backup, use the buttons under the game:
- **Download save** downloads your last Save Block save as `sarah-fading-world-save.json`.
- **Load save file** loads one of those files back in (on any computer or browser).

## XP and leveling up

Defeating creatures earns **XP**. A Smudge, Prickles and a Sidecrab are worth 1 XP each, a Gull or a Hermit Smudge 2 XP, and The Blot 10 XP. The XP bar sits under the health counter. Reaching Lv 2 takes 15 XP, and each Lv after that needs 10 more than the last (25, 35, 45…). On a level up the game freezes, confetti falls, and an announcement shows the new level: **+5 max health and health refilled**. Press Space to keep going.

The **Journal** tab in Pockets shows Sarah's level and XP, plus a page for each creature: how many you've defeated, how much XP each is worth, where it lives and how to beat it. Creatures you haven't beaten yet show as gray silhouettes.

## Admin Cheats Only

The cheat panel under the game is collapsed by default; click **Admin Cheats Only** to open it.

Below the game there's a red **Admin Cheats Only** box for testing. **Start Level 0 — Part 2** begins in the orchard with the Turnip, Festival Pin and Dab. **L0-2: festival (registered)** skips straight into town. Other buttons jump to after the chase, the contest results, or the Smudge fight, **Hub: back in town after Level 1** jumps straight to coming home, and **Replay Level 1 (from the hub)** starts a replay, **Hub: general store (fish + bait)** drops you inside Odds & Ends at Mr. Tally's counter with fish, bait and shells to sell, **Clear saved game** deletes the browser save, and **Restart from the beginning** starts a new game in Sarah's bedroom after you confirm (the browser save is kept until you use a Save Block). Level 1 buttons (**Start Level 1**, then **L1: …**) jump to the beach, the tide flats, the hidden dock, the shipwreck chest, the fishing spot, the bottom of the lighthouse, the big landing (for the Green Gem detour), the top of the lighthouse and the boss fight, plus **Give all 3 gems** and **Give Shell Shield**. **+20 coins** tops up your wallet, **Level up now** triggers a level up, and **Fill & open Journal** fills in every Journal page. **Restart Level 1** reloads the page.

`movement_test.html` is the earlier movement-only prototype and can be kept in the repository as a separate reference.
