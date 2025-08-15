# 🌦 Python Weather API — Historical Data (200+ Years)

A **Flask-based Weather API** that serves **historical weather data spanning over 200 years**.  
This project demonstrates my ability to:
- Build **scalable APIs**
- Efficiently manage and query **large datasets**
- Design clean and maintainable Python backends

---

## 🚀 Features
- RESTful API endpoints for querying historical weather data
- Data spanning **more than two centuries**
- Efficient search and filtering by:
  - Date
  - Location
  - Weather conditions
- Pagination for large result sets
- JSON-formatted responses
- Built with scalability and performance in mind

---

## 📦 Installation
Make sure you have **Python 3.9+** installed.

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/weather-api-flask.git
cd weather-api-flask
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Set up the dataset**
   - Place the historical weather dataset in the `data/` directory.
   - Supported formats: `.csv`, `.json`, or connect to a database.

---

## 🖥 Usage

### Run the API
```bash
python app.py
```
Default server: `http://127.0.0.1:5000`

---

## 🌐 Example Endpoints

### Get All Records (Paginated)
```
GET /api/weather?page=1&limit=50
```

### Filter by Date
```
GET /api/weather?date=1950-07-21
```

### Filter by Location
```
GET /api/weather?city=London
```

### Combined Filters
```
GET /api/weather?city=New York&date=1899-12-25
```

---

## 📂 File Structure
```
📁 weather-api-flask
 ├── app.py               # Main Flask application
 ├── requirements.txt     # Dependencies
 ├── README.md            # Documentation
 ├── data/                # Historical dataset
 └── utils/               # Data loading and query helpers
```

---

## 🧰 Dependencies
- **Flask** — Web framework for API creation
- **pandas** — Data loading and manipulation
- **gunicorn** — For production deployment
- **sqlite3 / PostgreSQL** — Optional database support

Install them all:
```bash
pip install -r requirements.txt
```

---

## 💡 How It Works
1. **Load Dataset** → Data is loaded from CSV/Database into memory or queried dynamically.
2. **Handle API Requests** → Flask routes process incoming requests with filtering, sorting, and pagination.
3. **Return JSON** → Results are returned as clean, structured JSON for easy integration.

---

## 📜 License
Licensed under the MIT License — free to use and modify.

---

## ⭐ Show Your Support
If you find this project useful, give it a ⭐ on GitHub!
