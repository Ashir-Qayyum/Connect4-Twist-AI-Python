# Connect 4 with Twist (Python + Pygame)

A modern twist on the classic Connect 4 game — now featuring row shifting mechanics and an AI opponent powered by Minimax with Alpha-Beta pruning. Built using Python 3, pygame, and numpy, this project delivers an interactive GUI and dynamic gameplay.

## 🎮 Features

*   ✅ Classic Connect 4 rules
*   ✅ Twist mechanic – shift any row left or right
*   ✅ Gravity automatically repositions pieces after a twist
*   ✅ AI opponent using Minimax with Alpha-Beta pruning
*   ✅ Player vs AI gameplay
*   ✅ GUI built in Pygame
*   ✅ Turn-based twist timing (based on move count)
*   ✅ Win detection: horizontal, vertical, and diagonal

## 🧠 Twist Mechanic

After a set number of moves:

*   Player and AI get the chance to twist any row
*   Row can shift left or right (circular rotation)
*   Gravity is reapplied to settle the pieces

Twist intervals depend on who starts:

| First Move | Twist Every (Player) | Twist Every (AI) |
| :--------- | :------------------- | :--------------- |
| Player     | 6 moves              | 3 moves          |
| AI         | 3 moves              | 6 moves          |

## 🤖 AI Logic

The AI uses:

*   Minimax Algorithm
*   Alpha-Beta Pruning
*   Depth = 5

Heuristic-based scoring:

*   Center column preference
*   Blocking opponent
*   Pattern evaluation (2s, 3s, 4-in-row)
*   Evaluates twist options using `ai_choose_twist()`

## 🧩 How to Play

1.  Run the Python script
2.  Click on a column to drop your piece
3.  When eligible, click a row (left/right mouse button) to twist
4.  AI plays automatically on its turn
5.  First to connect 4 wins (or draw)

## 📦 Requirements

Install dependencies before running:

```bash
pip install pygame numpy
```

## ▶️ Run the Game

```bash
python connect4_twist.py
```

## 📁 Project Structure

```
📂 Connect4-Twist
 └── connect4_twist.py     # Main script with GUI, AI, and game logic
 └── GUI Captures/         # GUI Screenshots
 └──Project Report         # Detailed Project Report
```

## ✨ Screenshots

<img width="699" height="725" alt="Basic Gaming 01" src="https://github.com/user-attachments/assets/8b3642e3-ecf5-4505-a384-6ec0160bd24f" />
<img width="698" height="723" alt="Before Twist 02" src="https://github.com/user-attachments/assets/db4a1083-e72e-4cc6-abca-cff328984b15" />
<img width="697" height="722" alt="Losing to AI 03" src="https://github.com/user-attachments/assets/804e9a05-40bf-4107-982b-ac6fe38c9bbe" />

## 🔧 Future Enhancements

*   Difficulty levels for AI
*   Restart/game menu
*   Sound effects & animations
*   Online/local 2-player mode
*   Custom twist settings
*   Stronger heuristic evaluation

## 📜 License

This project is for educational use. You may modify or extend it as needed.

## Developers

[Muhammad Ashir](https://github.com/Ashir-Qayyum)<br>
[Muhammad Anas](https://github.com/MrA006)<br>
[Muhammad Ammar](https://github.com/MuhammadAmmar7704)
