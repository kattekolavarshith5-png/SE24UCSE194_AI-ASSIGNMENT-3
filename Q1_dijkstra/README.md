This project is a Python-based application that calculates the shortest path between cities using **Dijkstra’s Algorithm** and real-world distance data from the **Google Distance Matrix API**.

---

## 🚀 Features

- 🌍 Fetch real-time distances between cities using Google API
- 🧠 Uses Dijkstra’s Algorithm for shortest path calculation
- 💾 Stores graph data locally (JSON cache)
- ➕ Add new cities dynamically
- 🔄 Rebuild entire graph anytime
- 📌 Interactive menu-driven program

---

## 🛠️ Technologies Used

- Python
- Google Distance Matrix API
- heapq (Priority Queue)
- requests
- dotenv (for API key management)
- JSON (for caching)

---

## 📂 Project Structure

```

├── main.py                # Main application file
├── distance_store.json   # Cached graph data
├── .env                  # API key storage
└── README.md             # Documentation

```

---

## 🔑 Setup Instructions

### 1. Clone the repository

```

git clone <your-repo-link>
cd <your-project-folder>

```

### 2. Install dependencies

```

pip install requests python-dotenv

```

### 3. Setup API Key

Create a `.env` file in the root directory:

```

GOOGLE_API_KEY=your_api_key_here

```

> ⚠️ Make sure your API key has access to **Distance Matrix API**

---

## ▶️ How to Run

```

python main.py

```

---

## 📋 Menu Options

1. Add new cities  
2. Rebuild full graph  
3. Compute shortest path  
4. Show cities  
5. Exit  

---

## 🧠 How It Works

- The program builds a graph where:
  - Nodes = Cities
  - Edges = Distance between cities (in km)

- Uses **Dijkstra’s Algorithm**:
  - Finds shortest path from source to destination
  - Uses priority queue for efficiency

---

## 💡 Example

```

Source: Delhi
Destination: Chennai

Distance: 2200 km
Route: Delhi -> Nagpur -> Chennai

```

---

## 📌 Notes

- Distances are fetched in **kilometers**
- If API fails, distances may be set to infinity
- Cached data helps reduce API calls and costs

---

## ⚠️ Limitations

- Requires internet connection for API calls
- API has usage limits (Google billing may apply)
- Large number of cities may slow performance

---

## 🔮 Future Improvements

- GUI interface (Tkinter / Web App)
- Map visualization
- Traffic-based routing
- Heuristic algorithms (A*)

---

## 👨‍💻 Author

Varshith Kattekola

---

## 📜 License

This project is for educational purposes.
```
