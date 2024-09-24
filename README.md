## Flask Application Design for Tetris Clone

### HTML Files

**tetris.html:** The primary HTML file that displays the game board, handles player input, and renders the game state. It includes:

- A canvas element to represent the game board.
- Input listeners for keystrokes to control the falling tetrominoes.
- JavaScript functions to update the game state, check for collisions, and handle game logic.

**index.html:** The main landing page for the application, providing a link to the game page and other relevant information.

### Routes

**app.py** defines the following routes:

**`/tetris` (GET):** Renders the `tetris.html` file, serving as the entry point for the game.

**`/reset` (POST):** Receives a request to reset the game state, clearing the canvas and initiating a new game.

**`/move` (POST):** Receives a request to move the current tetromino in a specified direction (left, right, or down). It updates the game state accordingly and responds with the updated state.

**`/rotate` (POST):** Receives a request to rotate the current tetromino clockwise or counterclockwise. It updates the game state and responds with the updated state.

**`/score` (POST):** Receives a request to update the game score based on completed lines and level progression. It updates the game state and responds with the updated score.