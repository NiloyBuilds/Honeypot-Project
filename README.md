# Java Honeypot System

A **Honeypot server** built in Java for detecting suspicious network activity, such as rapid scanning or Nmap probes.  
This project simulates a fake web server to attract and log potential attackers, while recording IPs, device details, and timestamps.

---

## 🏷️ Features

- Listens on a configurable port (default 2222)  
- Detects **rapid scans / Nmap probes** using time threshold (1 second)  
- Logs IP addresses, timestamps, and device/user-agent info  
- Serves a **fake HTML page** (`login.html`) to simulate a web server  
- Saves logs to a configurable log file (`logs/connections.log`)  
- Simple concurrency-safe handling using `ConcurrentHashMap`  

---

## 📁 Project Files

| File | Description |
|------|-------------|
| `Honeypot.java` | Main Java server code |
| `config/config.txt` | Configuration file (port and log file path) |
| `login.html` | Fake HTML page served to clients |
| `logs/connections.log` | Auto-generated log file of detected connections |

---

