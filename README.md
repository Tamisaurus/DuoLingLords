# BroTito's RNG - Night City

A fast-paced top-down roguelike shooter inspired by Brotato, featuring potato characters fighting through waves of enemies in a neon-lit cyberpunk world.

## Description

BroTito's RNG is a browser-based survival shooter where you play as a potato warrior fighting endless waves of enemies. Choose from different potato characters, unlock powerful weapons, and upgrade your stats to survive as long as possible. The game features:

- 5 unique playable characters with different stats and playstyles
- Campaign mode with 25 stages across 5 themed chapters
- Endless mode for high score chasing
- 7 different weapons including pistols, SMGs, snipers, orbital saws, tesla coils, mines, and turrets
- Progressive difficulty scaling with boss waves every 10 rounds
- Persistent save system using browser localStorage
- Full audio system with synthesized sound effects
- Mobile touch controls support

## Setup Instructions

### Quick Start

1. Download the HTML file
2. Open it in any modern web browser (Chrome, Firefox, Edge, Safari)
3. Click "CLICK TO CONTINUE" on the title screen
4. Start playing!

### Running Locally

No installation required! This is a standalone HTML file with all code embedded.

**Option 1: Double-click the file**
- Simply double-click the `.html` file to open it in your default browser

**Option 2: Run with a local server (recommended for development)**
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js http-server
npx http-server

# Then navigate to http://localhost:8000 in your browser
```

### Browser Requirements

- Modern browser with HTML5 Canvas support
- JavaScript enabled
- Web Audio API support (for sound effects)
- localStorage enabled (for save data)

Recommended browsers:
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## Controls

### Desktop Controls

**Movement:**
- `W` - Move Up
- `A` - Move Left
- `S` - Move Down
- `D` - Move Right

**Combat:**
- `Mouse Movement` - Aim
- `Left Mouse Button (Hold)` - Shoot (for manual weapons)
- Automatic weapons fire on their own cooldown

**Menu Navigation:**
- `ESC` - Pause/Resume Game
- `Mouse Click` - Select menu options and upgrades

### Mobile Controls

The game automatically detects mobile devices and shows touch controls:

**Movement:**
- `Virtual Joystick (Bottom Left)` - Move in any direction
- Character aims in the direction of joystick movement

**Combat:**
- `Fire Button (Bottom Right)` - Hold to shoot
- Automatic weapons still fire on their own

### UI Controls

**Main Hub:**
- `CAMPAIGN` - Play through 25 story stages
- `ENDLESS` - Survive infinite waves for high scores
- `CHARACTERS` - Select and unlock different potato warriors
- `Settings (Gear Icon)` - Toggle sound effects

**In-Game:**
- Top Left: HP bar, wave counter, stage info
- Top Right: Level, XP bar, score
- Left Panel: Current stats (damage, fire rate, speed, armor, vampirism)
- Bottom Center: Weapon cooldown indicators

**Level Up Screen:**
- Click any of the 4 upgrade cards to select it
- Upgrades include weapon improvements, new weapons, and stat boosts

## Game Modes

### Campaign Mode
- 5 Chapters with 5 stages each (25 total)
- Each stage has 5 waves
- Boss fight on the final wave of each stage
- Different environmental themes per chapter
- Progress is saved automatically
- Unlock new characters by reaching higher stages

### Endless Mode
- Infinite waves of enemies
- Boss every 10 waves
- Difficulty increases continuously
- Score-based progression
- High score tracking
- Perfect for testing builds and chasing leaderboards

## Characters

Unlock characters by reaching specific campaign stages:

1. **Classic** (Stage 1) - Well-rounded starter character
2. **Speedy** (Stage 3) - +Speed, -HP
3. **Chunky** (Stage 6) - +HP/Armor, -Speed
4. **Ghost** (Stage 11) - +Vampirism, -HP
5. **Demon** (Stage 16) - +40% Damage, No Regen

## Weapons

- **Pistol** - Balanced starter weapon
- **SMG** - High fire rate, lower damage
- **Sniper** - Slow but powerful piercing shots
- **Orbital Saws** - Melee weapons that orbit the player
- **Tesla Coil** - Chain lightning that hits multiple enemies
- **Mines** - Deployable explosives triggered by proximity
- **Turrets** - Automated gun emplacements

## Tips

1. **Movement is survival** - Keep moving to avoid enemy swarms
2. **Balance weapons** - Mix automatic and manual weapons
3. **Upgrade strategically** - Sometimes adding a new weapon is better than upgrading existing ones
4. **Use the environment** - Kite enemies around obstacles
5. **Watch cooldowns** - Time your manual weapon usage with ability cooldowns
6. **Collect gems quickly** - Level up faster by grabbing XP gems
7. **Health management** - Pick up medkits and use vampirism effectively
8. **Boss waves** - Save powerful abilities for boss encounters

## Save System

The game automatically saves:
- Maximum stage reached in campaign
- Selected character
- Sound settings
- Endless mode high score

Save data is stored in browser localStorage and persists between sessions.

**To reset progress:**
1. Open browser Developer Tools (F12)
2. Go to Console tab
3. Type: `localStorage.removeItem('brotito_save')`
4. Refresh the page

## Credits

Game Design & Programming: Original HTML5 implementation
Inspired by: Brotato by Blobfish
Font: Righteous & Teko (Google Fonts)
Audio: Web Audio API synthesized sounds

## Technical Notes

- Pure HTML5/CSS3/JavaScript - no frameworks required
- Canvas-based rendering
- Procedural audio generation using Web Audio API
- Responsive design supports desktop and mobile
- Object-oriented game architecture
- Delta-time based physics for consistent performance

## Browser Compatibility

Tested and working on:
- Chrome/Edge (Chromium) - Full support
- Firefox - Full support
- Safari (Desktop/iOS) - Full support
- Chrome Mobile (Android) - Full support with touch controls

## Known Issues

- Touch controls may need calibration on some tablet sizes
- Audio may require user interaction to start on iOS Safari
- Very old browsers (pre-2020) may have performance issues

## License

This is a demonstration project. Feel free to modify and learn from the code.

---

**Enjoy the game and survive the night city!**