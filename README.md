# CHIRAG_SINGHAL 21BKT0181
# Turn-based Chess-like Game

## Objective
Develop a turn-based chess-like game with a server-client architecture, utilizing websockets for real-time communication and a web-based user interface.
# Game Rules
## Characters and Movement
There are three types of characters available:
 1. **Pawn:**
    Moves one block in any direction (Left, Right, Forward, or Backward).
    Move commands: L (Left), R (Right), F (Forward), B (Backward)
2. **Hero1:**
   Moves two blocks straight in any direction.
   Kills any opponent's character in its path.
   Move commands: L (Left), R (Right), F (Forward), B (Backward)
3. **Hero2:**
    Moves two blocks diagonally in any direction.
    Kills any opponent's character in its path.
    Move commands: FL (Forward-Left), FR (Forward-Right), BL (Backward-Left), BR (Backward-Right)
    All moves are relative to the player's perspective.    

## Screenshots of Testing
## Feature

- **Real-Time Multiplayer:** Players connect and play in real-time using WebSockets.
- **Character Types:** Three types of characters (Pawns, Hero1, Hero2) with unique movement and combat abilities.
- **Turn-Based Gameplay:** Players take turns to move their characters, with the goal of eliminating all opponent characters.
- **Game Over Conditions:** The game ends when one player eliminates all of the opponent's characters.

## Setup Instructions

### Server Setup

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/Chiragsinghal24/CHIRAG_SINGHAL_21BKT0181.git
    cd chess-game
    ```

2. **Install Dependencies:**

    Navigate to the server directory and install the required Node.js packages:

    ```bash
    cd server
    npm install
    ```

3. **Start the Server:**

    Run the server using:

    ```bash
    npm start
    ```

    The server will start on `http://localhost:8080`.

### Client Setup

1. **Navigate to the Client Directory:**

    ```bash
    cd ../client
    ```

2. **Install Dependencies:**

    Install the necessary packages:

    ```bash
    npm install
    ```

3. **Start the Client:**

    Run the React application:

    ```bash
    npm start
    ```

    The client will be available at `http://localhost:5173`.

## How to Play

1. Open the client in your web browser.
2. Enter your player identifier (`A` or `B`) when prompted.
3. Use the game board to select your characters and issue move commands.
4. The game displays the current state, including whose turn it is, and a history of moves.
5. The game ends when one player eliminates all of the opponent's characters. The winner is announced on the screen.
