# 🎮 Inception Tic Tac Toe

> *A dream within a dream — strategy layered inside strategy.*

---

## 🧠 Overview

**Inception Tic Tac Toe** is an advanced, multi-layered version of the classic Tic Tac Toe game. Instead of a single 3×3 grid, this game introduces a **recursive structure**:

* A **macro-board (3×3)**
* Each macro cell contains a **micro-board (3×3 Tic Tac Toe)**

This creates a **game within a game**, requiring players to think at both tactical (micro) and strategic (macro) levels simultaneously.

---

## 🎯 Core Idea

To win:

1. Compete in individual **micro-boards**
2. Win micro-boards to **claim positions on the macro-board**
3. Form a **3-in-a-row on the macro-board**

This dual-layer mechanic introduces:

* Multi-level decision-making
* Positional foresight
* Trade-offs between local vs global advantage

---

## 🧩 Game Mechanics

### 🟦 Board Structure

* The game consists of **9 micro-boards**
* Each micro-board behaves like a normal Tic Tac Toe
* These are arranged into a **larger 3×3 macro-board**

---

### ⚙️ Move Logic

* Players alternate turns (**X** and **O**)
* Each move is placed inside a micro-board
* A completed micro-board determines ownership of that macro cell

---

### 🏆 Winning Rules

#### Micro-board outcomes:

* ✅ Win → Claimed by the player
* ⚖️ Draw → Assigned to the **opponent** *(unique twist)*

#### Macro-board outcome:

* Form 3 in a row → **Win the game**
* All filled without a winner → **Draw**

---

## 🔥 Unique Twist

Unlike traditional nested Tic Tac Toe:

> **Drawn micro-boards are awarded to the opponent.**

This introduces:

* Counter-intuitive strategies
* Intentional forcing of draws
* Higher-level mind games

---

## 🤖 AI System

The game includes an AI opponent with progressively increasing intelligence.

### Difficulty Levels

| Level  | Behavior                            |
| ------ | ----------------------------------- |
| Easy   | Random moves + light heuristics     |
| Medium | Minimax (depth-limited)             |
| Hard   | Advanced Minimax with optimizations |

---

### 🧠 AI Techniques Used

* **Minimax Algorithm**
* **Alpha-Beta Pruning**
* **Heuristic Evaluation Function**
* **Move Ordering**
* **Iterative Deepening**
* **Time-bound computation (~1.5s cutoff)**

The AI evaluates:

* Macro-board winning potential
* Micro-board control
* Positional weights
* Threat creation & blocking

---

## 🎮 Features

### 🕹️ Gameplay

* Single-player (vs AI)
* Local multiplayer (2 players)

### 🎨 UI/UX

* Responsive layout
* Clean minimal design
* Animated transitions
* Visual indicators for:

  * Wins
  * Draws
  * Claimed boards

### ⚡ Performance

* Efficient game state updates
* Optimized AI calculations
* Smooth rendering

---

## 🛠️ Tech Stack

| Layer     | Technology         |
| --------- | ------------------ |
| Structure | HTML5              |
| Styling   | CSS3               |
| Logic     | Vanilla JavaScript |

> No external frameworks or libraries used.

---

## 📁 Project Structure

```
├── index-3.html   # Complete game (HTML + CSS + JS)
```

---

## ▶️ Running the Project

No setup required.

### Option 1:

Open directly in browser:

```
double-click index-3.html
```

### Option 2:

Using terminal:

```bash
open index-3.html
```

---

## 📊 Design Considerations

* **Single-file architecture** for simplicity
* **State-driven rendering**
* Clear separation of:

  * Game logic
  * AI logic
  * UI rendering

---

## 🧪 Possible Enhancements

### Gameplay

* Online multiplayer (WebSockets)
* Undo/redo moves
* Replay system

### AI

* Monte Carlo Tree Search (MCTS)
* Reinforcement learning agent

### UI

* Dark mode
* Sound effects
* Animations for move transitions

### Engineering

* Modular JS structure
* Unit tests for game logic
* Performance profiling


---

## 🎬 Inspiration

Inspired by the idea of **nested realities**, this game mirrors the layered complexity seen in *Inception*, translating it into a strategic board game format.

---

## 🤝 Contribution

Contributions are welcome. You can:

* Improve AI logic
* Enhance UI/UX
* Refactor code structure
* Add new game modes

---

## 📄 License

Open-source and free to use.

---

## ⭐ If you like this project

Give it a star ⭐ and share feedback!
