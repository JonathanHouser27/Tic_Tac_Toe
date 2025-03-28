# Tic_Tac_Toe
Tic-Tac-Toe Game (Player vs Computer)
This is a simple console-based Tic-Tac-Toe game where you can play against the computer. The game will display a 3x3 board and you, as the player, will place 'X' while the computer places 'O'. The game continues until there is either a winner or a tie.

Features:
Two-player gameplay: Player (X) vs Computer (O)

A randomized computer move

Board drawing after each move

Win and tie detection

How to Play:
The game will display the Tic-Tac-Toe board with positions numbered 1 to 9.

The player will be prompted to choose a position (from 1-9) to place their marker ('X').

After the player’s move, the board will be redrawn, and then the computer will randomly place its marker ('O').

The game checks for a winner or a tie after each move.

If there is a winner, a message will indicate whether the player has won or lost.

If the game ends in a tie, a message will notify you of the tie.

Setup and Compilation:
Requirements:
A C++ compiler (e.g., GCC or Clang)

Compilation:
To compile the program, use the following command:

bash
Copy
Edit
g++ -o tic_tac_toe tic_tac_toe.cpp
Running the Game:
After compiling, run the game using:

bash
Copy
Edit
./tic_tac_toe
Example of the Game Output:
mathematica
Copy
Edit
     |     |     
  X  |  O  |  X  
_____|_____|______
     |     |     
  O  |  X  |  O  
_____|_____|______
     |     |     
  X  |  O  |  X  
     |     |     

Enter a spot to place a marker (1-9): 3
Functions:
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

std::string getPlayerName()
Gets the player's name (currently not used in this version).

std::string getComputerName()
Gets the computer's name (currently not used in this version).

Contributions:
Feel free to fork this repository and make improvements!
