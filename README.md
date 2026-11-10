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

Sarah steps through the gate into the Town Art Festival. Townsfolk recognize Dab from the old stories and start wondering whether Sarah is the legendary adventurer. Sarah would just like a lemonade.

1. **Register (optional).** Sarah left her banner at home, so the Registrar sends her to the Clay Corner. She can make a Ball of Clay or a Lopsided Teapot, or stare at the clay until it gets awkward and make nothing. Enter it and she wins 20 coins "for trying" after the results.
2. **Recipe Card.** A glowing card sits on the café table near the start. Chef Crumb can cook it into a Health Potion: Turnip + Butter Pat.
3. **Free Mr. Biscuits.** The judge's head is stuck in the playground jungle gym. Sarah sneaks a curl of butter from Brie's DO NOT TOUCH butter swan (2 Butter Pats, which stack) and greases him free.
4. **The chase.** Brie notices and chases Sarah. Jump the crates, hold **S** next to a crate to duck behind it, and you'll still get caught. Choose "Sorry." Refuse twice and you get a buttery slap (-1 health).
5. **Find Nib.** Lou saw something shiny in the sky. With Dab equipped, press **Q** by the art-supply stand to reveal a doodle staircase up to **Nib**, a living pencil. Q with Nib equipped jabs enemies. Swap buddies with **E** or the Buddy pocket.
6. **Contest results.** Juniper wins with a painting of the legendary adventurer, who looks a lot like Sarah, plus Dab. The town connects the dots. Sarah isn't so sure.
7. **The sky cracks again.** Smudges drain color from the painting, and a door falls out of the sky. Jab or stomp the Smudges. One of them drops the **Smudgy Key**. Mrs. Maple arrives to tell Sarah she must save the town. Unlock the sky door to finish Level 2 ("Level 3 coming soon!").

The town is set up as a future hub. It has Chef Crumb's healing recipes, Gus and his clogged pipe (a hook for later), shops "Closed for Festival" with joke signs, two Save Blocks, and hidden doodles for Dab to find.

## Admin Cheats Only

Below the game there's a red **Admin Cheats Only** box for testing. **Start Level 2** drops you at the festival with the Turnip, Festival Pin and Dab. Other buttons jump to after the chase, the contest results, or the Smudge fight. **Restart Level 1** reloads the page.

`movement_test.html` is the earlier movement-only prototype and can be kept in the repository as a separate reference.
