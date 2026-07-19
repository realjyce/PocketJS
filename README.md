# PocketJS
A grid-based, 2D RPG engine built completely from scratch using vanilla JavaScript and the HTML5 Canvas API. Built from scratch with HTML5 Canvas and vanilla JavaScript.
(Definitely not inspired by that monster-catching game from the late '90s)


This project demonstrates the core architectural components of classic top-down RPGs—such as state management, collision detection, grid movement, and event-driven interaction loops—without relying on external game engines or frameworks.

## Key Features

- **Tile-Based Movement & Grid Collision:** Implements per-pixel interpolation for smooth grid-locked traversal and bounding-box collision detection.
- **Turn-Based Battle System:** A state-driven combat engine supporting speed-based turn order, dynamic move selection, and stat calculations.
- **NPC & Dialogue System:** An event-driven interaction queue handling collision-triggered events, dialogue rendering, and script sequencing.
- **State Persistence:** Custom local storage serialisation allowing complete player state, team data, and inventory progress to save and load across sessions.
- **Sprite Animation Pipeline:** Efficient sprite sheet parsing and rendering using HTML5 Canvas `drawImage`, managing direction-based animation loops at uniform frame rates.

## Tech Stack

- **Language:** Vanilla JavaScript (ES6+)
- **Rendering:** HTML5 Canvas API
- **Styling & Layout:** Core CSS3

## Core Architectural Focus

The primary goal of this project was to understand and implement low-level game loop architecture. Building the project without a framework required solving several foundational engineering problems:

- **The Game Loop:** Implementing a consistent `requestAnimationFrame` loop that decouples rendering updates from game logic processing.
- **State Management:** Routing active game scenes (Exploration, Dialogue, Battle) using a centralised state machine.
- **Resource Loading:** Handling asynchronous asset preloading (sprites, tilesets) before initialising the engine loop to prevent rendering glitches.

## Running the Project Locally

Clone the repository and host it locally using any static server. For example, using Python:

```bash
python -m http.server 8000
```
Then navigate to `http://localhost:8000` in your browser.

## Disclaimer

This project is an open-source educational exercise inspired by classic 2D RPGs. It is strictly non-commercial and holds no affiliation with any major gaming franchises.
