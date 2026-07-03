# PyCraft — A Minecraft Clone in Python

A voxel-based sandbox game inspired by Minecraft, built entirely in Python using the [Ursina Engine](https://www.ursinaengine.org/). Explore, mine, and build in a procedurally generated 3D block world.

## 📖 Description

PyCraft is a lightweight recreation of Minecraft's core gameplay loop — walking around a blocky world, breaking blocks, and placing new ones — built as a learning project and demonstration of what's possible with Ursina, a beginner-friendly game engine built on top of Panda3D. It's not meant to replace Minecraft, but to explore game development fundamentals like first-person controls, voxel terrain generation, block interaction, and simple world persistence, all in pure Python.

## ✨ Features

- 🧱 **Block placing & breaking** — Left-click to break, right-click to place
- 🌍 **Procedurally generated terrain** using noise-based height maps
- 🎒 **Multiple block types** (grass, dirt, stone, sand, wood, etc.) with a simple hotbar/inventory
- 🚶 **First-person movement & camera controls** with WASD + mouse look
- 🦘 **Gravity, jumping, and collision detection**
- 🌤️ **Day/skybox environment**
- 💾 **(Optional) World save/load** — persist changes between sessions

## 🕹️ Controls

| Key / Input       | Action            |
|--------------------|-------------------|
| `W A S D`          | Move              |
| `Mouse`             | Look around       |
| `Space`             | Jump              |
| `Left Click`        | Break block       |
| `Right Click`       | Place block       |
| `1-9`               | Select block type |
| `Esc`               | Quit / release mouse |

## 🛠️ Requirements

- Python 3.9+
- [Ursina Engine](https://www.ursinaengine.org/)

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/pycraft.git
   cd pycraft
   ```

2. **Create a virtual environment (recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

   Or install Ursina directly:
   ```bash
   pip install ursina
   ```

4. **Run the game**
   ```bash
   python main.py
   ```

## 📁 Project Structure

```
pycraft/
├── main.py              # Entry point — sets up the Ursina app and game loop
├── world.py              # Terrain generation and chunk/block management
├── player.py              # First-person controller, physics, interaction
├── block_types.py         # Block definitions and textures
├── assets/
│   ├── textures/          # Block and UI textures
│   └── models/            # Any custom 3D models
├── requirements.txt
└── README.md
```

## 🚀 Roadmap / Ideas

- [ ] Infinite chunk-based world generation
- [ ] Caves and ore generation
- [ ] Simple mobs/enemies
- [ ] Crafting system
- [ ] Multiplayer support
- [ ] Sound effects and music

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome! Feel free to open an issue or submit a pull request.

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Ursina Engine](https://www.ursinaengine.org/) for making 3D game dev in Python approachable
- Inspired by Mojang's *Minecraft*
