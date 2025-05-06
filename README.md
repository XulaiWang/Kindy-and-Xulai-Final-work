# 🚀 Start the Fight – A Pygame Air Battle Game

**Start the Fight** is a retro-inspired 2D airplane shooting game built using Python and Pygame. This game recreates the classic arcade feel of vertical 
        scrolling shooters many of us played during childhood — fast-paced action, bullet hell dodging, and satisfying explosions.

With custom images, background music, and immersive sound effects, the game brings a complete nostalgic arcade experience to your desktop.

---

## 🎮 How to Play

- **Move**: Use **arrow keys** (↑ ↓ ← →) or **WASD** to control your plane.
- **Shoot**: Automatically fire bullets.
- **Use Bomb**: Press **spacebar** when bombs are available to clear all enemies on screen.
- **Pause/Resume**: Click the top corner button using **mouse**.

---

## 🖱️ Mouse Support

- Click on pause/resume icons to control the game state.
- Icons change when hovered for interactive feedback.

---

## 🧩 Game Files Overview

| File/Folder | Description |
|-------------|-------------|
| `_start_the_fight.py` | Main game entry point |
| `myplane.py` | Player aircraft class and movement logic |
| `enemy.py` | Enemy behavior, including small/mid/big aircraft |
| `bullet.py` | Bullet creation, movement, and collision |
| `supply.py` | Power-up spawning and collection (bombs, double bullets) |
| `record.txt` | Stores the highest score (e.g., 1324000) |
| `images/` | Contains all sprites: background, player, enemies, UI buttons |
| `sound/` | Includes background music and SFX (bombs, shooting, power-ups) |
| `font/` | Contains custom .ttf font files used for in-game text rendering |

---

## 🔥 Difficulty Scaling (Dynamic)

The game increases difficulty based on your score:

| Level | Score Threshold | New Enemies Added                        | Speed Increase                |
|-------|------------------|------------------------------------------|-------------------------------|
| 1     | 0–50,000         | Default                                   | -                             |
| 2     | > 50,000         | +3 small, +2 mid, +1 big enemy            | +1 speed to small enemies     |
| 3     | > 300,000        | +5 small, +3 mid, +2 big enemy            | +1 speed to small & mid       |
| 4     | > 600,000        | +5 small, +3 mid, +2 big enemy            | +1 speed to small & mid       |
| 5     | > 1,000,000      | +5 small, +3 mid, +2 big enemy            | +1 speed to small & mid       |

Each level-up is accompanied by a unique upgrade sound.

---

## 💥 Power-Ups

- **Double Bullet**: Enhanced firepower for a short duration.
- **Bomb Supply**: Adds 1 bomb (max: 3) that can clear all on-screen enemies.

---

## 🛠 Requirements

```
pip install pygame
```

---

## ▶️ Run the Game

```
python _start_the_fight.py
```

---


Relive your childhood air combat experience and challenge your reflexes – can you beat the high score? 🎯
