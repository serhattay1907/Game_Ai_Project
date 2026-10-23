# 🎮 Connect 4 AI — Minimax with Alpha-Beta Pruning

A Connect 4 game in Python/Pygame with an AI opponent that searches the game tree using **Minimax with Alpha-Beta pruning**.

## 🧠 How the AI works
- **Minimax** explores future moves (default depth **5**), assuming both players play optimally
- **Alpha-Beta pruning** cuts branches that cannot change the result, making deeper search feasible
- **Heuristic evaluation** scores board windows of four: rewards own 2/3-in-a-row, blocks the opponent's, and prefers the center column

Change difficulty by editing the search depth in `connect4_with_ai.py`:
```python
col, score = minimax(board, 5, -math.inf, math.inf, True)
```

## ▶️ Run
```bash
git clone https://github.com/serhattay1907/Game_Ai_Project.git
cd Game_Ai_Project
pip install pygame numpy
python connect4_with_ai.py
```
You play red, the AI plays green. Move the mouse to pick a column, click to drop.

## ⚙️ Settings
| Setting | Default | Meaning |
|---|---|---|
| `ROW_COUNT` | 6 | Board rows |
| `COLUMN_COUNT` | 7 | Board columns |
| `SQUARESIZE` | 100 | Cell size (px) |
| depth | 5 | AI search depth |

## 📁 Also in this repo
`flappy.py` / `flappy_update.py` — a Flappy Bird clone written as Pygame practice (not part of the AI project).
