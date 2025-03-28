# Tic_Tac_Toe
## Tic-Tac-Toe Game (Player vs Computer)
This is a simple console-based Tic-Tac-Toe game where you can play against the computer. The game will display a 3x3 board and you, as the player, will place 'X' while the computer places 'O'. The game continues until there is either a winner or a tie.

## Features:
Single-player gameplay: Player (X) vs Computer (O)

Computer will select a move via this priority:
     1. Win the game
     2. Block the player from winning the game
     3. Select the center space
     4. Select a corner
     5. Select a random space

Board drawing after each move

Win and tie detection

## How to Play:
The game will display the Tic-Tac-Toe board with positions numbered 1 to 9.

The player will be prompted to choose a position (from 1-9) to place their marker ('X').

After the player’s move, the board will be redrawn, and then the computer will randomly place its marker ('O').

The game checks for a winner or a tie after each move.

If there is a winner, a message will indicate whether the player has won or lost.

If the game ends in a tie, a message will notify you of the tie.

## Setup and Compilation:
### Requirements:
A C++ compiler (e.g., GCC or Clang)

### Compilation:
To compile the program, use the following command:

bash
Copy
Edit
g++ -o tic_tac_toe tic_tac_toe.cpp
### Running the Game:
After compiling, run the game using:

bash
Copy
Edit
./tic_tac_toe
Example of the Game Output:

     |     |     
  1  |  2  |  3  
_____|_____|______
     |     |     
  4  |  5  |  6  
_____|_____|______
     |     |     
  7  |  8  |  9  
     |     |     

Enter a spot to place a marker (1-9): 3

     |     |     
     |     |  X  
_____|_____|______
     |     |     
     |     |    
_____|_____|______
     |     |     
     |     |    
     |     |     

## Functions:
void drawBoard(char *spaces)
Draws the current Tic-Tac-Toe board.

void playerMove(char *spaces, char player)
Prompts the player to make a move, placing their marker ('X') at a valid position.

void computerMove(char *spaces, char computer)
Randomly selects a valid position for the computer to place its marker ('O').

bool checkWinner(char *spaces, char player, char computer)
Checks whether there is a winner. Returns true if a winner is found and displays a message.

bool checkTie(char *spaces)
Checks if the game has ended in a tie (all spaces are filled). Returns true if it's a tie.

## Contributions:
Feel free to fork this repository and make improvements!
