🐉 PacketWyrm - Network Guardian
A modern, Wireshark-like network packet analyzer with real-time capture, threat detection, and plain English explanations.

PacketWyrmLicensePlatform

Features
🔴 Real-time packet capture from any network interface
🔄 Switch interfaces on-the-fly without restart
⚠️ Threat detection with risk scoring
💡 Plain English explanations for all traffic
📊 Protocol analytics with visual breakdown
🔍 Advanced filtering by protocol, IP, or port
💾 CSV export for further analysis
📡 WebSocket streaming for real-time updates
🎨 Modern dark UI inspired by cybersecurity tools
Quick Start
Prerequisites
Docker & Docker Compose
Linux (Kali, Ubuntu, Debian, etc.)
Root/sudo access for packet capture
Installation
# Clone the repositorygit clone https://github.com/YOUR_USERNAME/packetwyrm.gitcd packetwyrm# Build and rundocker-compose up --build
Access
Open your browser: http://localhost:8080

Manual Installation (without Docker)
bash

# Install dependencies (Debian/Ubuntu/Kali)
sudo apt install libpcap-dev

# Build
cd backend
go mod tidy
CGO_ENABLED=1 go build -o packetwyrm .

# Run with root (required for packet capture)
sudo ./packetwyrm
Usage
Select Interface - Choose network interface from dropdown
Start/Stop Capture - Control packet capture
Filter by Protocol - Click protocol buttons in sidebar
Search - Enter IP address or keyword
Inspect - Click any packet for detailed info
Export - Download captured packets as CSV
Threat Analysis - Red highlighted packets are potential threats
Supported Protocols
HTTP / HTTPS
DNS
TCP / UDP
SSH
ICMP
ARP
Threat Detection
PacketWyrm automatically detects:

Traffic from blacklisted IPs (Tor exits, known malicious)
Connections to suspicious ports (4444, 5555, etc.)
External SSH attempts
Unusual port scanning activity
License
MIT License - Free forever
