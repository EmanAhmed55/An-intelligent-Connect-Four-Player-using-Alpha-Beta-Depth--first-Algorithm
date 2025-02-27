# Connect Four Game

This is a two-player Connect Four game implemented using Python and Pygame. One player is controlled by the user (Player 1), while the other player (Player 2) is controlled by the AI using a Minimax algorithm with alpha-beta pruning for decision-making.

## Features:
- Player 1 (Human) uses the mouse to place pieces in the grid.
- Player 2 (AI) makes moves based on the Minimax algorithm.
- The game board is a 6x7 grid.
- The game continues until one player wins or the grid is full.

## Game Mechanics:
The game is played on a 6-row by 7-column grid. The players take turns dropping their pieces into the columns. The first player to align 4 pieces in a row, either horizontally, vertically, or diagonally, wins the game. The AI player uses the Minimax algorithm to evaluate possible moves and make decisions based on the current state of the game.

## Requirements:
- Python 3.x
- Pygame Library

## How to Run the Game:
To play the game, ensure you have Python 3 and Pygame installed. Follow the steps below:
1. Clone the repository or download the Python script to your local machine.
2. Install Pygame by running the following command:
3. Run the game script with the following command:
4. The game window will open, and you can start playing. Player 1 is controlled by mouse input, and Player 2 is controlled by the AI.

## Code Explanation:
The provided Python code implements the following key functions:

- **create_board**: Initializes a 6x7 game board.
- **drop_piece**: Drops a piece for the current player in the specified column.
- **is_valid_location**: Checks if a column is open for placing a piece.
- **get_next_open_row**: Returns the next available row for a given column.
- **winning_move**: Checks if a player has won the game by aligning 4 pieces.
- **minimax**: Implements the Minimax algorithm with alpha-beta pruning to determine the best move for the AI.
- **evaluate_window**: Evaluates a "window" (a sequence of 4 consecutive cells) for scoring.
- **score_position**: Scores the board based on potential winning moves.
- **pick_best_move**: Picks the best move for the AI based on scoring.
- **draw_board**: Draws the current state of the game board on the screen using Pygame.

## Important Variables:
- **ROW_COUNT**: The number of rows in the game board (6).
- **COLUMN_COUNT**: The number of columns in the game board (7).
- **PLAYER_PIECE**: The piece used by Player 1 (Red).
- **AI_PIECE**: The piece used by Player 2 (Yellow).
- **EMPTY**: Represents an empty cell on the board.

## Gameplay:
The game begins with an empty board. The players take turns, and Player 1 controls the red pieces while Player 2 (AI) controls the yellow pieces. The AI makes its move based on the Minimax algorithm, which analyzes the current board and evaluates potential moves to maximize the AI's chances of winning.

Once the game ends (either due to a win or a tie), the result will be displayed on the screen, and the game will automatically restart after a short delay.

## Example Screenshot:
![Screenshot of the Connect Four Game](screenshot.png)

## Contributors:
This project was developed by **Your Name**. Feel free to contribute, report issues, or suggest improvements.

## License:
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.




