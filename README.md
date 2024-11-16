# PRODIGY_WD_03
interactive tic tac toe web application for prodigy infotech internship
Here’s a README file template for your Tic-Tac-Toe web application:

# Tic-Tac-Toe Web Application

This is a simple, interactive web-based Tic-Tac-Toe game built using HTML, CSS, and JavaScript. It allows two players to take turns playing the classic Tic-Tac-Toe game in their browser.

## Features

- **Turn-based Gameplay**: Players take turns placing their marks ('X' and 'O') on the grid.
- **Win Detection**: The game checks for winning patterns and displays the winner once a player achieves a win.
- **Reset Game**: Players can reset the game board after a win or draw using the "Reset" button.
- **New Game**: A fresh new game can be started using the "New Game" button, which resets the board and the turn sequence.

## How to Play

1. **Start the Game**: The game starts with player '0' (O). Players alternate turns clicking on any empty box to place their mark.
2. **Winning the Game**: A player wins by getting three marks (either 'X' or 'O') in a row, column, or diagonal.
3. **Resetting**: After a game is completed, use the "Reset" button to clear the board and start again.

## Features Breakdown

- **Turn Management**: The game alternates between two players – 'X' and 'O'.
- **Win Patterns**: The game checks all possible win patterns for both players.
- **Interactive UI**: Clickable boxes on the grid that are disabled after each move to prevent overwriting.
- **Dynamic Messages**: Displays a congratulatory message for the winner once the game ends.

## Technologies Used

- **HTML**: For structuring the Tic-Tac-Toe grid and UI elements.
- **CSS**: For styling the game board and buttons.
- **JavaScript**: For managing the game logic, including turn-based play, win detection, and game reset functionality.

## Code Explanation

### Main Variables

- `boxes`: Array of box elements representing the 3x3 grid.
- `resetBtn`: Button to reset the game.
- `newGameBtn`: Button to start a new game.
- `msgContainer`: Element to display the winner message.
- `msg`: Element that contains the winner message.

### Game Logic

- `turn0`: Boolean flag to track which player's turn it is. If `true`, it’s player 'O's turn; if `false`, it’s player 'X's turn.
- `winPatterns`: Array containing all possible winning combinations (rows, columns, and diagonals).
- `resetGame()`: Function to reset the game state, clearing the grid and resetting the turn.
- `checkWinner()`: Function to check if a player has won after every move.
- `disableBoxes()`: Disables all boxes (used when a winner is detected).
- `enableBoxes()`: Enables all boxes, clearing their content (used for new game or reset).

### Event Listeners

- **Box Click**: When a box is clicked, it is marked with either 'X' or 'O', and the game checks for a winner.
- **Reset Button**: Resets the game to its initial state.
- **New Game Button**: Starts a fresh game with a cleared grid and reset turn sequence.

## Installation

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/your-username/tic-tac-toe.git
   ```
2. Open the `index.html` file in a browser to play the game.

## License

This project is open-source and available under the MIT License. See the LICENSE file for more details.
