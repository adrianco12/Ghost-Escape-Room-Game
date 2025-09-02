# 👻 Ghost Escape Room

## Overview
Ghost Escape Room is a **first-person horror puzzle escape room game**.  
You play as an office worker who overslept and finds themselves locked inside the building.  
To escape, you must uncover clues, collect tools, and solve puzzles — all while avoiding a deadly ghost.  

- **Win Condition**: Escape the building without being caught.  
- **Lose Condition**: Get caught by the ghost.  

The game emphasizes exploration, puzzle-solving, and survival under pressure.

---

## Features
- First-person horror escape room setting.
- Interactive objects (computers, images, tools, and machines).
- Ghost AI with patrol, chase, and attack states.
- Inventory system with clues, keys, and tools.
- Puzzle-based progression to unlock areas and escape.
- Narration strings for immersive clue interaction.
- Instructions included for players to get started.

---

## Core Gameplay Mechanics
1. **Exploration** – Navigate the office building, search for objects, and analyze clues.  
2. **Inventory & Tools** – Collected objects are stored and can be used to solve puzzles.  
3. **Ghost AI** –  
   - **Patrolling**: Moves between waypoints.  
   - **Chasing**: Pursues the player when spotted.  
   - **Attacking**: Ends the game on contact.  
4. **Winning** – Find and connect all clues to unlock the exit.  
5. **Losing** – Get caught by the ghost.

---

## Technical Specifications
### Core Scripts
- **Shared Data Class**  
  - Manages player inventory (items, keys).  
  - Stores all game clues and narration text.  
  - Contains the global end-game function.  

- **Animation Script**  
  - Uses colliders and triggers (`OnTriggerEnter`, `OnTriggerExit`) to play animations when interacting with objects.  

- **Output Script**  
  - Instantiates prefab game objects with applied forces (via Rigidbody) to simulate outputs.  

- **Collect Script**  
  - Uses collider logic + interaction key (`E`) to collect objects and update inventory.  

- **Ghost Mover Script**  
  - Controls ghost movement with **NavMeshAgent**.  
  - Handles patrol, chase, and attack states.  
  - Calls game-ending function on successful attack.  

- **Player Mover Script**  
  - Handles player movement (walk, run, jump).  
  - Manages camera control and interaction detection through a forward-facing collider.  

---

## Instructions
1. Explore the office and look closely at walls, computers, and scattered tools.  
2. Press **E** to collect items when looking directly at them.  
3. Use collected items and keys to unlock areas and solve puzzles.  
4. Stay alert — if the ghost sees you, it will chase you.  
5. Find the escape route before the ghost catches you.  

---

## Future Improvements
- Additional puzzle mechanics.  
- More varied ghost AI behaviors.  
- Expanded environments and escape routes.  
- Sound design for greater immersion.  

---

## Credits
Developed by **Adrian Cortez**  
Made with Unity and C#  

