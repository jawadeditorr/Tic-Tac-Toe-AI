🧠 Tic Tac Toe AI using Minimax (Python)

An intelligent Tic Tac Toe game built in Python using the Minimax algorithm. The AI plays optimally and will never lose, making it a perfect demonstration of basic game AI and decision-making.

📸 Screenshots

(Add your screenshots in a /screenshots folder and update paths below)

🟢 Game Start
   |   |  
-----------
   |   |  
-----------
   |   |  
🔵 Mid Game
 X | O | X
-----------
   | O |  
-----------
   |   | X
🔴 Game Result
 X | O | X
-----------
 O | O | O
-----------
 X | X | O

AI Wins 🎉
📁 Folder Structure
tic-tac-toe-minimax/
│
├── main.py              # Entry point to run the game
├── minimax.py          # Minimax algorithm implementation
├── game.py             # Game logic (board, moves, win check)
├── utils.py            # Helper functions (optional)
│
├── screenshots/        # Store game screenshots here
│   ├── start.png
│   ├── mid.png
│   └── result.png
│
└── README.md           # Project documentation
🚀 Features
🤖 Unbeatable AI using Minimax
👤 Human vs AI gameplay
🔁 Recursive decision-making
🧼 Clean and modular code
💻 Command-line interface
🧩 How the Minimax Algorithm Works

The Minimax algorithm is used to choose the best move by simulating all possible future game states.

Key Idea:
The AI (Maximizing player) tries to maximize its score
The Human (Minimizing player) tries to minimize AI's score
Scoring System:
AI win → +1
Human win → -1
Draw → 0
Flow:
Generate all possible moves
Recursively simulate each move
Assign scores based on outcomes
Choose the move with the best score
🧠 Code Explanation
main.py
Starts the game loop
Takes user input
Calls AI move function
Displays board
game.py

Handles core game logic:

Board representation (2D list)
Checking win conditions
Checking draw state
Making and undoing moves

Example:

def check_winner(board):
    # check rows, columns, diagonals
    pass
minimax.py

Implements the Minimax algorithm:

def minimax(board, depth, is_maximizing):
    if terminal_state:
        return score

    if is_maximizing:
        best_score = -inf
        for move in moves:
            score = minimax(new_board, depth+1, False)
            best_score = max(score, best_score)
        return best_score
    else:
        best_score = inf
        for move in moves:
            score = minimax(new_board, depth+1, True)
            best_score = min(score, best_score)
        return best_score
utils.py (optional)
Board printing
Input validation
UI helpers
▶️ How to Run
Clone the repository:
git clone https://github.com/your-username/tic-tac-toe-minimax.git
cd tic-tac-toe-minimax
Run the game:
python main.py
📌 Future Improvements
🎨 Add GUI using Tkinter or Pygame
⚡ Optimize using Alpha-Beta Pruning
🌐 Web version using Flask or React
👥 Multiplayer mode
📚 Learning Outcomes
Understanding recursion and game trees
Implementing Minimax from scratch
AI decision-making fundamentals
🤝 Contributing

Pull requests are welcome! Feel free to improve UI, optimize code, or add new features.

⭐ Support

If you found this helpful, give it a ⭐ on GitHub!