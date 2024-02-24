## [Live](https://m-ayan-k.github.io/Chess-Engine/)

# About

The primary concern of chess-engine is the decision-making part of the application. All functionality outside the scope of the chess-engine are implemented using external libraries:
* Chessboard GUI: Using the chessboard.js API
* Game Mechanics: Using the chess.js API

This engine uses the minimax algorithm, which is optimised by alpha-beta pruning.

The evaluation function uses piece [square tables](https://www.chessprogramming.org/Piece-Square_Tables) adapted from Sunfish.py, and eliminates the need for nested loops by updating the sum based on each move instead of re-computing the sum of individual pieces at each leaf node.

A global sum is used to keep track of black's evaluation score after each move, which is used to display the 'advantage' bar.
