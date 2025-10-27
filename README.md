# Black Hole Simulation in Three.js

A stunning, interactive 3D black hole visualization built with Three.js, featuring realistic physics and beautiful visual effects.

🔗 **Live Demo:** https://julienokumu.github.io/vibed-claude-blackhole-sim/

![Black Hole Simulation](https://img.shields.io/badge/three.js-0.160.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## 🌌 Features

- **Event Horizon**: The black hole's point of no return, rendered as a perfect sphere
- **Photon Sphere**: A wireframe sphere showing where light can orbit the black hole
- **Animated Accretion Disk**: 5,000 particles orbiting the black hole with realistic physics
  - Inner particles orbit faster (following Kepler's laws)
  - Color gradient from hot white/orange (inner) to cooler red (outer)
- **Gravitational Lensing Effect**: Pulsing ring effect demonstrating light bending
- **Starfield Background**: 10,000 stars creating a deep space atmosphere
- **Interactive Controls**:
  - Mouse drag to rotate the view
  - Scroll to zoom in/out
  - Smooth camera damping for fluid movement

## 🤖 How This Was Built with Claude Code

This entire project was created through a conversation with Claude Code, my trusty AI coding buddy powered by [Giga AI Free](https://free.gigamind.dev/).

### The Development Process

**Step 1: The Initial Request**
I simply said: *"let's simulate a black hole in three.js"*

**Step 2: Claude Code Took Over**
Claude immediately:
- Created a comprehensive todo list to track the implementation
- Set up the complete HTML file with Three.js imports
- Implemented the scene, camera, and controls
- Built all the physics and visual effects

**Step 3: The Features Claude Implemented**
Without me having to specify details, Claude Code created:
- A realistic event horizon sphere
- An accretion disk with 5,000 particles that orbit with physically accurate speeds
- Color gradients based on temperature (hotter near the center)
- Gravitational lensing visualization
- A beautiful starfield background
- Smooth, interactive camera controls

**Step 4: GitHub Integration**
Claude Code then helped me:
- Initialize a git repository
- Configure my git credentials
- Create meaningful commits
- Install the GitHub CLI (`gh`)
- Authenticate with GitHub
- Create and push to the repository
- Set up GitHub Pages for live deployment

### The Magic of AI-Assisted Development

What impressed me most was:
- **Zero boilerplate hassle**: No time wasted on setup
- **Best practices built-in**: Proper Three.js structure, efficient rendering
- **Physics knowledge**: Claude understood orbital mechanics and implemented realistic particle speeds
- **Visual design**: Created a beautiful color scheme and effects without me specifying them
- **DevOps automation**: Handled all the git and GitHub setup seamlessly

The entire project, from concept to live deployment, took just a few minutes of conversation.

## 🚀 Running Locally

1. Clone the repository:
```bash
git clone https://github.com/julienokumu/vibed-claude-blackhole-sim.git
cd vibed-claude-blackhole-sim
```

2. Open `index.html` in your web browser:
```bash
# On Linux/Mac
open index.html

# Or just double-click the file
```

That's it! The simulation uses Three.js from a CDN, so no build process or dependencies are needed.

## 🛠️ Technical Details

### Technology Stack
- **Three.js 0.160.0**: 3D graphics rendering
- **OrbitControls**: Camera manipulation
- **Vanilla JavaScript**: No frameworks needed

### Physics Implementation
The accretion disk particles follow simplified Keplerian orbital mechanics:
```javascript
particle.speed = 0.5 / radius  // Inner particles orbit faster
```

### Performance
- Efficiently renders 15,000+ objects (5,000 disk particles + 10,000 stars)
- Smooth 60 FPS on modern hardware
- Uses `BufferGeometry` and `Points` for optimal performance

## 🎨 Visual Effects Breakdown

1. **Event Horizon**: Black sphere at radius 1.0 (Schwarzschild radius)
2. **Photon Sphere**: Transparent wireframe at radius 1.5 (where light orbits)
3. **Accretion Disk**: Particles from radius 2.5 to 6.5 with varying heights
4. **Color Temperature**: RGB values calculated based on distance from center
5. **Additive Blending**: Creates realistic glowing effect for hot matter

## 📝 Code Structure

```
index.html
├── Scene Setup (camera, renderer, controls)
├── Background Stars (10,000 point cloud)
├── Black Hole (event horizon sphere)
├── Photon Sphere (wireframe visualization)
├── Accretion Disk (5,000 animated particles)
├── Lensing Ring (gravitational effect)
└── Animation Loop (particle updates, rendering)
```

## 🌟 Future Enhancements

Potential additions:
- Shader-based gravitational lensing of background stars
- Hawking radiation particle effects
- Relativistic jets from the poles
- Doppler shifting for approaching/receding disk material
- VR support for immersive viewing

## 🙏 Acknowledgments

Built with **Claude Code** - an AI coding assistant that turned a simple idea into a fully functional, deployed web application in minutes.

Powered by [Giga AI Free](https://free.gigamind.dev/) - making advanced AI accessible to everyone.

## 📄 License

MIT License - Feel free to use this code for your own projects!

## 👨‍💻 Author

**Julien Okumu**
- GitHub: [@julienokumu](https://github.com/julienokumu)
- Email: codewithjulien@gmail.com

---

*Remember: In space, no one can hear you code... but they can see your awesome simulations!* 🚀
