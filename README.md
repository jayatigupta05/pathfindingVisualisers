# 🧭 Pathfinding Visualizer (A*, Dijkstra, BFS, DFS) with Pygame

An **interactive pathfinding visualizer** built with **Python + Pygame**, featuring four classic algorithms:
- ✨ **A\*** (with heuristic)  
- 📍 **Dijkstra's Algorithm**  
- 🌐 **Breadth-First Search (BFS)**  
- 🌀 **Depth-First Search (DFS)**  

🧱 You can draw walls, set start/end points, and watch how each algorithm explores the grid in real-time.

---

## 📂 Project Structure
```
├── a_star.py # ✨ A* pathfinding implementation
├── bfs.py # 🌐 Breadth-First Search
├── config.py # ⚙️ (Optional) configuration/parameters
├── dfs.py # 🌀 Depth-First Search
├── dijkstra.py # 📍 Dijkstra's shortest path
├── grid.py # 🎨 Grid + visualization logic
├── main.py # 🖥️ Interactive Pygame application
└── README.md # 📖 Project documentation
```

---

## 🎮 Features
- 🎨 **Grid-based visualization** with Pygame  
- 🖱️ **Mouse interactions**:
  - 🟢 Left-click → set **Start** node  
  - 🔴 Right-click → set **End** node  
  - 🧱 Middle-click → toggle a **Wall**  
- 🧭 **Buttons for algorithms**:
  - 🚀 `A*`, 🌐 `BFS`, 🌀 `DFS`, 📍 `Dijkstra`  
- ⚡ **Extra buttons**:
  - 🎲 `Random Walls` → generate random obstacles  
  - ♻️ `Clear` → reset the grid  
- 🖥️ **Smooth drawing** with double buffering (no flickering)  
- 📑 **UI Panel** below the grid for algorithm selection    

---

## 🛠 Requirements
- 🐍 **Python 3.8+**  
- 📦 Install dependencies:
```
pip install pygame
```

## ▶️ Running the Visualizer

Clone the repository and start `main.py`:

```
git clone https://github.com/yourusername/pathfinding-visualizer.git
cd pathfinding-visualizer
python main.py
```

---

## 🖥️ Controls

- 🟢 **Left Click** → Place **Start** node  
- 🔴 **Right Click** → Place **End** node  
- 🧱 **Middle Click** → Place/Remove **Wall**  

### 🔘 Buttons (below grid)
- 🚀 `A*` → Run A* Search  
- 🌐 `BFS` → Run Breadth-First Search  
- 🌀 `DFS` → Run Depth-First Search  
- 📍 `Dijkstra` → Run Dijkstra's Algorithm  
- 🎲 `Random Walls` → Generate random walls  
- ♻️ `Clear` → Reset grid  

---

## 📊 Algorithm Comparison

| 🔎 Algorithm   | 🌟 Optimal? | ✅ Complete? | ⚖️ Weighted? | 📝 Notes                                   |
|----------------|-------------|--------------|--------------|--------------------------------------------|
| 🌐 **BFS**     | ✅           | ✅            | ❌            | Finds shortest path in unweighted grids     |
| 🌀 **DFS**     | ❌           | ✅            | ❌            | Explores deep, not guaranteed optimal       |
| 📍 **Dijkstra**| ✅           | ✅            | ✅            | Weighted graphs, no heuristic               |
| 🚀 **A\***     | ✅           | ✅            | ✅            | Uses heuristic (e.g. Manhattan) to guide search |

---

## 📌 Roadmap

- 🧩 Add maze generation algorithms (recursive division, Prim’s, etc.)  
- ↔️ Add diagonal movement support  
- 💾 Save & load grids  
- ⚡ Performance profiling for large grids  
