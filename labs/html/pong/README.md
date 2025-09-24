# PONG Game 🏓

A classic single-page PONG game implementation using HTML5 Canvas, CSS3, and JavaScript.

## 🎯 Goal

Create and play the classic PONG arcade game directly in your web browser. The first player to reach 5 points wins!

## ✍️ Programming Languages

- **HTML5** - Structure and Canvas element
- **CSS3** - Styling and animations
- **JavaScript** - Game logic and physics

## 💻 IDE and Tools

- Visual Studio Code
- [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) (recommended for testing)
- Any modern web browser

## 🎮 Game Features

- **Classic PONG gameplay** - Two paddles and a bouncing ball
- **Player vs Computer** - Challenge the AI opponent
- **Smooth animations** - 60fps gameplay using requestAnimationFrame
- **Realistic physics** - Ball physics with collision detection
- **Dynamic difficulty** - Ball speed increases slightly after each paddle hit
- **Score tracking** - First to 5 points wins
- **Responsive controls** - Arrow keys or WASD controls
- **Retro styling** - Classic green-on-black color scheme with glow effects

## 🕹️ How to Play

### Controls
- **Arrow Up (↑)** or **W** - Move paddle up
- **Arrow Down (↓)** or **S** - Move paddle down

### Game Rules
1. Use your paddle (left side) to hit the ball
2. Prevent the ball from reaching your side
3. Try to get the ball past the computer's paddle (right side)
4. Each time the ball goes off either side, a point is scored
5. First player to reach 5 points wins!

### Game Buttons
- **Start Game** - Begin a new game
- **Pause/Resume** - Pause or resume the current game
- **Reset** - Reset scores and start over

## 🚀 Getting Started

### Option 1: Direct File Opening
1. Navigate to the `labs/html/pong/` directory
2. Double-click on `index.html` to open it in your default browser

### Option 2: Using Live Server (Recommended)
1. Open the project in Visual Studio Code
2. Install the Live Server extension if you haven't already
3. Right-click on `index.html`
4. Select "Open with Live Server"
5. The game will open in your browser at `http://localhost:5500`

### Option 3: Local Web Server
```bash
# Navigate to the pong directory
cd labs/html/pong/

# Start a simple HTTP server (Python 3)
python -m http.server 8000

# Or using Node.js (if you have http-server installed)
npx http-server -p 8000

# Open your browser and go to:
# http://localhost:8000
```

## 🔧 Technical Implementation

### Game Architecture
- **Game Loop**: Uses `requestAnimationFrame` for smooth 60fps animation
- **Collision Detection**: Implements precise ball-to-paddle collision detection
- **AI Opponent**: Computer paddle with realistic movement and slight delay
- **Physics Engine**: Custom ball physics with speed increase and angle variation

### Key Components
- **Canvas Rendering**: HTML5 Canvas for real-time graphics
- **Input System**: Keyboard event handlers for player controls
- **State Management**: Game state tracking (running, paused, game over)
- **Responsive Design**: Scales well on different screen sizes

### Performance Features
- Efficient rendering using Canvas 2D API
- Optimized collision detection algorithms
- Memory-conscious animation loop management

## 🎨 Visual Features

- **Retro Aesthetic**: Classic arcade game styling
- **Glowing Effects**: CSS and Canvas shadow effects
- **Smooth Animations**: Fluid paddle and ball movement
- **Dynamic UI**: Real-time score updates and game state changes
- **Responsive Layout**: Centers game on various screen sizes

## 🔮 Potential Enhancements

Feel free to extend the game with:
- Sound effects and background music
- Power-ups and special abilities
- Multiplayer support (two human players)
- Different difficulty levels
- Tournament mode
- Mobile touch controls
- Particle effects for collisions
- Different ball types and behaviors

## 🏗️ Code Structure

```
index.html
├── HTML Structure
│   ├── Game canvas
│   ├── Score display
│   ├── Control buttons
│   └── Instructions
├── CSS Styling
│   ├── Retro theme
│   ├── Layout and positioning
│   └── Visual effects
└── JavaScript Logic
    ├── Game state management
    ├── Physics engine
    ├── Collision detection
    ├── AI opponent
    ├── Input handling
    └── Rendering system
```

## 🌟 Learning Objectives

This project demonstrates:
- HTML5 Canvas manipulation and drawing
- Game loop implementation with requestAnimationFrame
- Physics simulation and collision detection
- Event handling for user input
- CSS styling for game interfaces
- JavaScript object-oriented programming concepts
- Real-time game state management

---

**Enjoy playing PONG! 🏓**

*This implementation showcases how GitHub Copilot can assist in creating complete, functional games with modern web technologies.*