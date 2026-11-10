# Sarah and the Fading World — Level 1

A small, self-contained 2D browser game prototype. It uses one HTML file, simple canvas drawings, and no external libraries or downloaded art assets.

## Play

Open `index.html` in a desktop browser, or upload it to a GitHub repository and enable GitHub Pages.

## Controls

- **A/D** or **Left/Right arrows**: move
- **W** or **Up arrow**: jump or climb up Mrs. Maple's ladder
- **S** or **Down arrow**: climb down Mrs. Maple's ladder
- **Space**: activate nearby doors, chests, and people; advance dialogue
- **Q**: use little buddy power to reveal nearby hidden things
- **I**: open or close inventory; current objective appears under **Hints**
- **R**: return to the last Save Block

Health is shown as a number out of 10.

The on-screen **Activate** button works like Space. Dialogue advances with Space or the Continue button; arrow keys do not advance it.

## Level 1 path

Sarah starts in her bedroom with a jumpable bed and is on her way to the town art festival. Open the wardrobe, then walk into the Health Potion and Road Chest Key to collect each; each disappears when touched. Open her front door with Space, then press Space again to go outside. The town gate has appeared overnight; the gate dialogue plays only on Sarah's first exit. Explore the road. The first flower points her toward the fountain's upward stream, and another flower gives her three coins.

Use the Road Chest Key from the wardrobe to unlock the first chest and collect its **Turnip** from the ground. Jump into the fountain's upward-moving water to get **Grandma's Chest Key**. At Mrs. Maple's house, use the nearby stack of art crates to jump onto the roof and collect the Festival Pin. A lightning quake reveals the crying gray flower. Continue past it to find a ladder leaning against a tree, then return to Mrs. Maple. The ladder stays in inventory while she talks and sets it up; after the exchange it is removed from inventory and becomes climbable. Climb up or down to grandma's chest. Use Grandma's Chest Key to meet Dab, Sarah's paintbrush little buddy. Keys and Dab have separate sections in the inventory, which scrolls when its contents need more room. Talk to Mrs. Maple again after giving her the ladder to hear her ask whether you climbed it.

Use Dab on the gray flower to restore its color. It thanks Sarah and gives her the **Town Gate Key**. Return to the gate at the left and unlock it to see: “Thanks for playing Level 1! Level 2 will be created soon!”

`movement_test.html` is the earlier movement-only prototype and can be kept in the repository as a separate reference.
