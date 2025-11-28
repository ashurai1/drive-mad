# 🚗 Drive Mad

A thrilling browser-based racing game where you navigate challenging obstacle courses with physics-based vehicle controls. Test your driving skills across multiple levels filled with ramps, bridges, and treacherous terrain!

![Drive Mad Game](https://drive-mad-flame.vercel.app/)

## 🎮 About the Game

Drive Mad is an arcade-style racing game that challenges players to complete levels without crashing their vehicle. With realistic physics, dynamic obstacles, and increasingly difficult tracks, each level presents a unique challenge that will test your precision and timing.

### Features

- 🏁 **Multiple Levels**: Progress through challenging courses with increasing difficulty
- 🎯 **Physics-Based Gameplay**: Realistic vehicle physics for an authentic driving experience
- 🎨 **Clean UI**: Modern, intuitive interface with smooth animations
- 📱 **Responsive Design**: Play on desktop or mobile devices
- 🔊 **Interactive Elements**: Buttons, obstacles, and dynamic game elements
- 💾 **Progress Tracking**: Your progress is automatically saved

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Local web server (optional, for development)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/ashurai1/drive-mad.git
   cd drive-mad
   ```

2. **Open the game**
   - Simply open `Index.html` in your web browser, or
   - Use a local web server for better performance:
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Node.js (with http-server)
     npx http-server
     ```
   - Navigate to `http://localhost:8000` in your browser

### How to Play

1. **Controls**:
   - **Arrow Keys** or **WASD**: Control your vehicle
   - **Mouse/Touch**: Navigate menus and interact with UI elements

2. **Objective**:
   - Navigate through each level without crashing
   - Reach the finish line to unlock the next level
   - Master the physics to achieve the best times

3. **Tips**:
   - Balance speed with control
   - Watch out for steep ramps and gaps
   - Some obstacles require precise timing

## 📁 Project Structure

```
drive-mad/
├── Index.html          # Main game file with embedded WebAssembly loader
├── style.css           # Game styling and UI design
├── script.js           # External JavaScript (currently minimal)
├── webapp/             # Game assets and resources
│   ├── cover.jpg       # Game cover image
│   └── ...             # Additional game assets
└── README.md           # This file
```

## 🛠️ Technologies Used

- **HTML5**: Structure and canvas rendering
- **CSS3**: Styling and animations
- **JavaScript**: Game logic and interactivity
- **WebAssembly (WASM)**: High-performance game engine
- **Emscripten**: C/C++ to WebAssembly compilation

## 🎨 Customization

### Modifying Styles

Edit `style.css` to customize:
- Color schemes (currently uses blue gradient theme)
- Font styles (uses 'Baloo 2' font family)
- Button designs and layouts
- Canvas dimensions and responsive behavior

### Adding Levels

The game levels are stored in the WebAssembly data files. To add custom levels, you would need to:
1. Modify the source game data
2. Recompile using Emscripten
3. Update the data files

## 🌐 Deployment

### Deploy to Vercel

This project is configured for easy deployment to Vercel:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/ashurai1/drive-mad)

#### Quick Deploy Steps:

1. **Push to GitHub** (if not already done):
   ```bash
   git add .
   git commit -m "Prepare for deployment"
   git push origin main
   ```

2. **Deploy via Vercel Dashboard**:
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Click "Deploy" (no configuration needed - `vercel.json` handles everything)

3. **Or use Vercel CLI**:
   ```bash
   npm i -g vercel
   vercel
   ```

#### Important Notes:
- ✅ The project includes `vercel.json` with proper WebAssembly configuration
- ✅ CORS headers are pre-configured
- ✅ MIME types are set correctly for .wasm and .data files
- ⚠️ External resources are loaded from CDN - ensure they're accessible

**Troubleshooting**: If you encounter issues, see [DEPLOYMENT.md](DEPLOYMENT.md) for detailed troubleshooting guide.

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

### Contribution Ideas

- 🐛 Bug fixes and performance improvements
- 🎨 UI/UX enhancements
- 📱 Mobile optimization
- 🌐 Localization/translations
- 📝 Documentation improvements

## 📝 License

This project is available for educational and personal use. Please respect the original game creator's work.

## 👤 Author

**Ashwani Rai**
- GitHub: [@ashurai1](https://github.com/ashurai1)
- Email: raishwani151104@gmail.com

## 🙏 Acknowledgments

- Original game concept by **jaxkingofpugs**
- Built with Emscripten and WebAssembly technology
- Font: [Baloo 2](https://fonts.google.com/specimen/Baloo+2) by Google Fonts

## 🐛 Known Issues

- Some browsers may require user interaction before audio plays
- Performance may vary on older devices
- Best experienced on desktop browsers

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on [GitHub Issues](https://github.com/ashurai1/drive-mad/issues)
- Contact me at raishwani151104@gmail.com

## 🔮 Future Enhancements

- [ ] Leaderboard system
- [ ] More vehicle options
- [ ] Custom level editor
- [ ] Multiplayer mode
- [ ] Achievement system
- [ ] Sound effects and background music controls

---

**Enjoy the game! 🎮🏁**

*If you like this project, please consider giving it a ⭐ on GitHub!*
