# ✈️ Airport Shortest Path Finder

A web-based application that finds the shortest route between two airports using **Dijkstra's algorithm**, built with Django and MySQL.

---

##  Features

- **Shortest Path Finder** — Calculates the optimal route between any two airports using Dijkstra's algorithm
- **Airport Management** — Add, view, and delete airports from the system
- **Route Management** — Add, view, and delete routes (edges) between airports with defined distances/weights
- **Web Interface** — Clean and user-friendly interface built with Django templates

---

##  Tech Stack

| Layer       | Technology        |
|-------------|-------------------|
| Backend     | Python, Django    |
| Frontend    | HTML, CSS         |
| Database    | MySQL             |
| Algorithm   | Dijkstra's Algorithm |

---

##  Project Structure

```
airport-shortest-path/
│
├── airports/               # Main Django app
│   ├── models.py           # Airport and Route models
│   ├── views.py            # Core logic and Dijkstra's implementation
│   ├── urls.py             # URL routing
│   └── templates/          # HTML templates
│
├── static/                 # CSS and static assets
├── manage.py               # Django management script
├── requirements.txt        # Python dependencies
└── README.md
```

---

##  Installation & Setup

### Prerequisites

- Python 3.8+
- MySQL Server
- pip

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/airport-shortest-path.git
   cd airport-shortest-path
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate        # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   
4. **Run migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Start the development server**
   ```bash
   python manage.py runserver
   ```

##  How It Works

1. **Add Airports** — Enter airport names/codes into the system
2. **Add Routes** — Define connections between airports with a distance or cost value
3. **Find Shortest Path** — Select a source and destination airport; the app applies Dijkstra's algorithm to return the shortest route and total distance

---
