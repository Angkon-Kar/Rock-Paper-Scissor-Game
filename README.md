# ⚔️ Rock Paper Scissors — Terminal Battle RPG

> *A classic game. A dark enemy. A fight for survival.*

A terminal-based Rock Paper Scissors game built in C++ — reimagined as an RPG boss battle. Fight **THE DARK AI** in a retro-style combat experience with health bars, critical hits, and ASCII art weapons.

---

## 🎮 Gameplay Preview

```
========================================
INITIALIZING BATTLE PROTOCOLS...
WARNING: OPPONENT 'THE DARK AI' DETECTED.
========================================

YOU (HERO)
 [||||||||||||||||    ] 80/100 HP

THE DARK AI (BOSS)
 [||||||||||||        ] 60/100 HP

----------------------------------------
WEAPON SELECTION: [1] Stone  [2] Paper  [3] Scissors
Action: _
```

---

## ✨ Features

- 🗡️ **RPG-style combat** — Health bars, damage system, and a final boss
- ⚡ **Critical Hits** — 20% chance to deal double damage (40 HP instead of 20)
- 🎨 **ANSI Color UI** — Color-coded HUD for player vs boss
- ⌨️ **Typewriter effect** — Retro character-by-character text intro
- 🪨 **ASCII Art weapons** — Stone, Paper, and Scissors rendered in ASCII
- 🛡️ **Input validation** — Handles bad input without crashing
- 🏆 **Win/Lose screens** — Mission accomplished or system shutdown ending

---

## 🛠️ Tech Stack

| Tool | Detail |
|------|--------|
| Language | C++17 |
| Libraries | `<iostream>`, `<thread>`, `<chrono>`, `<cstdlib>` |
| Platform | Windows (uses `system("cls")`) |
| Compiler | g++ / MSVC |

---

## 🚀 Getting Started

### Prerequisites
- A C++ compiler (g++, MSVC, or Clang)
- C++17 or later

### Compile & Run

**Using g++:**
```bash
g++ -std=c++17 -o rps_battle main.cpp
./rps_battle
```

**Using MSVC (Windows):**
```bash
cl /EHsc /std:c++17 main.cpp
rps_battle.exe
```

---

## 🎯 How to Play

1. Run the game and wait for the intro sequence
2. Choose your weapon each round:
   - `1` → 🪨 Stone
   - `2` → 📄 Paper
   - `3` → ✂️ Scissors
3. Deplete the Boss's 100 HP before yours hits 0
4. Each win deals **20 damage** (or **40** on a critical hit!)
5. First to reach 0 HP loses

---

## 📐 Game Logic

| You \ Boss | Stone | Paper | Scissors |
|-----------|-------|-------|----------|
| **Stone** | Draw | Lose | Win |
| **Paper** | Win | Draw | Lose |
| **Scissors** | Lose | Win | Draw |

- **Normal hit:** 20 HP damage
- **Critical hit (20% chance):** 40 HP damage
- **Draw:** No damage dealt

---

## 👨‍💻 Author

Built with passion for C++ and retro terminal aesthetics.  
Feel free to fork, improve, and make it your own!

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).