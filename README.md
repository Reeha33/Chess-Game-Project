# Chess-Game-Project
Overview
This is a simple chess game implemented in C++. The game allows two players to play against each other on the same machine. The game features a text-based interface where the chessboard is displayed using ASCII characters. Players can move their pieces according to the standard rules of chess.

Features
Text-based Interface: The game uses a console-based interface to display the chessboard and handle player input.

Standard Chess Rules: The game follows the standard rules of chess, including special moves like pawn promotion.

Save and Load Game: Players can save their current game state and load it later to continue playing.

Turn-based Gameplay: The game alternates turns between two players, one controlling the white pieces and the other controlling the black pieces.

How to Play
Starting the Game:

Compile and run the program.

The game will prompt you to either start a new game or load a previous game.

Making Moves:

On your turn, the game will ask you to select a piece to move.

Enter the row and column of the piece you want to move.

Then, enter the row and column of the destination square.

The game will validate your move according to the rules of chess.

Special Moves:

Pawn Promotion: If a pawn reaches the opposite end of the board, it can be promoted to a queen, rook, bishop, or knight.

Saving and Loading:

The game automatically saves the current state after each move.

You can load the saved game by choosing the appropriate option when starting the game.

Code Structure
Main Functions:

gotoRowCol(int rpos, int cpos): Moves the cursor to the specified row and column in the console.

number(int K, int L): Displays numbers along the rows and columns of the chessboard.

print_board(int r, int c, char ch): Draws a single square of the chessboard.

one_box(int r, int c, char ch): Draws the entire chessboard.

init(char A[]): Initializes the chessboard with the starting positions of the pieces.

chang_turn(bool &turn): Switches the turn between the two players.

display(char A[]): Displays the current state of the chessboard.

ask_for_move(int &rf, int &cf, int &rt, int &ct, char &h, bool turn): Prompts the player to enter their move.

pawn(char A[], int rf, int cf, int rt, int ct): Validates pawn moves.

ruk(char A[], int rf, int cf, int rt, int ct): Validates rook moves.

bishop(char A[], int rf, int cf, int rt, int ct): Validates bishop moves.

knight(char A[], int rf, int cf, int rt, int ct): Validates knight moves.

king(char A[], int rf, int cf, int rt, int ct): Validates king moves.

queen(char A[], int rf, int cf, int rt, int ct): Validates queen moves.

legal_move(char A[], int rf, int cf, int rt, int ct, char h, bool turn): Checks if a move is legal.

position_update(char A[], int rf, int cf, int rt, int ct, char h): Updates the chessboard after a move.

ask(char &R): Asks the player if they want to start a new game or load a previous one.

Requirements
Compiler: A C++ compiler that supports the C++11 standard or later.

Operating System: The game should run on any operating system that supports a terminal or command prompt.
