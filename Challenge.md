# 🧠 Memory Match Arena Hackathon  
### Progressive Game Development Challenge (Console → Desktop → Web)

---

## 📌 Overview

**Memory Match Arena** is a card-based memory game where players flip cards to find matching pairs.

This hackathon is designed as a **progressive engineering challenge**, where participants evolve their solution across three stages:

1. 🖥️ Console Application (Logic Validation)  
2. 🪟 Desktop Application (User Interaction)  
3. 🌐 Web Application (Scalability & Accessibility)  

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

Build the **Memory Match Arena** game step-by-step while ensuring:

- Strong **core logic foundation**
- Proper **separation of concerns**
- Reusability across platforms
- Incremental UI/UX improvements

---

## 🎨 Theme Selection (Mandatory)

Choose one theme for your cards:

- 🎨 Colors  
- 🌌 Star Wars characters  
- ⚡ Pokémon  
- 🌍 Countries & Flags  

> 💡 Optional: Integrate external APIs for dynamic card content

---

## ✅ Expected Deliverables

- ✔️ Fully working game logic  
- ✔️ Console-based version  
- ✔️ Desktop-based version  
- ✔️ Web-based version  
- ✔️ Reusable core engine  
- ✔️ Clean architecture  
- ✔️ `README.md` with setup instructions  

---

# 🛠️ Hackathon Tasks

---

## ✅ Task 1 — Console-Based Memory Game (Core Engine Validation)

### 🎯 Goal
Develop the complete game logic and validate it using a **console-based interface**.

---

### 📌 Scope

- Implement core game engine  
- Represent grid using text output  
- Accept user input (row, column)  
- Display card flips in console  

---

### ✅ Acceptance Criteria

- Grid initializes correctly with pairs  
- Cards are shuffled randomly each game  
- Player can flip only 2 cards per turn  
- Matching logic works correctly  
- Non-matching cards flip back (step-based or simulated delay)  
- Game ends when all pairs are matched  
- Input validation prevents invalid moves  

---

### 🎯 Evaluation Focus

- Logic correctness  
- State management  
- Code clarity and testability  

---

## ✅ Task 2 — Desktop Application (UI Integration)

### 🎯 Goal
Upgrade the console game into a **desktop-based interactive application**.

---

### 📌 Scope

- Use any GUI framework:
  - Tkinter / PyQt / etc.  
- Reuse the SAME core engine (no duplication)

---

### ✅ Acceptance Criteria

- Visual grid representation  
- Cards flip on user interaction (click events)  
- Match/mismatch reflected visually  
- Prevent rapid/invalid clicks (race condition handling)  
- Display:
  - Current player  
  - Matches found  
  - Game completion status  
- Reset functionality implemented  

---

### ⚠️ Key Constraint

> UI must only **call the core logic**  
> No game rules should exist inside UI code  

---

### 🎯 Evaluation Focus

- UI responsiveness  
- Proper integration with core logic  
- Separation of concerns  

---

## ✅ Task 3 — Web Application (Scalable Experience)

### 🎯 Goal
Transform the desktop application into a **web-based game**.

---

### 📌 Scope

Choose one:

- 🌐 Flask  
- ⚡ Streamlit  
- ⚛️ Any frontend framework (optional advanced track)

---

### ✅ Acceptance Criteria

- Game runs in a browser  
- Core engine reused without modification  
- Interactive card flipping  
- Game state persists correctly (session/state handling)  
- Match/mismatch logic works with delay  
- Game completion detection works  
- Basic responsive UI  

---

### 🚀 Bonus (Optional)

- Multiplayer mode  
- Leaderboard system  
- API-based dynamic cards  

---

### 🎯 Evaluation Focus

- Reusability of core logic  
- Web state management  
- UI/UX quality  

---
