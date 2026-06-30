# 📊 API Performance Monitor

A Python-based API Performance Monitor that continuously tracks the availability, response time, and status of REST APIs. The application logs API metrics, stores historical data in a database, and generates reports to help monitor API health and performance.

---

## 🚀 Features

- Monitor multiple REST APIs
- Measure response time and latency
- Track HTTP status codes
- Store API performance logs in SQLite
- Generate CSV reports
- Scheduled monitoring at regular intervals
- Error and timeout handling
- Simple, modular, and scalable architecture

---

## 🛠️ Tech Stack

- Python 3.x
- Requests
- SQLite
- Pandas
- APScheduler
- CSV
- Logging

---

## 📂 Project Structure

```
API_Performance_Monitor/
│
├── app.py
├── monitor.py
├── scheduler.py
├── database.py
├── export_csv.py
├── config.py
├── requirements.txt
├── api_monitor.db
│
├── reports/
│   └── api_report.csv
│
├── logs/
│   └── monitor.log
│
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/API_Performance_Monitor.git
cd API_Performance_Monitor
```

### 2. Create a virtual environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**macOS/Linux**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

### Start the API monitor

```bash
python app.py
```

### Run scheduled monitoring

```bash
python scheduler.py
```

### Export performance report

```bash
python export_csv.py
```

---

## 🗄️ Database Schema

```sql
CREATE TABLE api_logs (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    api_url TEXT,
    status_code INTEGER,
    response_time REAL,
    checked_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

---

## 📈 Workflow

```
API Endpoint
      │
      ▼
HTTP Request
      │
      ▼
Measure Response Time
      │
      ▼
Store in SQLite
      │
      ▼
Generate Reports
      │
      ▼
CSV Export
```

---

## 📊 Sample Output

### Database

| API URL | Status Code | Response Time | Checked At |
|---------|-------------|---------------|------------|
| https://api.example.com | 200 | 0.24 sec | 2026-06-30 |

### CSV Report

```csv
API URL,Status Code,Response Time,Checked At
https://api.example.com,200,0.24,2026-06-30 10:30:15
```

---

## 📚 Learning Outcomes

This project demonstrates:

- API Monitoring
- HTTP Requests with Requests
- Performance Measurement
- SQLite Database Integration
- Task Scheduling
- CSV Report Generation
- Logging and Error Handling
- Python Automation

---

## 🔮 Future Enhancements

- Email alerts for API failures
- Real-time dashboard with Flask or Streamlit
- Response time visualization using Matplotlib
- Slack/Discord notifications
- PostgreSQL or MySQL support
- Docker deployment
- Multi-threaded API monitoring
- Authentication support for protected APIs

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License.

---

## 👩‍💻 Author

**Tripti Bharadwaj Pandey**

If you found this project useful, consider giving it a ⭐ on GitHub!
