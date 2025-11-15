# RedSpecter

---

## What It Does
RedSpecter is a dual-mode attack tool that overwhelms target systems with either:
- **Bandwidth Flood**: Sends high-volume UDP packets to a specified IP and port, saturating network bandwidth.
- **HTTP Flood**: Bombards a target website with HTTP requests, including bot hammering to mimic search engine and social media bots.

It provides real-time statistics, including:
- Packets/requests sent
- Total data transferred (MB)
- Average throughput (Mbps)
- Requests per second (RPS) for HTTP Flood
- Response times (average and max) for HTTP Flood
- Elapsed and remaining time

## Features
- **Multi-threaded UDP Flooding**: Parallel threads maximize packet delivery speed.
- **Asynchronous HTTP Flooding**: Leverages `aiohttp` for high-performance HTTP requests.
- **Configurable Parameters**:
  - UDP: IP, port, duration, packet size, thread count.
  - HTTP: URL, thread count, request path.
- **Real-time Progress Tracking**: Live console updates with colorful output.
- **Accurate Metrics**: Tracks throughput, success/failure rates, and response times.
- **Error Handling**: Monitors target status and handles failed requests gracefully.
- **Cross-platform**: Runs on Linux, Windows, macOS, and Termux (Android).

---

## Installation

### For Termux Users (Android)

```bash
git clone https://github.com/ethz07/redspecter.git
cd redspecter
pip install -r requirements.txt

python menu.py
```

### For PC Users

```bash
pip install colorama
python menu.py
```

---

![Screenshot of menu](images/menu.png)

---

# Use responsibly. Only test on systems you own or have explicit permission to stress test.
DISCLAIMER: This tool is provided "as is" for educational and authorized penetration testing purposes only. The developer (@ethz07) and any contributors are not responsible for any misuse, illegal activities, damage to systems, networks, or data caused by this software.
All responsibility belongs to the user. You are solely liable for how you use this tool. Unauthorized attacks are illegal in most jurisdictions.

---

## Developer

**@ethz07 - RedSpecter**

---


