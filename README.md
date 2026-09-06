# BLOCKCRAFT 🎮

> A tiny voxel sandbox game. Build, break, and explore!

![HTML5](https://img.shields.io/badge/HTML5-E34C26?style=flat-square&logo=html5&logoColor=white)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=three.js&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

---

## 🌟 Features

- **Fully explorable voxel world** - Infinite-feeling terrain generated with procedural noise
- **6 block types** - Grass, Dirt, Stone, Wood, Leaves, and Sand
- **Dynamic trees** - Procedurally generated trees scattered across the landscape
- **Smooth first-person camera** - Mouse look with intuitive controls
- **Build & break blocks** - Left-click to destroy, right-click to place
- **Flying mode** - Toggle flight for creative exploration
- **Real-time statistics** - Track blocks placed/broken in your session
- **Optimized rendering** - Uses instanced meshes for smooth 60 FPS performance

---

## 🎮 How to Play

### **Controls**

| Key | Action |
|-----|--------|
| **W / A / S / D** | Move forward / left / backward / right |
| **Mouse** | Look around |
| **Space** | Jump (press twice to fly) |
| **Shift** | Fly downward (while flying) |
| **Left Click** | Break block |
| **Right Click** | Place block |
| **1-6** | Select block type |
| **Esc** | Pause / return to menu |

### **Block Types**

1. 🟢 **Grass** - The top layer of terrain
2. 🟤 **Dirt** - Found below grass
3. ⬜ **Stone** - Deep underground blocks
4. 🟫 **Wood** - Used for tree trunks
5. 🌲 **Leaves** - Tree foliage
6. 🟨 **Sand** - Desert-like blocks

### **Tips**

- **Double-tap Space** to enter flying mode and explore freely
- Use **Shift** while flying to descend
- The world extends ~26 blocks in all directions
- Your position and block count are shown in the top-left corner

---

## 🚀 Play Now

### Online
Play directly in your browser at: **[GitHub Pages URL will go here]**
- No installation needed
- Runs on desktop browsers (Chrome, Firefox, Safari, Edge)
- Works best on desktop; mobile support limited

### Locally
1. Download or clone this repository
2. Open `index.html` in your web browser
3. Click "Click to play" and start building!

---

## 🛠️ Technical Details

### Built With
- **Three.js** - 3D graphics library
- **Vanilla JavaScript** - No frameworks
- **HTML5 Canvas** - Rendering

### Architecture
- **Voxel Storage** - Map-based key-value storage for world blocks
- **Instanced Rendering** - Efficient mesh rendering using Three.js InstancedMesh
- **Procedural Generation** - Sine/cosine-based pseudo-noise for terrain
- **Raycasting** - Precise block selection with mouse

### Performance
- Optimized for 60 FPS on modern devices
- Efficient culling with fog
- Dynamic mesh rebuilding on block changes

---

## 🎨 Customization

Want to modify the game? Here are some easy tweaks:

### **Change World Size**
In the code, find:
```javascript
const WORLD_SIZE = 26;
```
Increase or decrease this number for a larger/smaller world.

### **Add More Block Types**
Add to the `BLOCK_TYPES` array:
```javascript
{ id: 7, name: 'MyBlock', color: 0xFF5733 },
```

### **Adjust Terrain Height**
Modify the pseudoNoise function or the height calculation:
```javascript
let h = Math.floor(4 + pseudoNoise(x, z));
```

### **Change Colors**
Hex color codes for each block type are in `BLOCK_TYPES`:
```javascript
{ id: 1, name: 'Grass', color: 0x5b9b3b }, // Change 0x5b9b3b
```

---

## 📦 File Structure

```
blockcraft/
├── index.html          # Main game file (all-in-one)
└── README.md          # This file
```

---

## 🐛 Known Limitations

- No multiplayer support
- No save/load functionality (yet)
- Limited mobile support (small touch targets)
- World doesn't wrap (edges are hard boundaries)

---

## 🚀 Future Features

- [ ] Save/load world functionality
- [ ] More block types and textures
- [ ] Day/night cycle
- [ ] Creative inventory system
- [ ] Sound effects
- [ ] Multiplayer support
- [ ] Mobile touch controls

---

## 📄 License

This project is open source and available under the **MIT License** - feel free to use, modify, and share!

---

## 🙏 Credits

- **Three.js** - Graphics library
- **Procedural generation** - Inspired by classic voxel games
- Made with ❤️ as a fun sandbox experiment

---

## 💬 Feedback & Contributions

Found a bug? Have an idea? Feel free to:
- Open an issue
- Fork and submit a pull request
- Share your creations!

---

**Happy building! 🏗️**
Website is:https://venkatramanyadav-design.github.io/
