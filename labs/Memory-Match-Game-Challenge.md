# 🧠 Memory Match Arena Game Challenge

---

## 📌 Overview

**Memory Match Arena** is a card-based memory game where players flip cards to find matching pairs.

This hackathon is focused **on building a desktop application**. Participants will develop the game logic and integrate it into an interactive desktop user interface.

The challenge emphasizes:

- Strong **core game logic**
- Proper **separation of concerns**
- Reusable and maintainable code
- Interactive **desktop UI/UX**
- Incremental improvements to the application

> **Scope:** Build and submit a **single desktop application** for the entire challenge.

---

## 🧱 Game Mechanics

- **Grid Sizes**: 4×4 / 6×6 / 8×8
- **Cards**: Paired symbols placed randomly
- **Turn System**: Flip 2 cards per move
- **Match Rules**:
  - ✅ Match → Cards remain face up
  - ❌ No Match → Cards flip back after a delay
- **End Condition**: All pairs matched

---

## 🧩 Objective

Build the **Memory Match Arena desktop application** while ensuring:

- Strong **core logic foundation**
- Proper **separation of concerns**
- Reusable game components and logic
- Clear separation between **game logic and desktop UI**
- Incremental UI/UX improvements

---

## 🎨 Theme Selection (Mandatory)

Choose one theme for your cards:

- 🎨 Colors
- 🌌 Star Wars characters
- ⚡ Pokémon
- 🌍 Countries & Flags

> 💡 Optional: Integrate an external API for dynamic card content, provided it can be used appropriately by the desktop application.

---

## 🖥️ Desktop Application Requirements

### Recommended GUI Frameworks

Choose a desktop GUI framework appropriate for your programming language, such as:

- **Python**: Tkinter, PyQt, etc.
- **C#**: Windows Forms, WPF, etc.
- **Java**: JavaFX, Swing, etc.

The selected technology must produce a **desktop application with a graphical user interface**.

---

## ✅ Expected Deliverables

- ✔️ Fully working **desktop Memory Match Arena application**
- ✔️ Complete game logic
- ✔️ Interactive desktop UI
- ✔️ Reusable core game engine
- ✔️ Clean architecture
- ✔️ Selected card theme
- ✔️ Reset functionality
- ✔️ `README.md` with setup and execution instructions

---

# 🛠️ Hackathon Tasks

---

## ✅ Task 1 — Build the Core Game Engine

### 🎯 Goal

Develop the complete game logic that will be used by the desktop application.

### 📌 Scope

- Implement the core game engine
- Represent cards and pairs
- Generate the selected grid size
- Shuffle cards randomly
- Track card state
- Implement the turn system
- Validate card matches
- Track matched pairs
- Detect game completion
- Support game reset

### ✅ Acceptance Criteria

- Grid initializes correctly with pairs
- Cards are shuffled randomly each game
- Player can flip only 2 cards per turn
- Matching logic works correctly
- Non-matching cards flip back after a delay
- Matched cards remain face up
- Game ends when all pairs are matched
- Invalid moves are prevented
- Game can be reset and started again

### 🎯 Evaluation Focus

- Logic correctness
- State management
- Code clarity
- Testability
- Separation of concerns

---

## ✅ Task 2 — Build the Desktop User Interface

### 🎯 Goal

Create an interactive **desktop GUI** for the Memory Match Arena game.

### 📌 Scope

- Create the main desktop application window
- Display the game grid visually
- Represent each card as an interactive UI element
- Handle card click events
- Show card contents when selected
- Show matched cards as face up
- Hide non-matching cards after the required delay
- Connect the UI to the core game engine
- Provide a Reset/New Game option

### ✅ Acceptance Criteria

- Visual grid representation is available
- Cards flip on user interaction using click events
- Match/mismatch is reflected visually
- Rapid or invalid clicks are prevented
- The same card cannot be selected twice in one turn
- Only two cards can be selected per turn
- Matched cards remain visible
- Non-matching cards are hidden after the delay
- Game completion status is displayed
- Reset functionality is implemented

### ⚠️ Key Constraint

> **The UI must only call the core game logic.**
>
> Game rules should not be duplicated inside UI code or click handlers.

### 🎯 Evaluation Focus

- UI responsiveness
- Proper integration with core logic
- Separation of concerns
- User interaction quality

---

## ✅ Task 3 — Desktop Game Information & User Experience

### 🎯 Goal

Improve the desktop application so that the player can clearly understand the current state of the game.

### 📌 Scope

The application should display relevant information such as:

- **Current player**
- **Matches found**
- **Game completion status**
- Reset/New Game control

The UI should clearly communicate the result of each card selection and the overall progress of the game.

### ✅ Acceptance Criteria

- Current player information is visible
- Number of matches found is visible
- Game completion status is visible
- Reset/New Game works correctly
- The game remains responsive during card-flip delays
- The interface clearly distinguishes matched and unmatched cards

### 🎯 Evaluation Focus

- UI clarity
- Responsiveness
- User experience
- Visual feedback

---

## 🚀 Bonus Features (Optional)

Participants may extend the desktop application with additional features such as:

- Multiplayer mode
- Leaderboard system
- API-based dynamic cards

Any bonus feature must remain part of the **desktop application**.

---

## 🏁 Final Submission Checklist

Before submitting, verify that:

- [ ] The application starts successfully on a desktop environment
- [ ] The selected grid size works correctly
- [ ] Cards are shuffled randomly
- [ ] Exactly two cards can be flipped per turn
- [ ] Matching cards remain face up
- [ ] Non-matching cards flip back after a delay
- [ ] Invalid and rapid clicks are prevented
- [ ] All pairs can be matched successfully
- [ ] Game completion is detected
- [ ] Reset/New Game works correctly
- [ ] Current player, matches found, and completion status are displayed
- [ ] UI code does not contain duplicated game rules
- [ ] The project contains a clear `README.md`

---

## 📄 README.md Requirements

The `README.md` should include:

### 1. Project Overview

Briefly explain the Memory Match Arena desktop application.

### 2. Features

List the features implemented in the desktop application.

### 3. Technology Stack

Mention the programming language, desktop GUI framework, and relevant libraries.

### 4. Setup Instructions

Provide clear instructions for installing prerequisites and dependencies.

### 5. Run Instructions

Explain how to launch the desktop application.

### 6. Game Instructions

Explain how players interact with the game and how matching works.

### 7. Architecture

Briefly explain how the **core game logic** and **desktop UI** are separated.

### 8. Screenshots

Include screenshots of the completed desktop application.

### 9. Bonus Features

Mention any optional features implemented.

---

## 🏆 Challenge Outcome

The final submission should be a **complete, working, interactive desktop Memory Match Arena application** with:

> **Correct Game Logic + Clean Architecture + Responsive Desktop UI + Good User Experience**

The primary goal is not just to make the game work, but to demonstrate good software engineering practices while building a desktop application.
