<!-- 
SEO Keywords: NullSec Bluetooth, Bluetooth security app, BLE scanner, Bluetooth hacking app,
device discovery, GATT explorer, Bluetooth pentesting, BLE security analyzer,
bad-antics, bad-antics, NullSec Framework, mobile Bluetooth tools, device tracker
-->

<div align="center">

# 🔵 NullSec Bluetooth

### Advanced Bluetooth Security Analyzer

[![Discord](https://img.shields.io/badge/🔑_GET_KEYS-discord.gg/killers-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/killers)
[![GitHub](https://img.shields.io/badge/GitHub-bad--antics-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/bad-antics)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/bad-antics/nullsec-bluetooth)

```
     ▓█████▄  ██▀███   ██▓ ██▓███      ▄▄▄▄   ██▓    ▓█████
     ▒██▀ ██▌▓██ ▒ ██▒▓██▒▓██░  ██▒   ▓█████▄▓██▒    ▓█   ▀
     ░██   █▌▓██ ░▄█ ▒▒██▒▓██░ ██▓▒   ▒██▒ ▄█▒██░    ▒███
     ░▓█▄   ▌▒██▀▀█▄  ░██░▒██▄█▓▒ ▒   ▒██░█▀ ▒██░    ▒▓█  ▄
     ░▒████▓ ░██▓ ▒██▒░██░▒██▒ ░  ░   ░▓█  ▀█░██████▒░▒████
      ▒▒▓  ▒ ░ ▒▓ ░▒▓░░▓  ▒▓▒░ ░  ░   ░▒▓███▀░ ▒░▓  ░░░ ▒░
      ░ ▒  ▒   ░▒ ░ ▒░ ▒ ░░▒ ░        ▒░▒   ░░ ░ ▒  ░ ░ ░
        ░        ░     ░            ░    ░  ░   ░      ░
     ▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄
     █░░ BLE SCANNER ░░░ GATT EXPLORER ░░░ DEVICE TRACKER ░█
     ▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀
                      bad-antics
```

### 🔓 **[Join discord.gg/killers](https://discord.gg/killers)** for premium features!

</div>

---

## 🎯 Features

| Feature | Free | Premium |
|---------|:----:|:-------:|
| 🔍 Device Discovery | ✅ | ✅ |
| 📊 Signal Strength | ✅ | ✅ |
| 📱 Device Classification | ✅ | ✅ |
| 🏭 Manufacturer Lookup | ✅ | ✅ |
| 🔗 GATT Service Explorer | ❌ | ✅ |
| 📡 BLE Advertising Data | ❌ | ✅ |
| 🕵️ Device Tracking | ❌ | ✅ |
| 📈 Signal History | ❌ | ✅ |
| 📋 Export Reports | JSON | All formats |
| 🔔 Proximity Alerts | ❌ | ✅ |
| 🗺️ Device Mapping | ❌ | ✅ |

---

## 📱 Supported Devices

### Bluetooth Classic
- 📱 Smartphones & Tablets
- 💻 Laptops & Computers
- 🎧 Headphones & Earbuds
- 🔊 Speakers & Audio Devices
- 🖱️ Keyboards & Mice
- 🚗 Car Audio Systems
- 🎮 Game Controllers

### Bluetooth Low Energy (BLE)
- ⌚ Smartwatches & Fitness Trackers
- 🏥 Medical Devices
- 🏠 Smart Home Devices
- 🔒 Smart Locks
- 📍 Beacons & Trackers
- 🌡️ Sensors & IoT Devices

---

## 🛡️ Security Analysis

### Device Classification
| Type | Icon | Detection Method |
|------|------|------------------|
| Phone | 📱 | CoD + Name pattern |
| Computer | 💻 | CoD major class |
| Audio | 🎧 | CoD + A2DP service |
| Wearable | ⌚ | BLE services |
| IoT | 🔌 | BLE + unknown CoD |
| Beacon | 📍 | iBeacon/Eddystone |

### GATT Analysis (Premium)
- Service UUID enumeration
- Characteristic discovery
- Security property analysis
- Read/Write permissions check
- Notification capabilities

---

## 📦 Installation

### Android
```bash
# Download from releases or build:
git clone https://github.com/bad-antics/nullsec-bluetooth.git
cd nullsec-bluetooth/android
./gradlew assembleDebug
adb install app/build/outputs/apk/debug/app-debug.apk
