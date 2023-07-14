![Badge em Desenvolvimento](https://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)

# Chess System in Java

This is a Java project for a chess game. It allows players to play chess against each other using the command line interface. The project is implemented using object-oriented programming principles and follows a layered architecture pattern.

## Class Diagram

![](https://github.com/jbrun0r/assets/blob/main/chess-system-design.png?raw=true)

## Class Details

### Position

- Class representing a position on the chess board.
- Encapsulates the row and column of a position.
- Provides constructors and methods for accessing and manipulating positions.
- Overrides the `toString()` method to provide a string representation of the position.

### Piece

- Abstract class representing a chess piece.
- Provides basic functionality and common attributes for all chess pieces.
- Subclasses of `Piece` implement specific types of chess pieces, such as Rook, King, Pawn, etc.
- Includes methods for checking if a piece can move to a given position and calculating its possible moves.

### Board

- Class representing the chess board.
- Encapsulates a 2D array (matrix) of `Piece` objects.
- Provides methods for accessing and manipulating the pieces on the board.
- Includes methods for validating positions, checking if a piece exists at a given position, etc.

### ChessPiece

- Subclass of `Piece` representing a chess piece with additional properties and functionality specific to a chess game.
- Adds a `color` property to differentiate between black and white pieces.
- Overrides the `toString()` method to provide a string representation of the piece.

### ChessMatch

- Class representing a chess match.
- Orchestrates the flow of the game, including handling turns, making moves, checking for check and checkmate, etc.
- Uses instances of `Board` and `Player` to manage the state of the game.
- Provides methods for performing chess moves, validating positions, and checking for check and checkmate.

### ChessConsole

- Class providing a command line user interface for playing chess.
- Handles user input and displays the chess board and game information.

## Usage

To use the chess system, run the ChessConsole class, which provides a command-line interface for playing chess. The game will prompt you for input and display the current state of the chess board.
