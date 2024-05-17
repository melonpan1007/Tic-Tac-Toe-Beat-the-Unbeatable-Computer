#Tic Tac Toe: Beat the Unbeatable Computer

This project is a console-based Tic Tac Toe game implemented in C++. The game allows a human player to challenge a computer with advanced decision-making logic designed to be very difficult to beat.

## How to Play


     |     |     
  1  |  2  |  3  
_____|_____|_____
     |     |     
  4  |  5  |  6  
_____|_____|_____
     |     |     
  7  |  8  |  9  
     |     |     



1. The game board is displayed with numbered positions from 1 to 9.
2. The player is prompted to enter a number between 1 and 9 to place their 'X' marker in the desired position.
3. The computer then makes its move with an 'O' marker based on its enhanced logic.
4. The game alternates between the player and the computer until there is a winner or a tie.

## Features

- **User-friendly Interface:** The game board is displayed after each move to show the current state.
- **Input Validation:** The player's input is validated to ensure it is within the correct range and that the chosen space is not already occupied.
- **Enhanced Computer Logic:** The computer uses a strategic approach to decide its moves, making it a tough opponent.

## Enhanced Computer Logic

The computer's decision-making process follows a prioritized strategy to ensure challenging gameplay:

1. **Win if possible:** The computer first checks if it can win in the next move. If a winning move is found, it makes that move.
2. **Block the player's win:** If the computer cannot win immediately, it checks if the player could win in their next move and blocks it.
3. **Play the center:** If the center space is available, the computer will take it, as it is the most advantageous position.
4. **Play a corner:** If the center is not available, the computer will choose a corner space.
5. **Play any empty space:** As a last resort, the computer will place its marker in any remaining empty space.

## Code Overview

### Main Loop

The main loop of the game alternates between the player's move and the computer's move, checking for a winner or a tie after each move.

### Key Functions

- `drawBoard(char *spaces)`: Draws the Tic Tac Toe board.
- `playersMove(char *spaces, char player)`: Handles the player's move.
- `computersMove(char *spaces, char computer)`: Implements the computer's enhanced logic for making a move.
- `checkWinner(char *spaces, char player, char computer)`: Checks if the given player has won.
- `checkTie(char *spaces)`: Checks if the game is a tie.
