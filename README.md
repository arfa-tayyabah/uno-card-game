# UNO Card Game With Raylib GUI

## Project Overview

It is a desktop edition of the UNO card game implementation in C++, with the Stack data structure as the core mechanism which facilitates all operations of the cards. The graphical user interface (GUI) is developed with the help of the Raylib library that creates an interactive and visual experience during the gameplay.
This project is aimed at showing how one basic data structure, Stack (LIFO), can be used to represent an entire game system in the real world.

## Objectives

 - To UNO card game with stack-based reasoning.
 - To use data structures concepts in a real life application.
 - To combine games logic and graphics.
 - To illustrate event-based program in Raylib.

## Implementation of Data Structures

The Stack data structure is used in all important elements of the game.

| Game Element    | Stack Usage                                  |
| --------------- | -------------------------------------------- |
| Draw Pile       | Stack of cards to draw from                  |
| Discard Pile    | Stack of played cards                        |
| Player Hands    | Each player’s cards stored in a stack        |
| Action Handling | LIFO behavior matches card effects naturally |

### Rationale for Using Stack

 - The last card to be played should always be used first (top of discard stack).
 - LIFO behavior is naturally followed by drawing cards.
 - Push and Pop operations are good representations of real card handling.

## Graphical User Interface

The project is based on the Raylib C/C++ graphics library to:

 - Render cards on the screen
 - Showing hand and discard stack.
 - Process mouse and key input.
 - Control game window and frame rate.

Raylib allows the user to interact with game logic in real-time.

## Game Features

- Complete UNO gameplay logic  
- Stack-based card playing and discarding  
- Card validation rules for playable cards  
- Turn-based gameplay system  
- Graphical user interface displaying game state and cards  
- Dynamic stack implementation with resizing  
- Event-based user input handling  

---

## Game Components

### Card Structure

Each card consists of:

- **Color:** Red, Blue, Green, Yellow, or Wild  
- **Value:** Numbers (0–9) or action types (Skip, Reverse, Draw Two, Wild)

---

### Player

Each player includes:

- A stack representing their hand of cards  
- Turn management logic  
- Validation checks before playing a card  

---

### Deck System

| Stack Name     | Purpose                                  |
|----------------|-------------------------------------------|
| Draw Stack     | Holds all remaining cards to be drawn     |
| Discard Stack  | Stores cards that have been played        |

---

## Game Flow

1. The deck is initialized and shuffled.  
2. Cards are distributed to players and pushed into their stacks.  
3. The game begins with one card placed in the discard pile.  
4. Players take turns:  
   - Playing a valid card, or  
   - Drawing a card from the draw stack.  
5. Action cards trigger special effects.  
6. The winner is the first player to empty their stack.  


## Technologies Used

| Technology                        | Purpose                         |
|----------------------------------|----------------------------------|
| C++                              | Core programming language        |
| Stack (Template Implementation)  | Primary data structure           |
| Raylib                           | Graphics and user interface      |


## Compilation and Execution

### Requirements

- C++ compiler (GCC, MinGW, or Visual Studio)  
- Raylib library installed and configured  


## Author

Developed as an academic project to demonstrate the use of **data structures and graphical programming** in game development.

## Conclusion

This project demonstrates that the Stack data structure can effectively manage the logic of a complex card game like UNO. It reinforces the importance of fundamental data structures in the development of interactive and functional software systems.
