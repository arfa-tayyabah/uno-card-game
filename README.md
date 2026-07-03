<div align="center">

# 🎴 UNO — Built on a Stack

### A desktop UNO card game in C++ where the entire game engine is powered by one data structure: the Stack.

<img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++" />
<img src="https://img.shields.io/badge/Raylib-FFC229?style=for-the-badge&logo=raylib&logoColor=black" alt="Raylib" />
<img src="https://img.shields.io/badge/Data%20Structure-Stack%20(LIFO)-0e75b6?style=for-the-badge" alt="Stack (LIFO)" />

</div>

---

## 📖 Overview

This is a fully playable, graphical UNO implementation in C++ — built to answer one question: *how far can a single data structure take you?*

Every part of the game — the draw pile, the discard pile, even each player's hand — is a **Stack**. No arrays standing in for game state, no shortcuts. The result is a real desktop game that also doubles as a working demonstration of LIFO logic applied to something more interesting than a textbook example.

The GUI runs on **Raylib**, rendering cards, hands, and the discard pile in real time and handling all mouse/keyboard input.

---

## 🎯 Objectives

- Model the complete UNO card game using stack-based logic
- Apply core data structure concepts to a real, interactive system
- Combine game logic with graphics programming
- Demonstrate event-driven programming with Raylib

---

## 🧱 Why a Stack?

UNO's rules map onto LIFO behavior more naturally than you'd expect:

- The **last card played** is always the one that matters next (top of the discard pile)
- **Drawing a card** is inherently a "pop from the top" operation
- **Push/pop** operations mirror exactly how a human handles a physical card pile

| Game Element | Stack Usage |
|:---|:---|
| Draw Pile | Stack of cards available to draw |
| Discard Pile | Stack of played cards |
| Player Hands | Each player's cards stored in their own stack |
| Action Handling | LIFO behavior naturally matches how card effects resolve |

---

## ✨ Features

- Complete UNO gameplay logic
- Stack-based card playing and discarding
- Card validation rules for legal plays
- Turn-based gameplay system
- Graphical interface showing live game state
- Dynamic, resizable stack implementation (custom template class)
- Event-based input handling via Raylib

---

## 🃏 Game Components

**Card structure** — every card has:
- **Color:** Red, Blue, Green, Yellow, or Wild
- **Value:** Numbers 0–9, or an action type (Skip, Reverse, Draw Two, Wild)

**Player** — each player has:
- A stack representing their hand
- Turn management logic
- Move validation before a card can be played

**Deck system:**

| Stack | Purpose |
|:---|:---|
| Draw Stack | Holds all remaining undrawn cards |
| Discard Stack | Stores every card that's been played |

---

## 🔄 Game Flow

1. The deck is initialized and shuffled.
2. Cards are dealt and pushed onto each player's hand stack.
3. One card is placed in the discard pile to start play.
4. Players take turns, either:
   - Playing a valid card, or
   - Drawing from the draw stack.
5. Action cards (Skip, Reverse, Draw Two, Wild) trigger their special effects.
6. The first player to empty their stack wins.

---

## 🧰 Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++" />
  <img src="https://img.shields.io/badge/Raylib-FFC229?style=for-the-badge&logo=raylib&logoColor=black" alt="Raylib" />
  <img src="https://img.shields.io/badge/Custom%20Template%20Stack-333333?style=for-the-badge" alt="Custom Template Stack" />
</p>

| Technology | Role |
|:---|:---|
| C++ | Core programming language |
| Stack (template implementation) | Primary data structure driving all game logic |
| Raylib | Graphics rendering and user interface |

---

## ▶️ Compilation & Execution

**Requirements:**
- A C++ compiler (GCC, MinGW, or Visual Studio)
- [Raylib](https://www.raylib.com/) installed and configured

**Build (example with g++):**

```bash
g++ unoGUI_Complete.cpp -o uno -lraylib -lopengl32 -lgdi32 -lwinmm
./uno
```
*(exact linker flags depend on your OS/setup — see the [Raylib build docs](https://github.com/raysan5/raylib/wiki) for your platform)*

---

## 🧑‍💻 Author

Developed as an academic project to demonstrate how core data structures — here, the Stack — can drive a fully interactive, graphical application, not just solve textbook problems.

---

## 🏁 Conclusion

This project shows that a single, well-understood data structure can carry the logic of a genuinely complex system. Building UNO around a Stack wasn't the easy path — it was the point: to prove that fundamentals, applied deliberately, are enough to build something real.

<div align="center">

**Part of my [GitHub profile](https://github.com/arfa-tayyabah) — see the full README for more projects.**

</div>
