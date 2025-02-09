# Tic-Tac-Toe
Components:
Game: I use this as my main container—it holds the overall state and history of the moves.

Board: This renders the 3×3 grid and contains the logic for handling clicks.

Square: Each square is a simple component that just displays its value and notifies me when it's clicked.

Props:
I pass data (like the current board array) and functions (like the click handler) down from Game to Board and from Board to Square. This lets me keep each component focused on its job while still communicating with each other.

State:
I keep all the mutable data (like the move history and current board configuration) in the Game component. When I click a Square, the state updates in Game, which then flows down as props, causing my UI to refresh with the new move.
