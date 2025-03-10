# TicTacToeSolver_202401100400207

This is a Tic-Tac-Toe Solver game where a user ('O') competes against an AI ('X') that uses the Minimax algorithm to make optimal moves. The game runs in the terminal, allowing the player to enter row and column numbers (0-2) to make a move. The AI responds with the best possible move to maximize its chances of winning and minimizing oponent's chance of winning.

How to Play:-
Run the Python script in a terminal.
The empty board will be displayed.
The player enters their move by specifying the row and column numbers (0-2).
The AI calculates its best move using the Minimax algorithm.
The game continues until a player wins or all cells are filled (resulting in a draw).
The game announces the result: "You win!", "AI wins!", or "It's a draw!".

Algorithm Used: Minimax

What is Minimax?
The Minimax algorithm is a decision-making algorithm used in two-player games like Tic-Tac-Toe. It finds the optimal move by simulating all possible future moves and choosing the best outcome.

Why Minimax Works Well for Tic-Tac-Toe?
It is optimal → AI will never lose if played perfectly.
Explores all possibilities → Ensures the AI picks the best move.
Backtracking approach → It undoes moves to analyze different scenarios.

How Minimax Works in This Game:-
AI (Maximizing Player 'X') tries to maximize its score.
User (Minimizing Player 'O') tries to minimize the AI's score.
The algorithm explores all possible and optimal moves and assigns a score:
AI wins: +10
Human wins: -10
Draw: 0
The AI chooses the move that results in the highest possible score.

Code main Functions:-
print_board(board) → Displays the Tic-Tac-Toe board.
check_winner(board, player) → Checks if a player has won.
minimax(board, depth, is_max) → Uses the Minimax algorithm to evaluate the best possible move.
best_move(board) → Finds the best move for AI using Minimax.
play_game() → Manages the game loop, taking player input and calling AI moves.
