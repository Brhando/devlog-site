# WhileIterating RPG Devlog

## Day 1: Environment Setup and Basic Design – 18 May, 2025

- Installed Godot 4.4.1 Mono
- Set up .NET 8 SDK
- Verified C# script runs inside Godot
- Configured Git, added .gitignore, made first commit
- Created base folders: /Scenes, /Scripts, /Assets, /UI
- Finalized core loop, races, classes, stat system, and world design
- Gained deeper understanding of Godot scenes, physics process, and script structure
- Ready to start player movement and time system tomorrow

## Day 2: Character Movement, Starting Area, and Early Dialogue – May 19, 2025

**Progress Made**
- Designed the **starting area** of the game, including terrain layout, environment objects, and player spawn placement.
- Added assets (sprites, terrain, etc.) to assets folder.
- Successfully implemented a **fully controllable player character**, complete with 4-directional movement and animation using `AnimatedSprite2D`.
- Set up the **Camera2D** to follow the player.
- Built the foundation of the **class selection system** using interactable items (e.g., a Short Sword).
- Implemented a `CanvasLayer`-based **dialogue UI system** using a `Panel` and `Label`.
- Wrote a reusable `DialogUI.cs` script to handle timed messages via `ShowMessage()`.
- Confirmed all internal values (text, visibility, position) were updating as expected.

**Challenges**
- Despite correct setup, the **dialogue UI wouldn't render in-game**.
- Troubleshot potential issues with:
  - Layout anchors and positioning
  - Text visibility and color overrides
  - Missing font assignments
  - Z-layering and rendering order
  - Viewport scaling/stretch modes
- After extensive debugging, decided to **scrap and rebuild** the dialogue UI from scratch to ensure clean behavior.

**Next Steps**
- Rebuild the dialogue UI from a clean scene using minimal structure.
- Confirm the panel anchors properly to the top of the screen and stays fixed regardless of camera movement.
- Add polish: fade-in/out, typewriter animation, or branching text.
- Fully connect **item pickup (sword/tome)** to **class assignment** logic.

**Reflection**
> Even though the dialogue box didn’t work out today, I made solid foundational progress: the player moves, the world is built, and the systems are coming together. Sometimes starting over is faster than untangling a UI issue—and now I know exactly how to rebuild it cleaner. Tomorrow’s gonna be a win.

## 🗡️ Day 3: Combat System, Scene Structure, and Sprite Animation – May 20, 2025

---

**Progress Made**
- Built and tested a fully functional **turn-based combat system**, including turn manager, player/enemy actions, win/loss conditions, and UI flow.
- Refactored the **DungeonUI** structure to avoid unnecessary scripting by handling logic directly in the `BattleScene` script via `GetNode()`.
- Finalized clean and modular **`PlayerEntity.cs`** and **`EnemyEntity.cs`** scripts with health systems, damage functions, and animation triggers.
- Gained a much clearer understanding of how to use **`GetNode<T>()`** to connect scripts with scene elements.
- Improved code organization by adopting consistent **C# naming conventions**: `_camelCase` for private fields and `PascalCase` for public ones.
- Integrated player and enemy **animations** using `AnimatedSprite2D`, including basic attack and hurt states.
- Pushed the full project update (excluding devlog) to Git for version tracking and backup.

---

**Challenges**
- Initially over-engineered the UI logic by trying to write a script for `DungeonUI` before realizing the logic belonged in `BattleScene`.
- Required a mindset shift to better understand **scene composition vs. scripting**—not every node needs behavior.
- Setting up **animations** was time-consuming due to sprite alignment and frame management, even with premade assets.
- Manually managing sprite sheets and ensuring **proper playback** for layered visuals (main + secondary animations) was more tedious than expected.

---

**Next Steps**
- Add polish to combat animations and transitions (e.g., **fade effects**, **idle resets**, or **sound FX**).
- Revisit and implement deferred code improvements (e.g., **clamped health values**, **constants for damage**, **ResetToIdle()**, etc.).
- Begin building the **Home Base scene** as part of the vertical slice, including player spawn, basic environment, and placeholder interactions.
- Lay groundwork for future expansion to **Resource Area**, **Overworld Map**, and **Day/Night system** after core polish.

---

**Reflection**
> Today everything started clicking. I finally understood how to wire up scenes using `GetNode()`, and my confidence with Godot and C# has skyrocketed. I learned not to overthink structure—sometimes simplicity is best. Also: animation is no joke. I’m grateful I bought a sprite pack, because aligning frames by hand is already a lot. Designing my own will be a mountain later, but that’s a future win. For now, I’m proud of what I’ve built. It works—and that feels awesome.

