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
Brick Breaker is an engaging arcade game where players control a paddle to bounce a ball and break bricks. This implementation features smooth graphics, power-ups, and modern gaming elements while maintaining the classic gameplay that made the original game a success.

## 💻 Requirements
- Windows Operating System
- Microsoft Visual Studio (2019 or later)
  - Desktop development with C++ workload must be installed
  - Windows SDK must be installed
- Minimum screen resolution: 1024x768

## 🚀 Installation & Setup
1. **Visual Studio Installation**
   - Download and install Visual Studio from [official website](https://visualstudio.microsoft.com/)
   - During installation, select "Desktop development with C++" workload
   - Ensure "Windows SDK" is selected in the installation options

2. **Project Setup**
   - Open Visual Studio
   - Go to `File > New > Project`
   - Select `Empty Project` under C++ templates
   - Name your project and choose location
   - Click `Create`

3. **Adding Source Files**
   - In Solution Explorer, right-click on `Source Files`
   - Select `Add > Existing Item`
   - Browse and select `game.cpp`
   - Similarly, add `yourgraphics.h` to `Header Files`

4. **Configure Project Settings**
   - Right-click on your project in Solution Explorer
   - Select `Properties`
   - Under `Configuration Properties > Linker > Input`
   - Add `gdi32.lib` and `user32.lib` to `Additional Dependencies`
   - Click `Apply` and `OK`

5. **Build and Run**
   - Press `F5` to build and run the game
   - Or use `Build > Build Solution` (F7) and then run

## ⚠️ Common Issues
- If using MinGW or g++ directly, the compilation will fail due to Windows-specific graphics functions
- The game must be compiled using Visual Studio with the proper Windows SDK and libraries
- Make sure both `game.cpp` and `yourgraphics.h` are in the correct project directories

## ✨ Features
- **Modern Interface:** Clean and intuitive user interface
- **Game Modes:** 
  - New Game
  - Continue Saved Game
- **Save System:** 
  - Save progress at any time
  - Load previous saves
  - Auto-save on exit
- **Score System:**
  - High score tracking
  - Score comparison
  - Persistent leaderboard
- **Special Abilities:**
  - Paddle elongation power-up
  - Vertical paddle movement
  - Dynamic ball physics

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