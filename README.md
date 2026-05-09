# PyGhost Platformer 🎮

A dynamic, tile-based 2D platformer developed in Python. This project features a data-driven level system, custom physics, and a unique "Ghost" mechanic that transforms the player's state upon failure.

## 📖 Project Overview
**PyGhost Platformer** is an arcade-style game where the player must navigate through various levels, collect gems, and avoid lethal lava hazards to reach the exit door. 

The game stands out through its polished death animation: when the player hits an obstacle, they don't just disappear—they turn into a ghost and float to the heavens, signaling a level reset or game over.

## 🛠 Tech Stack & Specifications

### Languages & Libraries
*   **Python 3.x**: The core programming language.
*   **Pygame**: Used for rendering 2D graphics, handling keyboard input, and managing the game clock.
*   **JSON**: Acts as the database for level layouts, allowing for decoupled game logic and world design.

### Technical Features
*   **AABB Collision System**: Custom-coded collision detection for X and Y axes to ensure smooth movement against walls and platforms.
*   **Physics Engine**: Realistic gravity simulation with terminal velocity and jump impulse handling.
*   **Sprite Animation Controller**: A state-based animation system that flips and cycles through frames based on velocity and direction.
*   **Data-Driven World Building**: The `World` class parses JSON matrices into interactive game objects, making it easy to expand the game with new levels.

## 🎮 Gameplay & Controls
*   **Objective**: Collect gems for points and reach the door to progress to the next level. You have 3 lives.
*   **Left/Right Arrows**: Movement.
*   **Spacebar**: Jump.
*   **Mouse**: Interact with Menu and Restart buttons.

## 📂 Project Structure
*   `main.py`: The entry point containing the Game Loop and Class definitions.
*   `levels/`: JSON files defining the grid (1=Dirt, 2=Grass, 3=Lava, 4=Door, 5=Gem).
*   `images/`: All visual assets including sprites and background.
*   `music/`: Sound effects (SFX) for jumps, gems, and game over states.

*   ## 📝 Level Editor Legend
If you wish to modify the levels in the `/levels` folder, use these IDs:
- **1**: Dirt Block
- **2**: Grass Block
- **3**: Lava (Hazard)
- **4**: Exit Door
- **5**: Collectible Gem

---
**Developed by Adrian-weber7** – 2026  
*This project is open-source. Feel free to fork and add your own mechanics!*
