## Tic Tac Toe Game Documentation
Overview
This project is a graphical implementation of the classic Tic Tac Toe game using Pygame. Players can choose to play against the computer, which makes random moves.

## Prerequisites
Python 3.x
Pygame
## Installation
Clone the repository:

git clone <repository-url>

## Install Pygame:

pip install pygame

## Running the Game
To start the game, run the main.py file:

python main.py

## Code Structure
Global Variables
->sign: Represents the player's sign (1 for cross, 0 for circle).
->csign: Represents the computer's sign (1 for cross, 0 for circle).
->board: A 3x3 matrix representing the Tic Tac Toe board, initialized with -1 indicating empty spots.
->white and black: Color definitions for the game.
->display_width and display_height: Dimensions of the game window.
->gameDisplay: The Pygame display surface.
## Functions
drawBoard()
Draws the Tic Tac Toe board.

drawCross(x, y)
Draws a cross (X) at the specified coordinates.

drawCircle(x, y)
Draws a circle (O) at the specified coordinates.

getStartingPoint(box)
Returns the starting pixel coordinates for drawing in the specified box.

boxLocation(mousePos)
Determines which box the mouse is pointing to based on its position.

screenMsg(text, size, center)
Displays a message on the screen at the specified position.

startScreen()
Displays the start screen where the player chooses their sign.

gameLoop()
Main game loop handling player moves and updating the display.

cmpPlay()
Handles the computer's move by randomly choosing an empty box.

checkMatch()
Checks for a winning condition or a draw.

checkWinner(w)
Determines the winner and calls the winnerScreen function.

winnerScreen(winner)
Displays the winner screen and offers to restart or quit the game.

gameReset()
Resets the game state for a new game.

## Game Flow
1.Start Screen: The player selects their sign (cross or circle).
2.Game Loop:
The player clicks on the board to make a move.
The computer makes a random move if it's its turn.
The game checks for a win or draw after each move.
3.Winner Screen: Displays the result and offers to restart or quit.
## Notes
The computer currently selects moves randomly. This can be enhanced with better AI.
The game uses simple Pygame graphics and a basic font for messages.
## Contributions
Contributions are welcome! Feel free to submit issues or pull requests.
