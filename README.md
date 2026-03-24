# 🗺️ FORT Algo Visualizer 2026

A **pathfinding algorithm visualizer** built with Python and Tkinter. Visualize how classic search algorithms navigate a grid in real-time — watch them explore, backtrack, and find the shortest path step by step.

---

## 📸 Preview

> Set a **Start** node → Set a **Target** node → Place **walls** → Click any algorithm!

---

## 🚀 Features

- 🟩 **Interactive Grid** — Click to place Start, Target, and Wall nodes on a 15×15 grid
- 🎨 **Real-time Visualization** — Watch each algorithm explore nodes with color-coded animations
- 🟡 **Final Path Highlighting** — The shortest (or found) path is traced in yellow
- 🔄 **Reset Button** — Clear the grid and start fresh anytime
- 6 classic search algorithms supported out of the box

---

## 🧠 Algorithms Included

| Algorithm | Description |
|-----------|-------------|
| **Breadth First Search (BFS)** | Explores level by level; guarantees shortest path |
| **Depth First Search (DFS)** | Explores as deep as possible first; does not guarantee shortest path |
| **Uniform Cost Search (UCS)** | Expands least-cost node first; optimal for weighted graphs |
| **Depth Limited Search (DLS)** | DFS with a fixed depth limit (default: 15) |
| **Iterative Deepening DFS (IDDFS)** | Combines DFS space efficiency with BFS optimality |
| **Bidirectional Search** | Searches simultaneously from Start and Target; meets in the middle |

---

## 🖱️ How to Use

1. **Click once** on the grid → Sets the **Start node** (green)
2. **Click again** on another cell → Sets the **Target node** (blue)
3. **Click any remaining cell** → Places a **Wall** (red, impassable)
4. **Click an algorithm button** on the sidebar → Watch it run!
5. **Click RESET GRID** → Clears everything and start over

---

## ⚙️ Requirements

- Python 3.x
- Tkinter *(comes pre-installed with standard Python)*
- No external packages needed!

---

## ▶️ Run the Project

```bash
python Q7.py
```

---

## 📁 Project Structure

```
📦 fort-algo-visualizer/
 ┣ 📜 Q7.py          # Main application file
 ┗ 📜 README.md      # Project documentation
```

---

## 🎨 Color Guide

| Color | Meaning |
|-------|---------|
| 🟩 Green | Start Node |
| 🔵 Blue | Target Node |
| 🔴 Red | Wall (blocked) |
| 🟠 Orange | Currently exploring |
| 🩵 Cyan | Discovered / Frontier |
| 🟣 Purple/Magenta | Bidirectional backward search |
| 🟡 Yellow | Final path |

---

## 🔧 Configuration

You can tweak these constants at the top of the `PathFinder` class:

```python
self.grid_size = 15      # Number of rows/columns
self.cell_size = 40      # Pixel size of each cell
```

For **Depth Limited Search**, the default depth limit is `15`. Change it here:

```python
self.add_btn("Depth Limited", self.colors["DLS"], lambda: self.exec_dls(15))
#                                                                         ^^
#                                                              Change this value
```

---

## 📚 Concepts Demonstrated

- Graph traversal and search algorithms
- Parent mapping for path reconstruction
- Bidirectional search with frontier merging
- Priority queue usage with `heapq` (UCS)
- Real-time GUI updates with `tkinter`

---

## 🤝 Contributing

Pull requests are welcome! If you'd like to add:
- A* Search
- Greedy Best-First Search
- Diagonal movement toggle
- Weighted edges

Feel free to fork the repo and open a PR.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Made with ❤️ using Python & Tkinter*

Display

<img width="808" height="674" alt="image" src="https://github.com/user-attachments/assets/7605169c-c237-48c6-b97e-84b7e3ffa976" />


