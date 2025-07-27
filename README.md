# 🎮 Brick Breaker Game

[![Language](https://img.shields.io/badge/language-C++-blue.svg)](https://isocpp.org/)
[![Platform](https://img.shields.io/badge/platform-Windows-lightgrey.svg)](https://www.microsoft.com/windows)
[![IDE](https://img.shields.io/badge/IDE-Visual%20Studio-purple.svg)](https://visualstudio.microsoft.com/)

A classic arcade-style brick breaker game implemented in C++ with modern features and smooth gameplay.

**Author:** Muhammad Husnain Ali

## 📋 Table of Contents
- [Overview](#overview)
- [Requirements](#requirements)
- [Installation](#installation)
- [Features](#features)
- [Game Controls](#game-controls)
- [Game Rules](#game-rules)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview
Brick Breaker is an engaging arcade game that combines classic gameplay with modern features. Built using C++ and Windows GDI for graphics rendering, this implementation offers a smooth and responsive gaming experience. The game features a dynamic ball-and-paddle system where players must strategically bounce the ball to destroy bricks while managing power-ups and avoiding obstacles.

### Technical Highlights
- **Graphics Engine:** Custom-built using Windows GDI for efficient 2D rendering
- **Collision System:** Precise collision detection for ball-brick and ball-paddle interactions
- **State Management:** Robust game state handling with save/load functionality
- **Performance:** Optimized frame rate and smooth animations
- **Memory Management:** Efficient C++ memory handling for game objects

### Game Architecture
- **Main Game Loop:** Implements a fixed time-step game loop for consistent physics
- **Object-Oriented Design:** Modular code structure with separate classes for:
  - Game objects (Ball, Paddle, Bricks)
  - Collision management
  - Power-up system
  - Score tracking
  - State persistence

### Visual Elements
- **Dynamic Graphics:** Smooth animations and visual effects
- **Color Schemes:** Visually distinct brick types and power-ups
- **UI Elements:** 
  - Real-time score display
  - Life counter
  - Power-up indicators
  - Game status messages

### Gameplay Mechanics
- **Progressive Difficulty:** Increasing challenge as levels advance
- **Brick Varieties:**
  - Standard bricks (1 hit)
  - Reinforced bricks (multiple hits)
  - Special bricks (trigger power-ups)
- **Ball Physics:**
  - Realistic bounce angles
  - Speed variations
  - Collision response
- **Paddle Features:**
  - Smooth movement control
  - Size modifications through power-ups
  - Position-based ball deflection

## 💻 Requirements
- Windows Operating System
- Microsoft Visual Studio (2022 or later)
  - Desktop development with C++ workload must be installed
  - Windows SDK must be installed
- Minimum screen resolution: 1024x768

## 🚀 Installation & Setup
1. **Prerequisites**
   - Install Visual Studio 2022 or later from [official website](https://visualstudio.microsoft.com/)
   - During installation, make sure to select "Desktop development with C++" workload

2. **Create New Project**
   - Open Visual Studio
   - Click `Create a new project`
   - Search for and select `Empty Project` (C++)
   - Choose a name for your project and click `Create`

3. **Add Project Files**
   - Copy `game.cpp` and `yourgraphics.h` into your project folder
   - In Solution Explorer, right-click on `Source Files` → `Add` → `Existing Item`
   - Select `game.cpp`
   - Right-click on `Header Files` → `Add` → `Existing Item`
   - Select `yourgraphics.h`

4. **Run the Game**
   - Press `F5` to build and run
   - Or use the green play button in the toolbar

## ⚠️ Common Issues
- If using MinGW or g++ directly, the compilation will fail due to Windows-specific graphics functions
- The game must be compiled using Visual Studio with the proper Windows SDK and libraries
- Make sure both `game.cpp` and `yourgraphics.h` are in the correct project directories

## ✨ Features
- **Game Modes:** 
  - Classic Mode: Traditional brick-breaking gameplay
  - Time Trial: Clear levels against the clock
  - Endless Mode: Play until you run out of lives
  - Practice Mode: Perfect your skills without life limits

- **Level System:**
  - Multiple unique level layouts
  - Progressive difficulty scaling
  - Special challenge levels
  - Custom level completion requirements

- **Power-up System:**
  - Paddle Extensions: Increase paddle size
  - Multi-Ball: Split ball into multiple instances
  - Speed Modifiers: Adjust ball and paddle speed
  - Special Powers: Extra lives, point multipliers
  - Power-up stacking mechanics

- **Score System:**
  - Dynamic point multipliers
  - Combo bonuses for consecutive breaks
  - Time-based bonus points
  - Global and local high scores
  - Detailed statistics tracking

- **Save System:** 
  - Multiple save slots
  - Auto-save checkpoints
  - Progress persistence
  - Achievement tracking
  - Profile management

- **Technical Features:**
  - Smooth 60 FPS gameplay
  - Responsive controls
  - Collision prediction
  - Physics-based ball movement
  - Optimized performance

- **Audio System:**
  - Sound effects for collisions
  - Background music
  - Dynamic audio feedback
  - Volume controls

## 🎮 Game Controls
| Key | Action |
|-----|--------|
| `W` | Move Up |
| `S` | Move Down |
| `A` | Move Left |
| `D` | Move Right |
| `P` | Pause Game |
| `U` | Unpause Game |
| `K` | Save Game |
| `L` | Load Game |
| `Q` | Quit Game |
| `E` | Activate Power-up |

## 📜 Game Rules
1. **Lives System:**
   - Start with 3 lives
   - Lose a life when ball falls below paddle
   - Game over when all lives are lost

2. **Scoring:**
   - Break bricks to earn points
   - Different brick types yield different scores
   - High scores are saved automatically

3. **Power-ups:**
   - Paddle elongation available once per game
   - Power-up effect lasts for limited time
   - Strategic timing is crucial

## 📁 Project Structure
```
brick-breaker/
├── game.cpp           # Main game logic
├── yourgraphics.h     # Graphics library
├── highscore.txt      # Score database
├── Saved_Game.txt     # Save state file
└── README.txt         # Documentation
```

## 🤝 Contributing
1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">
Made with ❤️ by Muhammad Husnain Ali
</div>