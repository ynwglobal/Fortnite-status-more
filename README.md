# Epic Games Status Monitor 🎮

![Python](https://img.shields.io/badge/python-v3.7+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen.svg)

A comprehensive real-time monitoring tool for Epic Games services, incidents, and free game promotions. Track Fortnite, Epic Games Store, Easy Anti-Cheat (EAC), and more!

## ✨ Features

- 🔍 **Real-time System Status** - Monitor all Epic Games services
- ⚡ **Easy Anti-Cheat (EAC) Tracking** - Specialized EAC status monitoring
- 🚨 **Incident Reports** - Active and recently resolved issues
- 🎁 **Free Games Tracker** - Current and upcoming Epic Store freebies
- 🎨 **Colored Terminal Output** - Easy-to-read status indicators
- 🔄 **Continuous Monitoring** - Auto-refresh with customizable intervals
- 📊 **API Health Monitoring** - Track which endpoints are working

## 🚀 Quick Start

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ynwglobal/epic-games-status-monitor.git
   cd epic-games-status-monitor
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the monitor:**
   ```bash
   python3 fnstatus.py
   ```

### One-Line Install & Run
```bash
git clone https://github.com/ynwglobal/epic-games-status-monitor.git && cd epic-games-status-monitor && pip install -r requirements.txt && python3 fnstatus.py --once
```

## 📖 Usage

### Basic Commands

```bash
# Run once and exit
python3 fnstatus.py --once

# Monitor with 5-minute intervals (default)
python3 fnstatus.py

# Monitor with custom interval (60 seconds)
python3 fnstatus.py 60

# Show help
python3 fnstatus.py --help
```

### Example Output

```
╔══════════════════════════════════════════════════════════════════╗
║                    EPIC GAMES MONITOR v3.1                        ║
║     Status • Incidents • EAC • Free Games • More! (FIXED)         ║
╚══════════════════════════════════════════════════════════════════╝

 SYSTEM STATUS
──────────────────────────────────────────────────────────────────────
Overall Status: ALL SYSTEMS OPERATIONAL

Fortnite                 : OPERATIONAL
Epic Games Store         : OPERATIONAL
Login/Authentication     : OPERATIONAL
Easy Anti-Cheat          : OPERATIONAL

 FREE GAMES & PROMOTIONS
──────────────────────────────────────────────────────────────────────
Currently FREE:
  Sid Meier's Civilization VI Platinum Edition
     Sid Meier's Civilization VI: Platinum Edition is the perfect...
     Ends in 5 days (2025-07-24 15:00 UTC)
```

## 🎯 What It Monitors

| Service | Description |
|---------|-------------|
| **Fortnite** | Battle Royale game status |
| **Epic Games Store** | Store and launcher functionality |
| **Login/Authentication** | Account services |
| **Easy Anti-Cheat (EAC)** | Anti-cheat system status |
| **Matchmaking** | Game matchmaking services |
| **Friends & Social** | Social features |
| **Downloads** | Game downloads and updates |
| **Payment Processing** | Purchase and payment systems |

## 🛠 Requirements

- **Python 3.7+**
- **requests** (HTTP library)
- **colorama** (Terminal colors)

All dependencies are listed in `requirements.txt`.

## 🔧 Configuration

The monitor automatically detects service status using Epic Games' official status API endpoints:

- System Status: `status.epicgames.com/api/v2/summary.json`
- Incidents: `status.epicgames.com/api/v2/incidents.json`
- Free Games: Epic Store backend API

## 🎨 Status Indicators

| Status | Indicator | Description |
|--------|-----------|-------------|
| ✅ **Operational** | `OPERATIONAL` | Everything working normally |
| ⚠️ **Degraded** | `DEGRADED PERFORMANCE` | Slower than usual |
| ❌ **Partial Outage** | `*** WARNING: PARTIAL OUTAGE ***` | Some features down |
| 🚨 **Major Outage** | `*** CRITICAL: MAJOR OUTAGE ***` | Service mostly down |
| 🔧 **Maintenance** | `MAINTENANCE` | Scheduled maintenance |

## 📊 API Status

The monitor tracks these Epic Games API endpoints:

- ✅ **Summary API** - Overall system status
- ✅ **Status API** - Current service status
- ✅ **Incidents API** - Active incidents
- ✅ **Components API** - Individual service components
- ✅ **Free Games API** - Store promotions

## 🎁 Free Games Tracking

- **Current Freebies** - Games available now
- **Countdown Timers** - Time remaining to claim
- **Upcoming Games** - Next week's free games
- **Promotion Details** - Game descriptions and end dates

## 🚨 Incident Monitoring

- **Active Incidents** - Current issues affecting services
- **Impact Levels** - Critical, Major, Minor classifications
- **Recent Updates** - Latest status updates from Epic
- **EAC-Specific Issues** - Anti-cheat related problems

## 🤝 Contributing

Contributions are welcome! Feel free to:

- 🐛 Report bugs
- 💡 Suggest features
- 🔧 Submit pull requests
- 📖 Improve documentation

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This tool uses Epic Games' public status APIs and is not affiliated with Epic Games. Use responsibly and respect API rate limits.

## 🆘 Troubleshooting

### Common Issues

**Connection Errors:**
```bash
# Check your internet connection
ping status.epicgames.com
```

**Python Version:**
```bash
# Verify Python 3.7+
python3 --version
```

**Missing Dependencies:**
```bash
# Reinstall requirements
pip install -r requirements.txt --force-reinstall
```

### Getting Help

If you encounter issues:

1. Check the [Issues](https://github.com/ynwglobal/epic-games-status-monitor/issues) page
2. Run with `--once` flag to test basic functionality
3. Verify your Python and pip versions
4. Check internet connectivity to Epic's APIs

## 🙏 Acknowledgments

- Epic Games for providing public status APIs
- The Python community for excellent libraries
- Contributors who help improve this tool

---

**Made with ❤️ for the Epic Games community**

⭐ **Star this repo if it helps you track Epic Games status!** ⭐
