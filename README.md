# Cybersecurity-Project


# 🔍 WiFi Network Scanner

A simple, cross-platform desktop application to scan and display nearby Wi-Fi networks with their signal strength using a graphical interface. Built with **Python** and **Tkinter**, this tool supports **Windows** and **Linux** environments.

## 🧰 Features

* 📡 Scans available Wi-Fi networks in real-time
* 📶 Displays SSID and signal strength (%) in a user-friendly table
* 🖱️ Allows users to click and highlight a preferred network
* 🌐 Cross-platform: Works on **Windows** and **Linux**
* 🎨 Clean and modern UI with Tkinter

## 📸 Screenshot

*(Insert a screenshot of the app here if you have one)*

## 🚀 Getting Started

### ✅ Prerequisites

* Python 3.6 or newer
* Platform:

  * **Windows**: Uses `netsh` command
  * **Linux**: Uses `nmcli` command

### 📦 Installation

1. **Clone the repository** or download the script:

   ```bash
   git clone https://github.com/your-username/wifi-scanner.git
   cd wifi-scanner
   ```

2. **Install required dependencies**

   ```bash
   pip install tk
   ```

   > Note: Tkinter is usually bundled with Python. If not, install it manually (`sudo apt install python3-tk` on Debian-based Linux).

3. **Run the app**

   ```bash
   python wifi_scanner.py
   ```

## ⚙️ How It Works

* **Windows**: Runs `netsh wlan show networks mode=Bssid` to fetch SSID and signal info.
* **Linux**: Uses `nmcli -t -f SSID,SIGNAL dev wifi` to get network data.
* Extracted information is displayed in a GUI using `ttk.Treeview`.


## ❗ Limitations

* macOS is not supported in this version.
* Doesn’t auto-connect to networks (only scans and displays info).
* Requires that `netsh` (Windows) or `nmcli` (Linux) is available in PATH.

## 📄 License

MIT License. See `LICENSE` file for more details.

