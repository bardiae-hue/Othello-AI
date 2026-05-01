Othello AI
A fully playable Othello (Reversi) game engine built in vanilla JavaScript, featuring a Minimax AI opponent with game tree search. No frameworks, no dependencies — runs entirely in the browser.
Play Live

Features

Complete game engine — move validation, legal move generation, board state evaluation, and win detection
Minimax AI — searches the game tree to simulate and score opponent moves, making strategic decisions at each turn
Two modes — Player vs AI or Player vs Player
Clean UI — board renders via HTML/CSS, responsive and accessible


How the AI works
The AI uses the Minimax algorithm to evaluate future game states:

From the current board, all legal moves are generated
For each move, the resulting board state is scored recursively
The AI maximizes its own score while assuming the opponent plays optimally
The move with the highest minimax value is selected

Board evaluation considers piece count, corner control (highest value squares), and edge stability — corners are weighted heavily as they can never be flipped once captured.

Stack
LayerTechGame engineVanilla JavaScript (ES6+)UIHTML5, CSS3AIMinimax with static board evaluationHostingGitHub Pages

Run locally
No build step required. Clone the repo and open Main.html in a browser:
bashgit clone https://github.com/bardiae-hue/othello-ai.git
cd othello-ai
open Main.html
