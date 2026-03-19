# 🚗 Dynamic UGV Path Planning Simulator (A* with Dynamic Obstacles)

This project simulates an **Unmanned Ground Vehicle (UGV)** navigating a grid using the **A\* algorithm** in a **dynamic environment**, where obstacles appear during execution.

---

## 🚀 Features

- 🧠 A* pathfinding with Euclidean heuristic
- 🌍 Random grid generation with configurable density
- 📍 User-defined start and goal positions
- ⚡ Dynamic obstacle injection during runtime
- 🔁 Automatic path replanning when blocked
- 📊 Performance metrics tracking
- 🎨 Visual simulation using matplotlib

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

├── dynamic_ugv.py   # Main simulation code
└── README.md        # Documentation

```

---

## ▶️ How to Run

### 1. Install dependencies

```

pip install numpy matplotlib

```

### 2. Run the program

```

python dynamic_ugv.py

```

---

## 📋 Menu Options

1. Generate Grid  
2. Set Points  
3. Run Simulation  
4. Show Metrics  
5. Exit  

---

## 🌐 Grid Details

- Grid Size: **70 x 70**
- Cell values:
  - `0` → Free space
  - `1` → Static obstacle
  - `2` → Dynamic obstacle

---

## ⚙️ Obstacle Configuration

### Density Levels:

| Level | Description | Density |
|-------|------------|--------|
| 1     | Low        | 15%    |
| 2     | Medium     | 30%    |
| 3     | High       | 50%    |

### Dynamic Obstacles:

- Spawn Rate: Every **5 steps**
- Spawn Count: **8 obstacles per cycle**
- Avoids start and goal positions

---

## 🧠 Algorithm Used: A*

A* combines actual path cost and heuristic:

```

f(n) = g(n) + h(n)

```

- **g(n)** → Cost from start
- **h(n)** → Euclidean distance to goal

### Movement:

- Straight → cost = 1  
- Diagonal → cost = 1.414  

---

## 🔁 Dynamic Replanning

- Obstacles are added during execution
- If path becomes blocked:
  - A* is re-run from current position
  - New optimal path is generated
- Tracks number of replans and expansions

---

## 📊 Performance Metrics

After simulation, the following metrics are shown:

- Total path distance
- Number of replans
- Dynamic obstacles added
- Number of turns
- Execution time (ms)

---

## 🎨 Visualization

- ⬛ Black → Static obstacles  
- 🔴 Red → Dynamic obstacles  
- 🔵 Blue → Path taken  
- 🟢 Green → Start  
- 🔴 Red (goal marker) → Goal  

---

## 💡 Example Workflow

```

1. Generate Grid → Select density
2. Set Start and Goal
3. Run Simulation
4. Watch path adapt to new obstacles
5. Check performance metrics

```

---

## ⚠️ Limitations

- No real-time animation (step-by-step movement)
- Replanning may be computationally expensive
- No advanced dynamic algorithms (e.g., D*, D* Lite)

---

## 🔮 Future Improvements

- Real-time animation of movement
- Implementation of D* Lite algorithm
- GUI-based interface
- Integration with real-world maps
- Smarter obstacle prediction

---

## 👨‍💻 Author

Varshith Kattekola

---

## 📜 License

This project is for educational purposes.
```
