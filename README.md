# 🧱 BrickBreaker Game in Assembly

A retro-style **BrickBreaker** game built entirely using **x86 Assembly Language**, showcasing low-level programming concepts, graphics manipulation, and direct hardware interfacing. Designed for DOSBox or any compatible x86 emulator.

---

## 🎮 Game Overview

Control a paddle to bounce the ball and break all bricks on the screen. This game demonstrates real-time input handling, collision detection, graphics rendering using VGA mode, and performance-critical loops — all written in Assembly.

---

## ✨ Features

- 🕹️ Keyboard-controlled paddle movement
- 🧱 Dynamic brick layout
- 🏐 Ball physics with collision detection
- 💥 Brick destruction logic
- 🧠 Real-time rendering using VGA mode 13h
- 💾 Score tracking and file-saving support

---

## 🧰 Tech Stack

- **Language**: x86 Assembly (NASM / TASM / MASM syntax)
- **Platform**: DOS (emulated via DOSBox)
- **Graphics Mode**: VGA 320x200x256 (Mode 13h)
- **Tools**:
  - DOSBox (runtime)
  - NASM / TASM (assembler)
  - Debugger (e.g., TD or DOSBox Debug)

---

## 🕹️ Controls

| Key       | Action           |
|-----------|------------------|
| ← / →     | Move paddle left/right |
| Esc       | Quit the game     |

---

## 📂 File Structure

```
.
├── brickbreaker.asm     # Main game loop and logic
├── graphics.asm         # Low-level VGA graphics routines
├── input.asm            # Keyboard interrupt handler
├── collision.asm        # Ball-brick/paddle collision
├── score.asm            # Score tracking and file I/O
├── build.bat            # Assembly and linking script
├── README.md
```

---

## 🏗️ Build & Run Instructions

### 🛠 Requirements

- DOSBox installed: [Download](https://www.dosbox.com/)
- NASM or TASM installed (depending on your syntax)

### ▶️ Running in DOSBox

1. Assemble the code:
   ```bash
   nasm -f bin brickbreaker.asm -o brickbreaker.com
   ```

2. Launch DOSBox and mount your folder:
   ```bash
   MOUNT C /path/to/brickbreaker
   C:
   brickbreaker.com
   ```

3. Play and enjoy the nostalgic 8-bit vibes!

---

## 💾 Score Persistence

- Top score is stored in a `.dat` file.
- When a new high score is achieved, it updates the file for future sessions.

---

## 📸 Screenshots

> _(Insert screenshots or ASCII previews here if available)_

---

## 🤯 Learning Outcomes

- Writing performant code in low-level Assembly
- VGA graphics interfacing and pixel plotting
- Memory addressing and stack management
- Handling keyboard interrupts
- Managing timing without OS-level APIs

---

## 🚀 Future Improvements

- 🎵 Add PC speaker sound effects
- 🧱 Power-ups and multiple brick types
- 🔄 Multiple levels and increasing difficulty
- 📊 High-score leaderboard system


---

🧠 Made for fun, learning, and nostalgia. Relive the golden age of games — one opcode at a time.
