# ♟️ Chess Game (SFML C++)

A fully interactive **Chess game** built using **C++ and SFML (Simple and Fast Multimedia Library)**.  
This project visually simulates a standard chess game with proper board setup, move logic, and player turns.  
It’s designed to demonstrate **game logic implementation**, **object-oriented design**, and **SFML rendering** skills.

---

## 🎥 Demo

Here’s a short demo of the game in action 👇  

![Chess Demo](assets/chess_demo.gif)


---

## 🧩 Features

- ✅ **8×8 chessboard** with alternating tile colors  
- ♔ **Fully functional chess pieces** (King, Queen, Rook, Bishop, Knight, Pawn)  
- 🔄 **Turn-based gameplay** (White & Black alternate turns)  
- 💡 **Move highlighting** for possible legal moves  
- 🏁 **Checkmate detection** and restart functionality  
- 🎨 Built entirely using **SFML for graphics & input handling**  

---

## 🏗️ Project Structure

| File / Folder | Description |
|:---------------|:------------|
| `board.h / board.cpp` | Handles board creation and rendering (8×8 grid). |
| `piece.h / piece.cpp` | Defines piece properties (type, player, position) and manages textures. |
| `chessgame.h / chessgame.cpp` | Main game controller that handles logic, turns, move validation, and drawing. |
| `pieceTextures.h / .cpp` | Loads and manages all chess piece textures. |
| `main.cpp` | Entry point — creates SFML window and runs the game loop. |
| `assets/` | Contains chess piece images, board textures, and fonts. |

---

## 🚀 Getting Started

### 🔧 Prerequisites
- C++17 or later
- SFML 2.5+ installed  
  ([SFML Installation Guide](https://www.sfml-dev.org/tutorials/2.5/))

### ⚙️ Build Instructions

**Using g++:**
```bash
g++ -IC:/path_to_sfml/include -LC:/path_to_sfml/lib src/*.cpp -o ChessGame -lsfml-graphics -lsfml-window -lsfml-system
```

**Using CMake (recommended):**
```bash
mkdir build
cd build
cmake ..
make
```

Run the game:
```bash
./ChessGame
```

---

## 🧠 How It Works

- The `Board` class creates 64 alternating-colored squares using `sf::RectangleShape`.
- Each `Piece` holds its type, player color, and current board position.
- The `ChessGame` class manages selection, movement, and rule enforcement.
- All rendering is done via SFML’s draw system using the `sf::Drawable` interface.

---

## 🖼️ Gameplay Screenshot

*(Optional — add if you have one)*  
![Chess Screenshot](assets/chess_screenshot.png)

---

## 💻 Technologies Used
- **C++17**
- **SFML 2.5+**
- **OOP Design**
- **Git & GitHub**

---

## 🔁 Future Improvements
- Add AI opponent using Minimax algorithm  
- Implement move history and undo functionality  
- Add timer and score system  
- Improve UI (menus, sounds, and themes)

---

## 👨‍💻 Author

**Anurag Wanwe**  
📧 anuwanwe1463@gmail.com    

---

## 🪪 License
This project is open-source under the [MIT License](LICENSE).
