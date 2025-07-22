# SmartUnlock

A smart, secure, and AI-enhanced door access system built using ESP32-CAM.  
The project integrates face detection, emotion tracking, Telegram alerts, keypad unlocking, and smart automation — designed for modern homes and safety-focused environments.

---

## 🔧 Features

- 📸 **Face Detection** using ESP32-CAM
- 😊 **Emotion Recognition** (smile, neutral, angry, etc.)
- 🚪 **Door Unlock via Telegram Bot**
- 🔢 **4x4 Keypad Unlock** with dynamic password (Google Authenticator support)
- 🚨 **Unknown Face or Covered Face Alert**
- 🚶‍♂️ **Motion-Triggered Alerts** without pressing doorbell
- 🌗 **Smart Light Control** for low-light camera visibility
- 🧲 **Reed Switch** to detect door open/close state
- 🆘 **SOS Button** in Telegram for emergency alert
- 🔐 **Local Manual Unlock** via physical button (in case of network failure)

---

## 🛠️ Hardware Components

- ESP32-CAM
- FTDI Programmer
- 4x4 Matrix Keypad
- Relay Module (2x)
- Reed Switch + Magnet
- Push Button
- LED Light (5V)
- Motion Detection via ESP32-CAM
- PCF8575 (I/O Expander)
- Buck Converter (24V to 5V)
- Power Adapter (24V)
- Wires, soldering, connectors, enclosure

---

## 🧠 Software Stack

- Arduino IDE (ESP32 Board)
- C/C++ (Arduino Sketch)
- Telegram Bot API
- Face & Emotion Detection (ESP32 AI capability)
- Optional: Google Authenticator-compatible time-based passwords

---

## 📲 How It Works

1. **Motion Detected / Bell Pressed**
2. ESP32 captures image → runs face detection
3. Image + emotion sent to Telegram bot
4. If known person → Unlock via button in chat
5. If covered face → Alert sent
6. Keypad can unlock with rotating password
7. Smart LED turns ON in dark for better visibility

---

