# 👻 Ghost Escape Room

## Overview
Ghost Escape Room is a **first-person horror puzzle escape room game**.  
You play as an office worker who overslept and finds themselves locked inside the building.  
To escape, you must uncover clues, collect tools, and solve puzzles — all while avoiding a deadly ghost.  

## [Link to Game Files](https://drive.google.com/file/d/1eMjn9RdXzVpOdtdSqfqwnfNwNxEeNzsc/view?usp=drive_link)  

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

## 💻 System Requirements

### Windows
- OS: Windows 10 or later
- Processor: Intel i5 or equivalent
- RAM: 8 GB
- Graphics: DirectX 11 compatible GPU
- Storage: ~1 GB available space

---

## ▶️ How to Run the Game (Windows)

1. Download the ZIP file from the repository.
2. Extract the ZIP file (do **not** run the game from inside the ZIP).
3. Open the extracted folder.
4. Double-click: GhostGame.exe

⚠️ Make sure the `GhostGame_Data` folder is in the same directory as the `.exe` file.

---

## 🛠 How to Open the Project in Unity

If you want to edit or explore the project:

1. Install the correct Unity version used for development.
2. Open **Unity Hub**.
3. Click **Add Project**.
4. Select the extracted project folder.
5. Open the project.

> Note: Unity may re-import assets on first launch.

---

## 🎯 Controls

- **WASD** – Move  
- **Mouse** – Look around  
- **Left Click** – Interact  
- **Shift** – Sprint  
- **Esc** – Pause  

---

## 📁 Project Structure

- `Assets/` – Game scripts, scenes, models, audio, and prefabs  
- `ProjectSettings/` – Unity configuration files  
- `GhostGame.exe` – Playable build  
- `GhostGame_Data/` – Required game data files  

---

## Credits
Developed by **Adrian Cortez**  
Made with Unity and C#  

