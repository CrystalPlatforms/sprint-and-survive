# 🎮 Sprint'n Survive!

A fast, retro-style runner built with HTML5 Canvas and Vite. Dodge red obstacles, collect points and survive the whole run — the finish line is 1000 meters away!

## 📝 Description

Sprint'n Survive is a dynamic side-scrolling platform game. You control a blue runner who sprints automatically through a dark, neon-lit level full of red obstacles. Jump over them or slide past them vertically, score points for every obstacle you dodge, and hold out until you reach the finish line.

## 🎯 Gameplay

- **The run is 1000 m long** — the distance counter drops while you run. Reach `0 m` to win.
- **Obstacles** are red pillars rising from the ground with random heights (50–150 px). They scroll from right to left and keep spawning as you go.
- **Scoring:** every obstacle that leaves the screen unhit gives you **+10 points**.
- **One touch = game over** — but your score is saved and shown on the game-over screen.
- **Physics:** the runner is affected by gravity. SPACE makes you jump, and while airborne you can fine-tune your height with the ↑/↓ arrows.

### 🕹️ Screens

| Screen | What happens there |
|---|---|
| **Menu** | Start the game, open "How to play", switch language (PL / EN / CN) |
| **Game** | The run itself — points and distance-to-finish shown above the canvas |
| **How to play** | Short instructions in the selected language |
| **Game over** | Your score + "Play again" / "Back to menu" |
| **Victory** | Congratulations screen with your final score |

## 🎮 How to Play

1. **Controls:**
   - `SPACE` — jump
   - `↑` `↓` — move up/down (also in mid-air)
   - Mouse — menu buttons

2. **Objective:**
   - Avoid the red obstacles
   - Collect +10 points for each dodged obstacle
   - Survive all 1000 m and reach the finish line!

## 🌍 Languages

The UI is fully translated into **Polish 🇵🇱, English 🇬🇧 and Chinese 🇨🇳**. You can switch the language at any time from the main menu — points labels, buttons and instructions change instantly.

## 🎵 Sounds

| File | When it plays |
|---|---|
| `sounds/lobby-game-retro.mp3` | Loops in the menu |
| `sounds/start-game-retro.mp3` | When a run starts |
| `sounds/win-retro.mp3` | When you reach the finish line |
| `sounds/fail-retro.mp3` | When you hit an obstacle |

> 💡 Browsers block audio until your first click or keypress — that's normal. Click anything once and the menu music will kick in.

## 🎨 Graphics

- Modern, minimalist design
- Gradient and glow effects (canvas shadows)
- Rounded corners on the player, obstacles and buttons
- Hover states and pointer cursor on menu buttons
- Responsive layout (canvas scales down on small screens)

## 🚀 Getting Started

### Requirements

- [Node.js](https://nodejs.org/) **20.19+** (LTS recommended) — includes `npm`

### Installation & running

```bash
npm install    # downloads dependencies (Vite)
npm run dev    # starts the dev server → http://localhost:5173
```

The dev server has hot reload — every change in `src/` appears in the browser instantly, no refresh needed.

### Production build

```bash
npm run build     # builds optimized files into dist/
npm run preview   # serves the build locally to check it
```

## 📁 Project Structure

```
sprint-and-survive/
├── index.html          # game page (canvas + audio elements)
├── package.json        # npm config and Vite scripts
├── public/             # static files served as-is
│   ├── favicon.ico
│   └── sounds/         # music and sound effects
│       ├── fail-retro.mp3
│       ├── lobby-game-retro.mp3
│       ├── start-game-retro.mp3
│       └── win-retro.mp3
└── src/
    ├── main.js         # all game logic (rendering, physics, menus, i18n)
    └── style.css       # page styling and layout
```

## 🛠️ Technologies

- HTML5 Canvas
- Vanilla JavaScript (ES modules)
- [Vite](https://vite.dev/) — dev server & build tool
- CSS3
- [Comic Neue](https://fonts.google.com/specimen/Comic+Neue) (Google Fonts)

## 🔜 Planned Features

- [ ] Power-up system
- [ ] Upgrades shop
- [ ] New levels
- [ ] Achievement system
- [ ] Multiplayer mode
- [ ] Character customization

## 🤝 Contributing

We welcome suggestions and pull requests! If you have an idea to improve the game, don't hesitate to propose it.

## 📝 License

This project is licensed under the MIT License.

## 👥 Authors

- Game Developer: [MrCrystal2](https://github.com/MrCrystal2)
