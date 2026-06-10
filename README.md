2048 Game - Java Edition

This is a complete implementation of the classic 2048 puzzle game built with Java Swing. To run the game, compile all Java files with javac *.java and then execute with java Main.

The game is played on a 4x4 grid. Use the arrow keys to slide all tiles in the chosen direction. When two tiles with the same number collide, they merge into one tile with double the value, and that value is added to your score. After each move, a new tile with value 2 or 4 appears in a random empty space. The goal is to create a tile with the value 2048.

The controls include arrow keys for manual movement, the A key for auto-move where the AI analyzes all possible moves and selects the most efficient one, the R key for a random valid move, the Z key to undo your last move, and the ESC key to reset the game completely.

The AI system works by evaluating all four possible directions and ranking them using a priority queue. Each move is scored based on how many empty tiles it creates and the total score gained from merges. The auto-move then executes the highest ranked move automatically.

The game detects when no more moves are possible and displays a loss message, and when the 2048 tile is created it shows a win message with your final score. The undo system uses a stack to save previous board states and scores, allowing you to rollback your moves at any time.

This project requires Java 8 or higher and uses the Swing framework for all graphical components following the Model-View-Controller design pattern. The source code includes five main classes: Main for application entry point, Controller for keyboard input handling, Model for all game logic and AI algorithms, View for rendering the game board, Tile for individual tile properties and colors, and MoveEfficiency for comparing move quality.



Features
✅ Full 2048 gameplay

✅ Smart AI auto-move

✅ Undo/rollback system

✅ Score tracking

✅ Win/loss detection

✅ Color-coded tiles
