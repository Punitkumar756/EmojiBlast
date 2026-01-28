# 🍬 Candy Crush Emoji

A fun and addictive match-3 puzzle game built with vanilla HTML, CSS, and JavaScript. Match colorful emoji candies to score points before time runs out!

![Game Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![HTML](https://img.shields.io/badge/HTML-E34F26?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## 🎮 Game Features

- **Classic Match-3 Gameplay**: Swap adjacent emojis to create matches of 3 or more
- **Special Power-Ups**:
  - 🚀 **Striped Horizontal** (4 in a row): Clears entire row
  - 🎯 **Striped Vertical** (4 in a column): Clears entire column
  - 💣 **Bomb** (5 matches): Clears surrounding 3x3 area
- **Time Challenge**: Complete as many matches as possible in 60 seconds
- **Move Limit**: Strategic gameplay with 20 moves per game
- **Score Tracking**: Local high score persistence using localStorage
- **Smooth Animations**: Fade effects and popup score indicators
- **Sound Effects**: Audio feedback for swaps and matches
- **Drag-and-Drop Interface**: Intuitive controls for swapping candies

## 🎯 How to Play

1. **Drag and Drop**: Click and drag an emoji to swap it with an adjacent emoji (up, down, left, or right)
2. **Match 3+**: Create horizontal or vertical matches of 3 or more identical emojis
3. **Create Power-Ups**: 
   - Match 4 emojis to create a striped candy
   - Match 5 emojis to create a bomb
4. **Score Points**: 
   - 3-match: 3 points
   - 4-match: 11 points (includes power-up bonus)
   - 5-match: 12 points (includes power-up bonus)
   - Power-up activation: 10-15 bonus points
5. **Beat the Clock**: Complete as many matches as possible within 60 seconds and 20 moves
6. **Beat Your High Score**: Try to surpass your previous best!

## 🍓 Available Emojis

The game features 6 colorful fruit emojis:
- 🍓 Strawberry
- 🍋 Lemon
- 🍊 Orange
- 🍏 Green Apple
- 🫐 Blueberry
- 🍇 Grape

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- No additional dependencies or installations required!

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/emoji-blast.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd EmojiBlast
   ```

3. **Open the game**:
   - Simply double-click `main.html` or
   - Right-click and select "Open with" your preferred browser

### Alternative: Run Locally with a Server

If you want to run it on a local server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

Then navigate to `http://localhost:8000/main.html` in your browser.

## 📂 Project Structure

```
EmojiBlast/
│
├── main.html          # Main game file (HTML, CSS, and JavaScript)
└── README.md          # Project documentation
```

## 🎨 Customization

### Changing Game Difficulty

You can modify the game parameters in [main.html](main.html):

```javascript
// Line 119-121: Adjust initial game settings
let moves = 20;        // Change number of moves
let timeLeft = 60;     // Change time limit in seconds
```

### Adding More Emojis

```javascript
// Line 123: Add or modify candy emojis
const candyIcons = ["🍓", "🍋", "🍊", "🍏", "🫐", "🍇", "🍉", "🍑"];
```

### Adjusting Grid Size

```javascript
// Line 115: Change grid dimensions (current: 8x8)
const width = 8;  // Change to 6 for 6x6 or 10 for 10x10
```

Update the CSS grid dimensions accordingly:
```css
/* Line 10-11: Update grid size */
.grid {
  width: 320px;   /* width * 40px */
  height: 320px;  /* height * 40px */
}
```

## 🛠️ Technical Details

### Technologies Used

- **HTML5**: Structure and layout
- **CSS3**: Styling, animations, and responsive design
- **Vanilla JavaScript**: Game logic, DOM manipulation, and event handling
- **LocalStorage API**: Persistent high score storage
- **Drag and Drop API**: Intuitive candy swapping mechanism

### Key Game Mechanics

- **Match Detection**: Algorithm checks for horizontal and vertical matches of 3, 4, and 5
- **Gravity System**: Emojis fall down to fill empty spaces after matches
- **Special Candy Generation**: Automatically created for 4-in-a-row or 5-match combinations
- **Cascade Effects**: New emojis drop from the top to create potential chain reactions
- **Game Loop**: Runs at 150ms intervals for smooth gameplay

## 🎯 Game Strategy Tips

1. **Plan Ahead**: Look for potential matches before making a move
2. **Create Power-Ups**: Prioritize creating 4 or 5 matches for powerful effects
3. **Use Power-Ups Wisely**: Save bombs and striped candies for maximum impact
4. **Cascade Combos**: Create matches that lead to chain reactions
5. **Manage Your Moves**: Use your 20 moves strategically
6. **Time Management**: Keep an eye on the timer - fast moves = more points!

## 📱 Browser Compatibility

| Browser | Supported | Version |
|---------|-----------|---------|
| Chrome  | ✅ | 90+ |
| Firefox | ✅ | 88+ |
| Safari  | ✅ | 14+ |
| Edge    | ✅ | 90+ |
| Opera   | ✅ | 76+ |

## 🐛 Known Issues

- Audio files are loaded from external CDN (requires internet connection)
- Game state is not saved between sessions (only high score is saved)

## 🔮 Future Enhancements

- [ ] Multiple difficulty levels (Easy, Medium, Hard)
- [ ] Additional power-ups and special candies
- [ ] Level progression system
- [ ] More animations and visual effects
- [ ] Mobile touch support
- [ ] Leaderboard system
- [ ] Background music toggle
- [ ] Pause/Resume functionality
- [ ] Hint system for possible moves
- [ ] Achievement system

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

PUNIT KUMAR


## 🙏 Acknowledgments

- Inspired by the classic Candy Crush game
- Sound effects from [SoundJay](https://www.soundjay.com/)
- Emoji graphics provided by Unicode Consortium

## 📊 Stats

![GitHub Stars](https://img.shields.io/github/stars/yourusername/emoji-blast?style=social)
![GitHub Forks](https://img.shields.io/github/forks/yourusername/emoji-blast?style=social)
![GitHub Watchers](https://img.shields.io/github/watchers/yourusername/emoji-blast?style=social)

---

**Enjoy the game! 🎮 Happy matching! 🍬**

*If you like this project, please give it a ⭐ on GitHub!*
