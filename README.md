# 💣 Bomberman DOM - Multiplayer Battle Arena 💥

## Overview

**Bomberman DOM** is a multiplayer browser-based game inspired by the classic Bomberman, developed using only the **DOM API** — no Canvas, no WebGL, and no external frameworks. It was built using our **custom mini-framework** from a previous project.

Up to **4 players** can join the game online and battle in real-time until only one remains standing. The game also features a built-in **WebSocket-based chat system** to allow players to communicate before and during the game.

This project emphasizes **performance**, ensuring smooth animations and responsiveness at a stable **60 FPS** using `requestAnimationFrame`.

---

## 👥 Team

- Abdelilah Bouchikhi  
- Rachid Serraf  
- Ayoub Lahmami  
- Yassin Kharkhach  

---

## 🚀 Features

- ⚔️ **Multiplayer Battle (2–4 players)** via WebSockets  
- 🕹️ **Smooth gameplay at 60 FPS** using requestAnimationFrame  
- 💬 **Integrated WebSocket chat** between players  
- 🎮 **Responsive DOM-based rendering** (no Canvas, WebGL, or frameworks)  
- 🧱 **Randomly generated breakable blocks + fixed unbreakable walls**  
- 💥 **Bombs and power-ups**:  
  - Extra Bombs (drop more at once)  
  - Flames (increase explosion radius)  
  - Speed (move faster)  

---

## 🧩 Game Mechanics

### Players
- Each player has **3 lives**.
- Start positions are fixed: one player per corner of the map.

### Map
- Fully visible to all players.
- Two block types:
  - **Walls**: fixed and indestructible
  - **Blocks**: destructible, placed randomly at game start
- Safe zones around players at the start to avoid immediate elimination.

### Bombs
- Explode in **four directions** (up, down, left, right).
- Explosion range can increase via power-ups.
- Can destroy blocks and eliminate players within range.

### Power-Ups (spawn randomly when blocks are destroyed)
- 🔸 **Bombs**: increase number of bombs a player can place at once  
- 🔸 **Flames**: extend explosion range  
- 🔸 **Speed**: increase movement speed  

---

## 🕓 Lobby & Match Start Logic

- On game load, users input a **nickname**.
- Players enter a **waiting lobby**, displaying a **player counter**.
- Start logic:
  - If **4 players** join: a **10-second countdown** begins, then the game starts.
  - If **2–3 players** join: wait **20 seconds**, then trigger a **10-second countdown** before the game starts.

---

## 🧠 Performance Goals

- Maintain **60 FPS at all times**.
- No frame drops, using `requestAnimationFrame` for all animations and game loops.
- DOM manipulation is **highly optimized** through our custom mini-framework.

---

## 💻 Tech Stack

- 🔧 **Custom Mini-Framework** (DOM-based, built in a previous project)
- 🌐 **WebSockets** for multiplayer sync and chat
- ⚙️ **Vanilla JavaScript**, HTML, and CSS (no Canvas, WebGL, or external libraries)
- 🔍 Developer Tools: Chrome & Firefox performance analyzers

---

## 💬 Chat System

- Realtime WebSocket-based messaging
- Available from the lobby and in-game
- Serves as a foundation for future multiplayer interactions

---

## 🌟 Bonus Ideas (Optional Additions - Not Implemented Yet)

- 🤖 AI opponents (Solo or Co-op mode)
- 🧠 Smarter power-ups:  
  - Bomb Push, Bomb Pass, Block Pass, Detonator, 1-Up
- 👻 Ghost mode: eliminated players can revive by touching teammates
- 🎯 2v2 Team Mode

---

## 📷 Screenshots

## 📸 Screenshots

### 👥 Waiting Room
![Waiting Room](./assets/readme/waitingPage.png)

### 🎮 Gameplay
![Gameplay](./assets/readme/gamePlay.png)

### 💣 Bombing Action
![Bombing](./assets/readme/bombing.png)

### 🔥 Explosion Effect
![Fire Effect](./assets/readme/fireEffect.png)

### 🏆 Win Screen
![Victory](./assets/readme/win.png)
---

## 🧪 How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/Abdelilah-99/Bomber-Man.git
   cd bomberman-dom

## 📄 License

All rights reserved. This project is intended for educational purposes only.

You may not reuse, modify, or distribute this code without written permission from the authors.
