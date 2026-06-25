# ⚡ UltraFastSharing v1.1.0

![Platform: Windows](https://img.shields.io/badge/Platform-Windows-blue.svg)
![License: Proprietary Freeware](https://img.shields.io/badge/License-Proprietary_Freeware-red.svg)
![Offline: 100%](https://img.shields.io/badge/Offline-100%25-orange.svg)

**UltraFastSharing** is a secure, 100% offline, peer-to-peer file transfer utility that bridges the gap between your Windows PC and any mobile device. Built for speed and absolute privacy, it allows you to transfer unlimited file sizes across your local network (Wi-Fi or USB tethering) without ever touching the cloud.

---

## ✨ Key Features

*   **🚫 100% Offline & Private:** No internet connection required. No servers, no cloud logging, and no data caps. Your files never leave your local environment.
*   **🚀 Unlimited File Size:** Send 1000GB+ video files, raw project assets, or entire archives in seconds. The only limit is your hard drive space.
*   **📱 Universal Access (Phone or PC):** No app required on the receiving device. Just scan the QR code on your phone, or type the local IP address into a second PC's web browser, to instantly access the sleek, premium transfer vault.
*   **💻 PC-to-PC Direct Transfer:** Seamlessly send files between two laptops. The receiver gets a glorious 800px wide, glassmorphic desktop web UI! Includes native buttons to instantly trigger Windows Mobile Hotspot or Bluetooth PAN right from the dashboard.
*   **📂 Advanced Vault Controls:** Native support for diving into sub-folders, downloading entire folders instantly (using zero-compression ZIP technology for raw speed), and multi-selecting files for batch downloads.
*   **⚡ Instant Connections:** Lightning-fast server start and stop logic. Sockets are dynamically tracked and destroyed upon closing, ensuring the software is incredibly snappy.
*   **🔌 Universal Connectivity:** Works on traditional home Wi-Fi networks, Mobile Hotspots, direct USB Tethering, Bluetooth Tethering PANs, and hardwired Ethernet/LAN networks seamlessly.

---

## 🛠 How It Works

Traditional file transfer methods (like Google Drive, Dropbox, or email) upload your files to a corporate server and then download them back to your second device. This takes double the time and compromises privacy.

**UltraFastSharing** acts as a local node:
1. It spins up a lightweight `Node.js`/`Express` server locally on your machine.
2. It binds directly to your local IP address (ignoring virtual adapters like Tailscale or VMs).
3. It exposes a beautifully crafted `HTML/CSS` vault UI to the local network.
4. When you upload a file from your phone, it is routed directly over the local network frequencies straight into your PC's storage.

---

## 🔒 Security & Privacy

Privacy is the core philosophy of this tool. 
*   **Zero Telemetry:** There are no analytics, trackers, or middle-men. 
*   **Firewall Sandboxing:** The software operates strictly on local area network protocols. 

*Note: As this tool opens a local port (8080) for file reception, it is recommended to only run the server when actively transferring files, and to only run it on networks you trust.*

---

## 📦 Installation Options

We offer two ways to run UltraFastSharing on your Windows machine:

### 1. The Setup Installer (Recommended)
A full, professional installation perfect for daily use.
1. Download `UltraFastSharing Setup 1.0.0.exe`.
2. Run the installer. It will safely install into your `C:\Program Files` directory.
3. It will automatically create a Desktop and Start Menu shortcut.
4. *Note: Upon first launch, Windows Defender Firewall will ask for network permissions. Ensure the **Public** box is checked so mobile hotspots can connect.*

### 2. The Portable Version
A standalone executable perfect for USB drives or strict environments.
1. Download `UltraFastSharing 1.0.0.exe`.
2. Double-click to run it instantly. No installation required.

---

## 🚀 Usage Guide

1. **Launch the App:** Open UltraFastSharing on your Windows PC.
2. **Start the Server:** Click the toggle to "Active".
3. **Connect Your Phone:** Ensure your phone is connected to the same Wi-Fi network (or your PC is connected to your phone's mobile hotspot).
4. **Access the Vault:** Open your mobile browser and enter the IP address displayed on the PC app (e.g., `http://192.168.1.5:8080`).
5. **Drop Files:** Tap the drop-zone on your phone to select and send files instantly to your PC.

---

## 💻 Built With

*   **[Electron](https://www.electronjs.org/)** - Cross-platform desktop framework
*   **[Node.js](https://nodejs.org/)** - Backend server runtime
*   **[Express.js](https://expressjs.com/)** - Fast, unopinionated web framework
*   **[Formidable](https://github.com/node-formidable/formidable)** - Node.js module for parsing form data and file uploads
*   **Vanilla HTML/CSS/JS** - For a zero-dependency, lightning-fast frontend UI

---

*Crafted with code and coffee.*
