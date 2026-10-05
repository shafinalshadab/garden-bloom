# 🌸 Garden Bloom

A delightful, interactive flower-growing game where you nurture beautiful flowers by clicking to make them bloom.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen.svg)
![HTML5](https://img.shields.io/badge/HTML5-Ready-orange.svg)

## 🎮 About the Game

**Garden Bloom** is a relaxing, adorable clicker game where you:

- 🌹 **Plant flowers** from a variety of beautiful types
- 🖱️ **Click to grow** - Each flower needs a different number of clicks to bloom
- 🌺 **Collect petals** - Blooming flowers reward you with petals
- 📈 **Level up** - Reach new levels as you collect more petals
- 💾 **Auto-save** - Your garden is automatically saved to your browser
- 🎨 **Enjoy beautiful visuals** - Cute emojis, smooth animations, and gradient designs

## 🌼 Features

✨ **8 Unique Flower Types**
- Rose (🌹) - 5 clicks
- Tulip (🌷) - 4 clicks
- Sunflower (🌻) - 6 clicks
- Cherry Blossom (🌸) - 4 clicks
- Hibiscus (🌺) - 5 clicks
- Daisy (🼼) - 3 clicks
- Lotus (🪷) - 7 clicks
- Orchid (🦋) - 8 clicks

🎨 **Beautiful Design Elements**
- Rainbow gradient backgrounds
- Smooth bloom animations
- Sparkle particle effects on clicks
- Achievement popups and notifications
- Responsive design for all devices
- Hover effects and smooth transitions

💾 **Game Mechanics**
- Grow up to 6 flowers at once
- Random petal rewards (3-8 per bloom)
- Progressive level system
- Progress bars for each flower
- Message feedback system
- One-click garden reset

## 🚀 Quick Start

### Installation
Simply download or clone the repository and open the HTML file in any modern web browser:

```bash
git clone https://github.com/yourusername/garden-bloom.git
cd garden-bloom
open garden_bloom_game.html
```

### No Dependencies
Garden Bloom is a **single HTML file** with no external dependencies. Everything is self-contained:
- Pure HTML5
- Vanilla CSS3
- Vanilla JavaScript (ES6)

## 📁 File Structure

garden-bloom/
├── garden_bloom_game.html # Main game file (all-in-one)
├── FILE_STRUCTURE.md # Detailed documentation
├── README.md # This file
└── LICENSE # MIT License


## 🎯 How to Play

1. **Click "Plant New Flower"** to add a flower to your garden
2. **Click the flower emoji** to make it grow
3. **Watch the progress bar** fill up as you click
4. **Celebrate the bloom!** When a flower is fully grown, it blooms and you earn petals
5. **Level up** by collecting enough petals
6. **Expand your garden** up to 6 flowers at once
7. **Remove flowers** to make room for new ones

### Game Statistics
- **Clicks:** Total number of clicks made
- **Petals:** Total petals collected from all blooms
- **Level:** Your current level (increases every 20 petals)

## 🎨 Customization

### Add New Flower Types
Edit the `flowerTypes` array in the JavaScript section:

```javascript
{
  name: 'Your Flower',
  emoji: '🌼',
  clicksNeeded: 5
}
```

### Change Colors
Modify the gradient definitions in the CSS `<style>` section:

```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Adjust Game Difficulty
Change the `clicksNeeded` values for each flower type to make the game easier or harder.

## 💾 Data Persistence

Your garden is automatically saved to your browser's `localStorage`:
- Game state persists across page refreshes
- Click "New Garden" to reset everything
- Data is stored locally (no server required)

## 🛠️ Technical Details

### Browser Support
- ✅ Chrome/Chromium (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

### Performance
- **File Size:** ~18KB (unminified) / ~12KB (minified)
- **Load Time:** Instant
- **Memory Usage:** <2MB during gameplay
- **No external requests** - Fully offline capable

### Technologies Used
- **HTML5** - Semantic structure
- **CSS3** - Gradients, animations, flexbox, grid
- **JavaScript ES6** - Game logic, state management, DOM manipulation

## 🎓 Code Architecture

### Main Class: `GardenGame`
```javascript
class GardenGame {
  constructor()           // Initialize game
  plantFlower()          // Add new flower
  clickFlower(id)        // Increment progress
  bloomFlower(flower)    // Handle bloom event
  removeFlower(id)       // Delete flower
  reset()                // Clear garden
  save()                 // Persist to localStorage
  load()                 // Restore from localStorage
  showMessage(text)      // Display feedback
  showAchievement()      // Show popup
  render()               // Update UI
}
```

### Game State Structure
```javascript
{
  flowers: [
    {
      id: timestamp,
      type: FlowerType,
      progress: number,
      isGrowing: boolean
    }
  ],
  stats: {
    clicks: number,
    petals: number,
    level: number
  }
}
```

## 📊 Animations & Effects

- **Bloom Animation** - Flowers scale from 0 to 1 with smooth easing
- **Sparkle Particles** - ✨ effects fade out and float upward
- **Hover Effects** - Flower plots lift up slightly on hover
- **Achievement Popup** - Pop-in animation for level-ups and rewards
- **Smooth Transitions** - All interactions use CSS transitions

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Add new flower types
- Improve animations
- Enhance mobile experience

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Created By

**Shafin** - Game Designer & Developer

## 🙏 Acknowledgments

- Inspired by cozy, relaxing clicker games
- Beautiful emoji flowers from Unicode
- CSS gradient inspiration from modern web design trends

## 🌟 Features Coming Soon (Potential)

- 🎵 Background music and sound effects
- 🏆 Achievement badges and medals
- 🎁 Special events and seasonal flowers
- 👥 Multiplayer garden sharing
- 🎨 Flower color customization
- 📊 Stats and gameplay analytics
- 🌍 Garden themes and backgrounds

## 📸 Screenshots

### Desktop View
Beautiful gradient background with responsive garden layout, colorful stat cards, and interactive flower plots.

### Mobile View
Optimized 2-column grid layout perfect for phones and tablets with touch-friendly button sizes.

## 🐛 Known Issues

- None currently reported

## 💬 Feedback & Support

Have suggestions or found a bug? Open an issue on GitHub or reach out to the developer!

## 📱 Mobile Experience

Garden Bloom is fully responsive and optimized for mobile devices:
- Touch-friendly button sizes
- Responsive grid layout
- Optimized animations for mobile performance
- Works offline once loaded

---

**Happy Gardening! 🌸🌺🌻**
