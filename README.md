🎮 Connect 4 with AI

A fun Connect 4 game built with Python and Pygame, featuring a smart AI opponent powered by the Minimax algorithm with Alpha-Beta pruning.
-------------------------------------------------------------------------------------------------------------------------------------------
📖 Table of Contents

Overview  – What the game does

Installation  – How to set it up

How to Play
 – Game controls

AI Logic
 – How the AI works

Customization
 – Adjust settings

License
 – Usage rights
-------------------------------------------------------------------------------------------------------------------------------------------
🕹️ Overview

Play the classic Connect 4 against an intelligent AI.
Drop colored discs into a grid — the first to connect four in a row wins!

-------------------------------------------------------------------------------------------------------------------------------------------

⚙️ Installation

Set up and start the game in a few steps:

git clone https://github.com/yourusername/connect4_with_ai.git
cd connect4_with_ai
pip install pygame numpy
python connect4_with_ai.py


💡 Requires Python 3.8+
-------------------------------------------------------------------------------------------------------------------------------------------
🎮 How to Play

You play as red, the AI is green.

Move your mouse to select a column and click to drop your piece.

The AI will play automatically after your move.

The first to connect four pieces wins!
-------------------------------------------------------------------------------------------------------------------------------------------

🧠 AI Logic

The AI uses Minimax with Alpha-Beta pruning to find the best move.
It looks ahead a few moves (default depth = 5) and blocks or creates winning opportunities.
You can adjust its difficulty by changing the depth value in the code:

col, score = minimax(board, 5, -math.inf, math.inf, True) 
-------------------------------------------------------------------------------------------------------------------------------------------

🎨 Customization

You can tweak these values in the code:

Setting	Default	Description
ROW_COUNT	6	Number of board rows
COLUMN_COUNT	7	Number of columns
SQUARESIZE	100	Cell size (pixels)
depth	5	AI difficulty

Example:
ROW_COUNT = 8
COLUMN_COUNT = 8
SQUARESIZE = 80


ROW_COUNT = 8
COLUMN_COUNT = 8
SQUARESIZE = 80
