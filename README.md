# Sarah and the Fading World — Level 1

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
- **Q**: Dab's power — sniff out hidden doodles (they burst into coins)
- **I**: open or close Sarah's Pockets (inventory)
- **R**: return to the Save Block

A pink **!** appears over Sarah whenever there's something to activate. The on-screen Activate button works like Space (and becomes **Continue** during dialogue). You can also click the screen to advance dialogue.

## Sarah's Pockets

The inventory has four pockets: **Items**, **Keys**, **Buddy** (Dab) and **Hints** (current goal plus a checklist of what you've done). Use the arrow keys to pick a slot, **Tab / Q / E** to switch pockets, and **Space** to use an item (the Health Potion restores your health). Mouse clicks work too.

## Level 1 path

Sarah starts in her bedroom (the bed is bouncy). Open the wardrobe, then walk into the Health Potion and Road Chest Key to pick them up. Open the front door with Space, then press Space again to go outside. On her first exit Sarah notices a gate that appeared overnight — locked, with the art festival on the other side.

Along the road: a mailbox with a letter from the Festival Committee, a sign, and a flower that tells her the fountain is spraying the wrong way. Use the Road Chest Key on the chest to release a **Turnip**. Jump into the fountain's upward stream to ride it up and grab **Grandma's Chest Key**. The Save Block restores health (and has opinions). Another flower gives Sarah three coins. Climb the art crates onto Mrs. Maple's roof for the **Festival Pin**.

Past Mrs. Maple's house, lightning rips the sky. The far end of the road loses its color, a flower turns gray and starts crying, and ink **Smudges** appear — stomp them, or lose 1 health if they touch you. Grab the ladder leaning against the tree and bring it to Mrs. Maple, who sets it against her shelf. Climb up and use Grandma's Chest Key to free **Dab**, Sarah's paintbrush little buddy.

Bring Dab to the gray flower to restore its color (and the whole road's). It gives Sarah the **Town Gate Key**. Return to the gate at the far left and unlock it to see: "Thanks for playing Level 1! Level 2 will be created soon!"

`movement_test.html` is the earlier movement-only prototype and can be kept in the repository as a separate reference.
