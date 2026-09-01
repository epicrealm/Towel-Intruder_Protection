# 🧼 Towel Security Suite v1.0.0

[![Platform](https://shields.io)](https://microsoft.com)
[![Language](https://shields.io)](https://github.com)
[![License](https://shields.io)](https://opensource.org)

**Towel** is an on-demand, stealthy, and lightweight endpoint threat containment and anti-intruder protection application suite for your Windows laptop. 

When armed, it completely locks down system inputs locally, blocks unauthorized keystrokes or mouse button clicks from registering to the OS, and triggers silent background tracking. It features a responsive, touch-friendly **Mobile Web Console** allowing you to stream your laptop's screencast, webcam, and room audio live to your phone over Wi-Fi *only* when you manually toggle them on.

---

## 📂 Project Directory Structure

Ensure your directory maintains this exact folder hierarchy before launching:

```text
Towel/
├── start_towel.exe       # Master Launcher Binary (Double-click to start)
├── towel_core.exe        # Core Sleek C++ Dark-Mode Window Controller
├── stop_towel.bat        # Complete System Kill-Switch (Clears all tasks)
├── README.md             # This instruction documentation manual
├── workers/
│   ├── surveillance.py   # Silent local video/audio threat vault logger
│   └── screencast.py     # On-demand phone WebSocket communication engine
└── towel_server/
    ├── server.js         # Local Express Web Broker Node API
    └── public/
        └── index.html    # Responsive touch-friendly Phone Dashboard UI
```

---

## ⚙️ Prerequisites & Installation

Before running the application framework for the first time, your system must have the following dependencies configured:

### 1. Runtimes
* [Node.js](https://nodejs.org) (v18.0.0 or newer recommended)
* [Python](https://python.org) (v3.10 or newer recommended)

### 2. Python Dependencies
Open your standard Command Prompt (`cmd`) and install the required machine surveillance and socket streaming bindings:
```bash
pip install sounddevice scipy numpy opencv-python pillow python-socketio[client] websocket-client
```

### 3. Node.js Dependencies
Navigate directly into your server subfolder and install the core web socket engine:
```bash
cd towel_server
npm install express socket.io
```

---

## 🚦 How To Operate & Test (Same PC)

1. Navigate to your main `Towel` directory folder and double-click **`start_towel.exe`**.
2. The master launcher will automatically sweep lingering tasks, boot up your local node web broker engine invisibly, initialize the capture loops, and display your sleek C++ window.
3. Open any modern desktop web browser and visit the local dashboard pipeline:
   👉 **`http://localhost:3000`** *(The console view remains completely blank to save resources until requested).*
4. Tap **Screencast OFF** on your browser layout. The button turns bright blue, cleanly commanding your laptop to stream live frames to the site.
5. Click **ARM SECURITY** inside your desktop application window. Step away from your laptop. Your normal home screen remains completely visible, but all hardware mouse clicks and typing actions are completely locked out.
6. To safely unlock the physical interface, hold down the **`Ctrl`** key and tap **`D`** (`Ctrl + D`). Your desktop window transforms back to idle mode instantly.

---

## 📱 Running the Wireless Phone Dashboard (Over Wi-Fi)

To monitor your laptop completely remotely while stepping away from your desk:

1. Open your laptop terminal loop (`cmd`), type `ipconfig`, and copy your active **IPv4 Address** (e.g., `192.168.1.15`).
2. Make sure your smartphone is connected to the **exact same Wi-Fi network** as your laptop.
3. Open the web browser (Safari or Chrome) on your phone and type your IP followed by port `:3000`:
   👉 **`http://192.168.1.15:3000`**
4. The dashboard will scale perfectly to fit your portrait smartphone display canvas screen. Tap the large structural controls on your mobile phone screen to watch and listen to your device live!

---

## 🛑 Shutting Down the Application Suite

When you are done utilizing the platform and want to clean all background servers, web nodes, and capture pipelines out of your computer's system memory completely:

👉 Double-click **`stop_towel.bat`** inside your directory window. It will safely terminate all processes.

---

## 🔒 Security & Data Localization Matrix

* **100% Private:** Towel operates entirely locally on your machine infrastructure (`localhost`).
* **Offline Records:** Intruders' structural data packages and recordings are written locally inside the `Intruder_Logs` workspace folder.
* **Zero Leakage:** No metadata, video packages, microphone chunks, or authentication tokens are ever sent to an external third-party server.

---
Developed for public safety. Secure your workspace endpoint environments! 🧼
