# Sarah and the Fading World

A small, self-contained 2D browser game prototype. It uses one HTML file, simple canvas drawings, and no external libraries or downloaded art assets.

## Play

Open `index.html` in a desktop browser, or upload it to a GitHub repository and enable GitHub Pages.

## Look and feel

Level 1 is styled as a paper-craft adventure: characters are flat cut-outs with white paper borders that flip paper-thin when they turn around, the world is built from blocky cardstock hills and patterned ground blocks, and everyone talks in comic speech bubbles. Everything is still drawn in code on a canvas, with no downloaded art.

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

## Level 1 path

Sarah starts in her bedroom (the bed is bouncy). Open the wardrobe, then walk into the Health Potion and Road Chest Key to pick them up. Open the front door with Space, then press Space again to go outside. On her first exit Sarah notices a gate that appeared overnight — locked, with the art festival on the other side.

Along the road: a mailbox with a letter from the Festival Committee and a flower that tells her the fountain is spraying the wrong way. Use the Road Chest Key on the chest to release a **Turnip**. Jump into the fountain's upward stream to ride it up and grab **Grandma's Chest Key**. The Save Block saves your progress and restores health. Another flower gives Sarah three coins. Climb the art crates onto Mrs. Maple's roof for the **Festival Pin**.

Past Mrs. Maple's house, lightning rips the sky. One flower at the far end of the road turns gray and starts crying, and ink **Smudges** appear — stomp them for a coin, or lose 1 health if they touch you. Grab the ladder leaning against the tree and bring it to Mrs. Maple, who sets it against her shelf. Climb up and use Grandma's Chest Key to free **Dab**, Sarah's paintbrush little buddy.

Bring Dab to the gray flower to restore its color. It gives Sarah the **Town Gate Key**. Return to the gate at the far left and unlock it to finish Level 1, then press Space to continue to Level 2.

## Level 2 — The Festival Fiasco

**The orchard.** Level 2 starts in the town orchard: a sign that says "The Orchard" and four apple trees (apples out of reach for now). A path in the orchard leads to the lake, where a lakeside tree has 5 coins in its branches, so you can earn the entry fee before registering. Walk left out of the orchard to go back to the (cleared) Level 1 road. If you skipped the Festival Pin on Mrs. Maple's roof, it's still there. At the end is the **Registration table**. Entry costs 5 coins, or it's free if you're *wearing* your Festival Pin (Pockets → Key Items → Festival Pin → Wear). The Registrar notices whether you're wearing it. You can also **Try bargaining**: guess her favorite color. Cyan gets you in free (she's a CMYK girl, even on a screen). Any other color earns the same joke, and you still pay. Bargaining works once. If you walk in wearing the pin, she still gives you the color quiz for fun and makes the CMYK joke. Then she tells Sarah about the art contest. The same Registrar takes your contest entry later.

**The main story:**
1. **Arrive.** Townsfolk recognize Dab from the old stories and wonder whether Sarah is the legendary adventurer. Mr. Umber teaches the hiding trick (hold Down/S by a crate).
2. **Contest (optional).** Make a Ball of Clay or a Lopsided Teapot at the Clay Corner (or make nothing) and bring it to the Registrar. Entering wins 20 coins "for trying."
3. **Free Mr. Biscuits.** His head is stuck in the jungle gym. Sneak a curl from Brie's butter swan (2 Butter Pats) and grease him free.
4. **The chase.** Brie chases you. Jump crates, duck behind them, and choose "Sorry." when caught (refuse twice and you get a buttery slap).
5. **Find Nib.** Dab's Q by the art-supply stand reveals a doodle staircase up to Nib the pencil (Q jabs).
6. **Prickles.** A tall, spiky creature blocks the stage. You can't jump over him or on him, and touching him hurts. The waiting crowd points you to something sparkling by the Weather Station (Nib). The crowd (and Mr. Biscuits, once freed) waits on this side of him. Prickles has a health bar and takes two Nib jabs. Then everyone walks to the stage, the cat hops onto the judge's seat, and the results begin; the cloth falls away before the painting is revealed.
7. **Results.** Juniper's painting looks a lot like Sarah and Dab. The prophecy!
8. **Finale.** (A Save Block on the second floor sits right before the sky door.) The sky cracks. Smudges drain the painting, and a door falls onto the **second floor** balcony above the stage. One Smudge drops the Smudgy Key. Mrs. Maple hurries over towing the **balloon dog** sculpture on a string, says Sarah must save the town, then moves the string over to Sarah's backpack so she can float up to the jump bars on the right of the stage. Fall off and Mrs. Maple puts down a trampoline. Climb to the second floor and unlock the door: "Level 3 coming soon!"

**Around town (optional):**
- **The lake** (door in the orchard): chicken coop, a sign ("Eggs: friends of the dog only") and Waffles the dog, who won't let you in but would love dog food. A **Fishing Area** sign stands on the dock, but nobody has a pole to spare yet — Sarah finds Reel in Level 3. (With Reel, press Space at the end of the dock to cast; when the bobber is yanked under you have 2 seconds to press Space.) Falling off the dock costs 1 health and puts Sarah back on the dock.
- **The hole** near the entrance. Its sign is faded gray until Dab (Q) restores it: "Dig crew entry here." Jump over the hole, or fall in to reach **Undertown**, a full underground floor with a bar (pick up the **Town Map**), the Grimy Grotto club (a bouncer won't let you in), a closed Potter's Studio, Lost & Found, Arcade, a crooked-roofed Alchemy shop with a bubbling cauldron, a sewer tunnel, and a dinosaur skeleton stuck in the dirt (dig skills coming someday). A trampoline bounces you back up.
- **Chef Crumb** cooks from recipe cards: a glowing card near the Clay Corner (Turnip + Butter Pat → Health Potion) and the Cheese recipe (2 Butter Pats → Cheese Wedge, +3 health).
- **Balloons and the sky:** Inka sells balloons for 5 coins (next jump twice as high). The Library roof chest has a Turnip, the Cheese recipe and 15 coins. From the roof, four coin clouds lead to a one-time fairy (+5 max health and a full heal). After she leaves, a Smudge guards the top cloud.
- **Gus** is fixing the elevator to the second floor (a future hook). Shops are "Closed for Festival" with joke signs, including a Pet Store (dog food, someday), the Hatter's and a Toy Shop. Next to the butter swan are a balloon dog and a melting ice duck.

**Little buddies:** Dab (Q finds hidden doodles), Nib (Q jabs) and Reel (fishing). Swap with E or in the Buddy pocket.

**Pockets:** Items (things you use up), **Key Items** (important things you can't get rid of: keys, the Town Map, recipe cards, the Festival Pin), Buddy, **Journal** and Hints.

## Level 3 — The Watercolor Coast

Finishing Level 2 (through the door from the sky) continues into Level 3. The chapter is split into sub-chapters, each with a title card.

**3-1: The Watercolor Coast.** Sarah lands face-first on a beach that's still wet paint, with the colors running into the sea.
- **Marina**, a hermit crab who runs (and is) the Shell Shack, says the sand and sea are full of treasure. She trades **3 Seashells for her Shell Shield**: use it from Pockets and a bubble blocks the next **2 hits**, then breaks away.
- With Dab equipped, **Q** reveals buried treasure as pink X marks; stand on one and press Space to dig. You'll find Seashells, coins, and a **Heart Necklace** with a big red heart-shaped gem: the **Red gem**.
- Past the digging beach are the **Tide Flats**. The tide goes out for about 6 seconds, then rolls in and stays in for a few seconds. Run across while it's out, or wait it out on one of the two tall rocks. Get caught on the flats when the water's up and the tide sweeps you back to the last safe spot (-1 health). There are four rocks along the way, and treasure to dig on the flats, too.
- After the flats, the old dock out to the shipwreck has faded away. Use Dab (Q) to paint it back, then run along it (watch the gulls overhead) and hop across the rocks to the **shipwreck**. The treasure chest on its deck turns out to be **Reel**, the fishing-pole buddy. He explains the lighthouse lamp is failing and needs three gems: **Red, Green and Blue**.
- Fish from the back of the shipwreck (Reel can also fish off the hidden dock, the rock two to the left of the boat, and the rock just to its right). You'll catch between 1 and 5 Sea Perch, then hook the **Blue Gem**. Falling in the sea costs 1 health.
- With Red and Blue in hand, hop across a longer run of rocks (six of them, at different heights) past the boat to the sand where the lighthouse stands.

**3-2: The Gray Lighthouse.** Every few seconds an ink drip falls from somewhere above (it hurts if it hits Sarah, and about 1 in 10 turns into a Smudge where it lands). A tall vertical climb (extra-long, with a new stretch above the big landing) with static and **moving platforms** (blue, with ◀ ▶ or ▲▼ arrows) The only Save Block in Level 3 sits on the last platform before the boss deck; otherwise your checkpoint is the start of the beach, then the lighthouse entrance.
- The **Green Gem** is hidden in a painted-over gray nook high on the left, above the big landing. Getting there: ride a lift up, step onto a cracked ledge that crumbles a second after you land on it, then jump onto a moving bar that's packed with Smudges. You have to land on top of them to make room. Once you're in the nook, use Dab (Q) to reveal the gem. The Smudges on the bar come back if you return to the landing.
- At the top: a **Health Potion**, then the boss, **The Blot**, a giant ink squid. Jab its tentacles with Nib when they slam down (a slam that lands on Sarah costs 2 health), dodge falling ink drops (watch their shadows; about 1 in 10 turns into a **Smudge** on the deck) and stomp its head when it rises over the railing (1 damage per stomp). It has a health bar.
- Set the three gems in the lamp to light the lighthouse and bring the coast's colors back. If the Green Gem is missing, drop down the gap on the left of the deck to go find it.

**New creatures:** Sidecrabs (stomp only when their claws are down), Gulls (swoop to steal a coin; hit them while they're low to get it back), Hermit Smudges (too hard to stomp until Nib flips them over; then stomp or jab again).

## XP and leveling up

Defeating creatures earns **XP**. A Smudge, Prickles and a Sidecrab are worth 1 XP each, a Gull or a Hermit Smudge 2 XP, and The Blot 10 XP. The XP bar sits under the health counter. Level 2 needs 15 XP, and each level after that needs 10 more than the last (25, 35, 45…). On a level up the game freezes, confetti falls, and an announcement shows the new level: **+5 max health and health refilled**. Press Space to keep going.

The **Journal** tab in Pockets shows Sarah's level and XP, plus a page for each creature: how many you've defeated, how much XP each is worth, where it lives and how to beat it. Creatures you haven't beaten yet show as gray silhouettes.

## Admin Cheats Only

The cheat panel under the game is collapsed by default; click **Admin Cheats Only** to open it.

Below the game there's a red **Admin Cheats Only** box for testing. **Start Level 2** begins in the orchard with the Turnip, Festival Pin and Dab. **L2: festival (registered)** skips straight into town. Other buttons jump to after the chase, the contest results, or the Smudge fight, Level 3 buttons jump to the beach, the tide flats, the hidden dock, the shipwreck chest, the fishing spot, the bottom of the lighthouse, the big landing (for the Green Gem detour), the top of the lighthouse and the boss fight, plus **Give all 3 gems** and **Give Shell Shield**. **+20 coins** tops up your wallet, **Level up now** triggers a level up, and **Fill & open Journal** fills in every Journal page. **Restart Level 1** reloads the page.

`movement_test.html` is the earlier movement-only prototype and can be kept in the repository as a separate reference.
