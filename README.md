# MicroArcade 150 - Tic-Tac-Toe

A minimal, high-performance Tic-Tac-Toe game with AI opponent and difficulty levels, built as a single HTML file under 150 lines of code.

## 🎯 Features

- **Three Difficulty Levels**: Easy (random moves), Medium (70% strategic), Hard (full strategic AI)
- **Score Tracking**: Persistent win/loss tracking with localStorage
- **Intelligent AI Opponent**: Strategic AI that blocks your moves and takes winning opportunities
- **Enhanced UI**: Glassmorphism design with smooth animations, pulsing effects, and modern styling
- **Game State Persistence**: Automatically saves your game state and difficulty preference
- **Instant Loading**: Optimized for sub-2-second load times
- **Zero Dependencies**: Fully self-contained, no external libraries or assets

## 🚀 Quick Start

Simply open `microarcade.html` in any modern web browser. No installation or server required.

## 🎮 How to Play

1. **Select Difficulty**: Choose Easy, Medium, or Hard before starting
2. You play as **X**, AI plays as **O**
3. Click any empty cell on the 3×3 grid to make your move
4. AI will automatically respond after your move
5. Win by getting three in a row (horizontal, vertical, or diagonal)
6. Your score is tracked and saved automatically
7. Click "🔄 Reset Game" to start a new match

## 🏗️ Technical Architecture

### Code Structure

- **HTML**: Minimal semantic structure with game container
- **CSS**: Inline styles for board grid, cells, and responsive layout
- **JavaScript**: Game logic, AI algorithm, win detection, and state management

### AI Difficulty Levels

**Easy Mode**: Random moves - AI makes completely random valid moves (great for beginners)

**Medium Mode**: Mixed strategy - 70% of the time uses optimal strategy, 30% random moves (balanced challenge)

**Hard Mode**: Full strategic AI using a three-tier decision system:
1. **Win Move**: Takes immediate winning opportunity
2. **Block Move**: Prevents player from winning on next turn
3. **Optimal Placement**: Chooses center, then corners, then remaining cells

### State Management

- Game state (board, current player, active status, difficulty) is saved to localStorage after each move
- Score tracking persists across sessions
- On page refresh, the game automatically restores to the last state and difficulty
- State is cleared when a game ends (win/draw)

## 📊 Performance

- **File Size**: ~2.5 KB (minimal HTML/CSS/JS)
- **Load Time**: < 1 second on modern browsers
- **Interactivity**: Immediate response (< 50ms click latency)
- **Lines of Code**: ~109 lines (excluding comments and whitespace)

## 🎨 Design Philosophy

- **Minimalism**: Every line serves a purpose
- **Performance**: Fast rendering, efficient algorithms
- **UX**: Clear visual feedback, smooth transitions
- **Accessibility**: Keyboard-friendly, clear status messages

## 🛠️ Browser Compatibility

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 Code Quality

- Clean, readable code structure
- Efficient algorithms (O(1) win checking, smart AI)
- No external dependencies
- Self-contained and portable

## 🔧 Customization

To modify the game:

- **AI Difficulty**: Adjust `findBestMove()` function logic
- **Styling**: Modify CSS variables in `<style>` section
- **Board Size**: Update grid template and win conditions (requires more code)
