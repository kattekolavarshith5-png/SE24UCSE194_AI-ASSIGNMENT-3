# 🚗 UGV Path Planning Simulator (A* Algorithm)

This project simulates an **Unmanned Ground Vehicle (UGV)** navigating a grid environment using the **A\* (A-Star) pathfinding algorithm**. It supports obstacle generation, performance analysis, and visual path representation.

---

## 🚀 Features

- 🧠 A* pathfinding with Euclidean heuristic
- 🌍 Random grid generation with obstacle density levels
- 📍 User-defined start and goal positions
- 📊 Performance metrics (distance, efficiency, nodes explored, etc.)
- 🎨 Graphical visualization using matplotlib
- 🔄 Interactive menu-driven interface

---

## 🛠️ Technologies Used

- Python
- NumPy
- Matplotlib
- heapq (priority queue)
- math
- random
- time

---

## 📂 Project Structure

```

├── README.md   
└── code.py
└──requirements.txt

```

---

## ▶️ How to Run

### 1. Install dependencies

```

pip install numpy matplotlib

```

### 2. Run the program

```

python ugv_simulator.py

```

---

## 📋 Menu Options

1. Generate Grid  
2. Set Start/Goal  
3. Run A*  
4. Show Stats  
5. Exit  

---

## 🌐 Grid Details

- Grid Size: **70 x 70**
- Each cell represents:
  - `0` → Free space
  - `1` → Obstacle

### Obstacle Density Levels:

| Level  | Description | Density |
|--------|------------|--------|
| 1      | Low        | 15%    |
| 2      | Medium     | 30%    |
| 3      | High       | 50%    |

---

## 🧠 Algorithm Used: A*

- Combines:
  - **g(n)** → Cost from start
  - **h(n)** → Heuristic (Euclidean distance)

- Formula:

```

f(n) = g(n) + h(n)

```

- Movement:
  - 4-directional (cost = 1)
  - Diagonal (cost = 1.414)

---

## 📊 Performance Metrics

After running A*, the program provides:

- Straight-line distance
- Actual path distance
- Efficiency (%)
- Nodes expanded
- Path length (nodes count)
- Number of turns
- Execution time (ms)

---

## 🎨 Visualization

- ⬛ Black → Obstacles  
- 🔵 Blue → Path  
- 🟢 Green → Start  
- 🔴 Red → Goal  

---

## 💡 Example Workflow

```

1. Generate Grid → Select density
2. Set Start and Goal positions
3. Run A* algorithm
4. View path visualization
5. Check performance stats

```

---

## ⚠️ Limitations

- No dynamic obstacles
- Large grids may increase computation time
- No real-world map integration

---

## 🔮 Future Improvements

- Add Dijkstra and BFS comparison
- Real-time moving obstacles
- GUI (Tkinter / Web)
- Map-based navigation (Google Maps API)
- Path smoothing techniques

---

## 👨‍💻 Author

Varshith Kattekola

---
