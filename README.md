# PONG - Two Player Classic

A modern, mobile-optimized Progressive Web App (PWA) implementation of the classic Pong game.

![PONG Game](icon-512.png)

## Features

- 🎮 **Two-player gameplay** - Play with a friend on the same device
- 📱 **Mobile-optimized** - Touch controls with split-screen for each player
- 🖥️ **Desktop support** - Mouse and keyboard controls
- 🌐 **Progressive Web App** - Install on your phone like a native app
- 🔌 **Offline capable** - Play even without internet connection
- 🎨 **Modern design** - Neon aesthetics with smooth animations

## Play Now

**[Play Online](https://joeykills.github.io/pong/pong.html)**

Or install as an app on your iPhone:
1. Open the link above in Safari
2. Tap Share → "Add to Home Screen"
3. Tap "Add"

## Controls

### Mobile (Touch)
- **Left half of screen** - Controls Player 1 (blue paddle)
- **Right half of screen** - Controls Player 2 (pink paddle)
- Drag your finger up/down to move your paddle

### Desktop
- **Player 1**: W/S keys or mouse (left side)
- **Player 2**: Arrow Up/Down keys or mouse (right side)
- **Spacebar** or **Click** - Start/continue game

## Gameplay

- First player to **7 points** wins
- Ball speed increases slightly with each paddle hit
- Particle effects on collisions and scoring

## Installation

### As a Progressive Web App

See [PWA-INSTALL.md](PWA-INSTALL.md) for detailed installation instructions.

### Run Locally

```bash
# Clone the repository
git clone https://github.com/JoeySkills/pong.git
cd pong

# Start a local server
python3 -m http.server 8080

# Open in browser
open http://localhost:8080/pong.html
```

## Tech Stack

- Pure HTML5 Canvas - No frameworks
- Service Workers for offline functionality
- Progressive Web App manifest
- Responsive design with dynamic scaling

## Files

- `pong.html` - Main game file (self-contained)
- `manifest.json` - PWA configuration
- `service-worker.js` - Offline caching
- `icon-192.png`, `icon-512.png` - App icons

## License

MIT License - Feel free to use and modify!

## Credits

Built with Claude Code
