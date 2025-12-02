🕵️‍♀️ Python Network Sniffer

A lightweight Python packet sniffer built using Scapy, capable of capturing and analyzing live network traffic with real-time packet inspection.

📌 Overview

This project is a simple yet powerful network analysis tool created during my cybersecurity internship. It captures packets on a chosen network interface and extracts useful details such as protocol type, source/destination IP, timestamps, and raw payload data.

It works similar to basic packet monitoring utilities and helps students understand how real-time traffic analysis works at a low level.

✨ Features

📡 Live packet capture (no file needed)

🧭 Source and Destination IP extraction

🔎 Protocol identification (TCP, UDP, ICMP)

⏱ Timestamp logging

📄 Payload extraction (Raw layer)

🧾 Optional logging to file

🌐 Works on Linux, CentOS, and Kali machines

🧱 Project Structure
python-network-sniffer/
│
├── sniffer.py          # Main script for packet capture
├── packet_logs.txt     # Log file (optional)
└── README.md           # Documentation

⚙ Requirements

Install Scapy:

pip3 install scapy


You must run the script with root privileges:

sudo python3 sniffer.py

▶️ How It Works

The script uses Scapy’s sniff() function to:

Listen on a network interface (ens33, wlan0, eth0, etc)

Capture each incoming/outgoing packet

Extract:

Timestamp

Source IP

Destination IP

Transport protocol

Raw payload (if available)

Print details in clean readable format

Optionally log packets to a file

This gives beginners a practical understanding of packet anatomy and real-time traffic flow.

🚀 Run the Sniffer

Run the sniffer directly:

python3 sniffer.py

📥 Example Output
========== PACKET ==========
Time: 2025-12-02 18:00:53
Source IP: 172.67.212.105
Destination IP: 192.168.149.145
Protocol: TCP
Payload: b'HTTP/1.1 301 Moved Permanently\r\nDate: ...'

📌 Future Improvements

Planned enhancements:

Add color-coded terminal output

Build an HTML dashboard for packet visualization

Export packets to CSV / JSON

Add filtering options (port, protocol, IP)

Add multithreading

Build a GUI version using PyQt5

📄 License

MIT License. Free to use, modify, and learn from.

🧑‍💻 Author

Aailah
Cybersecurity & Automation
GitHub: https://github.com/Aaila-IO

If you want, I will also:

✔ improve your sniffer code
✔ rewrite comments inside code
✔ add color output
✔ add filtering (HTTP only, TCP only, DNS only etc)
✔ make this entire project look senior-level

Just say: “upgrade my sniffer code” and I’ll do it.
