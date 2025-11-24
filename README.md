# Half Chess Board - FEN Generator

A web-based chess board where two players can independently position pieces on their respective halves of the board, then generate FEN (Forsyth-Edwards Notation) representing the combined position.

## Features

- **Split Board Control**: Each player controls one half of the chess board
  - Player 1 (Black pieces): Ranks 5-8 (top half)
  - Player 2 (White pieces): Ranks 1-4 (bottom half)
- **Drag and Drop**: Intuitive piece movement within allowed areas
- **FEN Generation**: Convert the board position to standard FEN notation
- **Board Management**: Reset to starting position or clear all pieces

## How to Use

1. Open `index.html` in a web browser
2. Drag and drop pieces to position them on your half of the board:
   - Black pieces can only be placed on ranks 5-8 (top half)
   - White pieces can only be placed on ranks 1-4 (bottom half)
3. Click "Generate FEN" to create the Forsyth-Edwards Notation string
4. Use the FEN output for analysis, sharing, or importing into chess software

## Controls

- **Generate FEN**: Creates FEN notation from current board position
- **Reset to Starting Position**: Restores the standard chess starting position
- **Clear All Pieces**: Removes all pieces from the board

## FEN Notation

The generated FEN string includes:
- Piece placement (from rank 8 to rank 1)
- Active color (white)
- Castling availability (none)
- En passant target square (none)
- Halfmove clock (0)
- Fullmove number (1)

## Technical Details

- Pure HTML, CSS, and JavaScript (no dependencies)
- Uses Unicode chess piece symbols
- Responsive design with visual half-board indicators
- Drag-and-drop validation to enforce half-board restrictions
