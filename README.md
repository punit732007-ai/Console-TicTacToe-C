🎮 Console Tic-Tac-Toe in C

A robust, interactive 2-player Command Line Interface (CLI) Tic-Tac-Toe game written in pure C. This project demonstrates foundational software engineering concepts including structured data encapsulation, modular design, real-time state management, and strict input validation.

📥 Download & Play (No Setup Required)

Want to just play the game? You don't need to compile any code.
👉 Download the Playable Demo v1.0.0 (.exe)

Note: Windows may show a "Windows protected your PC" warning because the file is an unassigned .exe. Click "More info" and "Run anyway" to launch the game.

✨ Key Features

Interactive CLI Graphics: Clean, dynamically updated terminal rendering.

Real-time State Tracking: Displays the current turn, complete move history, and updates the board live.

Persistent Score Tracking: Maintains a running score across multiple rounds for competitive sessions.

Bulletproof Input Validation: Prevents invalid keystrokes, out-of-bounds moves, and overwriting existing grid coordinates using <ctype.h>.

Dynamic Symbol Selection: Players can dynamically choose their symbols (X or O) at the start of the session.

🛠️ Technical Architecture

This application utilizes a centralized struct to act as the single source of truth for the game state, ensuring data consistency across all functions:

typedef struct {
    char board[3][3];     // The 3x3 game grid
    char p1Symbol, p2Symbol;
    int p1Score, p2Score; // Running totals
    int currentPlayer;    // Tracks active turn
    int gameMoves[9];     // Historical move tracking
    int moveCount;        // Total turns played
    int gameRunning;      // Execution flag
} GameState;


Language: C

Design Pattern: Modular file splitting (main.c for execution, tictactoe.h for logic implementation).

🚀 Getting Started

Prerequisites

A Windows PC (This project currently utilizes <conio.h> and system("cls"), which are optimized for Windows command prompt environments).

Installation & Execution

Download the Release: Go to the Releases page and download the .zip file (or direct .exe) for the latest demo version.

Extract the Files: If you downloaded the .zip file, extract it to your computer and open the newly extracted folder.

Run the Game: Double-click the main .exe file to launch the application.

Bypass Windows Warning: A blue screen may appear saying "Windows protected your PC". This is completely normal for newly created software (similar to installing a downloaded APK on an Android phone).

Click on "More info".

Click "Run anyway" to start the game!

👨‍💻 Author

Punit

GitHub: @punit732007-ai

[LinkedIn](https://www.linkedin.com/in/punit-bhyan-a01492381?utm_source=share_via&utm_content=profile&utm_medium=member_android)
