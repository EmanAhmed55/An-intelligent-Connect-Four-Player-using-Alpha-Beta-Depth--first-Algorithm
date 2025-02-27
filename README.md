<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">


</head>
<body>
    <h1>Connect Four Game</h1>

    <p>This is a two-player Connect Four game implemented using Python and Pygame. One player is controlled by the user (Player 1), while the other player (Player 2) is controlled by the AI using a Minimax algorithm with alpha-beta pruning for decision-making.</p>

    <h2>Features:</h2>
    <ul>
        <li>Player 1 (Human) uses the mouse to place pieces in the grid.</li>
        <li>Player 2 (AI) makes moves based on the Minimax algorithm.</li>
        <li>The game board is a 6x7 grid.</li>
        <li>The game continues until one player wins or the grid is full.</li>
    </ul>

    <h2>Game Mechanics:</h2>
    <p>The game is played on a 6-row by 7-column grid. The players take turns dropping their pieces into the columns. The first player to align 4 pieces in a row, either horizontally, vertically, or diagonally, wins the game. The AI player uses the Minimax algorithm to evaluate possible moves and make decisions based on the current state of the game.</p>

    <h2>Requirements:</h2>
    <ul>
        <li>Python 3.x</li>
        <li>Pygame Library</li>
    </ul>

    <h2>How to Run the Game:</h2>
    <p>To play the game, ensure you have Python 3 and Pygame installed. Follow the steps below:</p>
    <ol>
        <li>Clone the repository or download the Python script to your local machine.</li>
        <li>Install Pygame by running <code>pip install pygame</code> in your terminal or command prompt.</li>
        <li>Run the game script with the following command: <code>python connect_four_game.py</code></li>
        <li>The game window will open, and you can start playing. Player 1 is controlled by mouse input, and Player 2 is controlled by the AI.</li>
    </ol>

    <h2>Code Explanation:</h2>
    <p>The provided Python code implements the following key functions:</p>
    <ul>
        <li><strong>create_board</strong>: Initializes a 6x7 game board.</li>
        <li><strong>drop_piece</strong>: Drops a piece for the current player in the specified column.</li>
        <li><strong>is_valid_location</strong>: Checks if a column is open for placing a piece.</li>
        <li><strong>get_next_open_row</strong>: Returns the next available row for a given column.</li>
        <li><strong>winning_move</strong>: Checks if a player has won the game by aligning 4 pieces.</li>
        <li><strong>minimax</strong>: Implements the Minimax algorithm with alpha-beta pruning to determine the best move for the AI.</li>
        <li><strong>evaluate_window</strong>: Evaluates a "window" (a sequence of 4 consecutive cells) for scoring.</li>
        <li><strong>score_position</strong>: Scores the board based on potential winning moves.</li>
        <li><strong>pick_best_move</strong>: Picks the best move for the AI based on scoring.</li>
        <li><strong>draw_board</strong>: Draws the current state of the game board on the screen using Pygame.</li>
    </ul>

    <h2>Important Variables:</h2>
    <ul>
        <li><strong>ROW_COUNT</strong>: The number of rows in the game board (6).</li>
        <li><strong>COLUMN_COUNT</strong>: The number of columns in the game board (7).</li>
        <li><strong>PLAYER_PIECE</strong>: The piece used by Player 1 (Red).</li>
        <li><strong>AI_PIECE</strong>: The piece used by Player 2 (Yellow).</li>
        <li><strong>EMPTY</strong>: Represents an empty cell on the board.</li>
    </ul>

    <h2>Gameplay:</h2>
    <p>The game begins with an empty board. The players take turns, and Player 1 controls the red pieces while Player 2 (AI) controls the yellow pieces. The AI makes its move based on the Minimax algorithm, which analyzes the current board and evaluates potential moves to maximize the AI's chances of winning.</p>

    <p>Once the game ends (either due to a win or a tie), the result will be displayed on the screen, and the game will automatically restart after a short delay.</p>

    <h2>Example Screenshot:</h2>
    <img src="screenshot.png" alt="Screenshot of the Connect Four Game" style="width: 100%; max-width: 500px; border: 1px solid #ccc;">

    <h2>Contributors:</h2>
    <p>This project was developed by <strong>Your Name</strong>. Feel free to contribute, report issues, or suggest improvements.</p>

    <h2>License:</h2>
    <p>This project is licensed under the MIT License - see the <a href="LICENSE">LICENSE</a> file for details.</p>

</body>
</html>

