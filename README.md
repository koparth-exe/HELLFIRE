# 🎮 HELLFIRE: The Last Ember

A browser-based 2D action-adventure RPG built as a single HTML game using JavaScript and Phaser 3.60.

## 🔥 Play the Game

**Live Game:** https://hell-fire.netlify.app/

**Architecture Website:** 
https://hell-fire-architecture.netlify.app/

The architecture website provides an interactive visual representation of the game's actual client-side runtime architecture and signal flow.

## 🎮 Game Overview

HELLFIRE: The Last Ember is a 2D cinematic action-adventure RPG set in the Ashen Keep.

The game combines exploration, platforming, combat, NPC interactions, collectibles, checkpoints, and a multi-phase boss encounter.

## 🏗️ Architecture

HELLFIRE uses a client-side browser architecture.

```text
Browser
   ↓
HTML / CSS
   ↓
Inline JavaScript
   ↓
Phaser 3.60 Runtime
   ↓
GameScene
   ├── Player / Input / Physics
   ├── Enemies / Combat
   ├── Fallen King: Ignivar
   ├── NPCs / Dialogue
   ├── Checkpoints / Collectibles
   └── HUD / Camera / Effects
   ↓
Browser localStorage
   ↓
Save / Load Progress
```

### Main Runtime Flow

1. The browser loads the HTML document.
2. HTML and CSS provide the game container, interface, and controls.
3. Inline JavaScript contains the game logic, scenes, assets, audio, and gameplay systems.
4. Phaser 3.60 is loaded from an external CDN and provides rendering, Arcade Physics, input handling, and scene management.
5. The Phaser runtime starts the game and launches the GameScene.
6. GameScene creates the world and connects the main gameplay systems.
7. Browser localStorage is used for local save and load persistence.

## ⚔️ Gameplay Systems

### Player, Input, and Physics

Handles player movement, jumping, attacks, interactions, and physics.

### Enemies and Combat

Controls enemy behaviour, combat interactions, attacks, and hit events.

### Fallen King: Ignivar

The main boss encounter uses multiple phases. The boss changes behaviour as its health reaches the defined phase thresholds.

### NPCs and Dialogue

NPCs provide story interactions and dialogue throughout the Ashen Keep.

### Checkpoints and Collectibles

Checkpoints provide save points and restore player resources. Collectibles include embers and coins.

### HUD, Camera, and Effects

The HUD displays gameplay information while the camera follows the player and visual effects provide particles and combat feedback.

## 💾 Save System

The game uses the browser's `localStorage` instead of a separate backend server.

Player progress can include values such as:

- Position
- Level
- XP
- HP and maximum HP
- MP and maximum MP
- Gold
- Embers
- Player statistics

This allows the game to restore local progress when it is loaded again.

## 🛠️ Technology Stack

- HTML5
- CSS3
- JavaScript
- Phaser 3.60
- Phaser Arcade Physics
- Browser localStorage
- External Phaser CDN

## 🌐 Architecture

The interactive architecture is available here:

**https://koparth-exe.github.io/HELLFIRE/**

It visualizes:

- Primary runtime path
- Phaser runtime
- GameScene
- Gameplay systems
- Boss flow
- Save and load path
- External Phaser dependency
- Client-side browser boundary

## 📁 Project Structure

The main game is implemented as an HTML file containing the page structure, styling, JavaScript game logic, and Phaser configuration.

```text
HELLFIRE/
└── index.html
```

## ▶️ Run Locally

Because the game is browser-based, it can be opened locally in a modern browser.

1. Clone or download the repository.
2. Open the main HTML file in a browser.
3. Start playing.

An internet connection may be required for external CDN resources such as Phaser and web fonts.

## 🎯 Project Highlights

- Browser-based gameplay
- Client-side architecture
- Phaser 3.60 game engine
- Arcade Physics
- Exploration and platforming
- Combat system
- Multi-phase boss battle
- NPC dialogue
- Checkpoints
- Collectibles
- Local save and load system
- Desktop and touch-oriented controls

## 👤 Credits

Created by **Parth Korgaonkar**.

HELLFIRE: The Last Ember is a personal game development project focused on combining game design, programming, interactive systems, and visual presentation.
