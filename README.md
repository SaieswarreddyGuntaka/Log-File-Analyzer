# 🧾 Log File Analyzer (Beginner-Friendly)

A simple Python script that reads and analyzes Apache-style web server logs to provide insights such as:

- Top IP addresses making requests  
- Most requested endpoints (paths)  
- Error status code summary (e.g., 404, 500)

Built using:
- Python 3
- `re` (Regular Expressions)
- `collections.Counter` for aggregation

---

## ✨ Features

- Parses standard Apache log format  
- Displays:
  - Top 5 IP addresses
  - Top 5 requested endpoints
  - Count of HTTP 4xx and 5xx error codes  
- Easily extendable to add visualizations or export options

---

## 📁 Project Structure


- log-file-analyzer/
 -├── analyze\_logs.py       # Main script for log parsing and analysis
 -├── sample.log            # Sample Apache-style log file for testing
 -└── README.md             # Documentation

````

---

## ⚙️ Getting Started

### 1️. Clone or Download the Repository

```bash
git clone https://github.com/yourusername/log-file-analyzer.git
cd log-file-analyzer
````

---

### 2️. Run the Script

Make sure you have Python 3 installed.

```bash
python analyze_logs.py
```

You will see the top IPs, most visited paths, and a summary of error codes printed in your terminal.

---

## 🧪 Sample Input

Here’s a sample `sample.log` file in standard Apache log format:

```
192.168.1.1 - - [11/Jun/2025:10:00:00 -0500] "GET /index.html HTTP/1.1" 200 2326
192.168.1.2 - - [11/Jun/2025:10:01:00 -0500] "GET /about.html HTTP/1.1" 404 720
192.168.1.1 - - [11/Jun/2025:10:02:00 -0500] "POST /submit HTTP/1.1" 500 123
192.168.1.3 - - [11/Jun/2025:10:03:00 -0500] "GET /contact.html HTTP/1.1" 200 1045
192.168.1.1 - - [11/Jun/2025:10:04:00 -0500] "GET /index.html HTTP/1.1" 200 2326
```

---

## 📤 Output Example

When you run the script, the output will look like this:

```
Top 5 IP addresses:
[('192.168.1.1', 3), ('192.168.1.2', 1), ('192.168.1.3', 1)]

Top 5 Requested Paths:
/index.html - 2
/about.html - 1
/submit - 1
/contact.html - 1

Error Code Summary:
404 - 1
500 - 1
```

---

## 📦 Files Included

* `analyze_logs.py` – Python script to parse and analyze logs
* `sample.log` – Sample log file in Apache format
* `README.md` – Project overview and documentation

---

## 🤝 Contributions

Want to contribute?

* Add support for other log formats (e.g., NGINX)
* Export results to CSV or JSON
* Add a web interface using Flask or Streamlit
* Create visualizations using Matplotlib or Plotly

Pull requests are welcome!

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🙋‍♂️ Questions?

Feel free to open an issue or contact me if you need help understanding the script or extending it for your own logs.
Happy coding! 🚀

```

Let me know if you'd like a matching `LICENSE` file or instructions for pushing this to GitHub.
```

