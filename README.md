# Snake Game

## Overview

A modern implementation of the classic Snake game built with React and Vite. Control a snake as it moves around the board, eating food to grow longer while avoiding collisions with walls and itself.

## Features

- **Responsive game board**: 15x15 grid with smooth gameplay
- **Classic snake mechanics**: Move in four directions using arrow keys
- **Food consumption**: Grow your snake with each food item eaten
- **Score tracking**: Keep track of your current score
- **Special food items**: Purple food that reverses your snake's direction
- **Game reset**: Automatic restart on game over

## Technologies Used

- [React](https://reactjs.org/) - UI library
- [Vite](https://vitejs.dev/) - Build tool and development server
- Custom CSS for styling
- JavaScript ES6+ features
- Custom LinkedList implementation for snake movement

## Installation and Setup

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Steps to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/snake-game.git
   cd snake-game
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. Open your browser and navigate to `http://localhost:5173`

## How to Play

- **Start**: The game begins automatically when the page loads
- **Controls**: Use arrow keys to change direction
  - ↑ (Up Arrow): Move Up
  - → (Right Arrow): Move Right
  - ↓ (Down Arrow): Move Down
  - ← (Left Arrow): Move Left
- **Objective**: Eat the red food items to grow your snake and increase your score
- **Special Items**: Purple food will reverse your snake's direction when eaten
- **Game Over**: Occurs when your snake hits a wall or itself. The game automatically restarts.

## Game Mechanics

### Snake Implementation

The game uses a linked list data structure to represent the snake, which allows for efficient movement and growth operations:

- The snake moves by adding a new node at the head and removing the tail
- When food is consumed, the snake grows by adding a node without removing the tail
- The special purple food triggers a direction reversal, implemented by reversing the linked list

### Food Generation

- Regular food (red) appears randomly on the board
- Special direction-reversing food (purple) has a 30% chance of appearing instead of regular food
- Food never appears on cells already occupied by the snake

## Project Structure

```
snake-game/
├── public/
├── src/
│   ├── Board/
│   │   ├── Board.jsx     # Main game component with game logic
│   │   └── Board.css     # Styling for the game board
│   ├── lib/
│   │   └── utils.js      # Utility functions (intervals, randomization, etc.)
│   ├── App.jsx           # Root component
│   ├── App.css           # Global styles
│   ├── index.css         # Base styles
│   └── main.jsx          # Entry point
├── index.html            # HTML template
├── package.json          # Project dependencies and scripts
└── vite.config.js        # Vite configuration
```

## Future Enhancements

- Add a proper start/restart game UI
- Implement difficulty levels (speed options)
- Add high score tracking with local storage
- Add mobile support with touch controls
- Add sound effects and music
- Create different themes/skins for the snake and board

## Contributing

Contributions are welcome! If you'd like to contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

---

<div align="center">
  Made with ❤️ by [Gaurav Chaudhary ]
</div>

