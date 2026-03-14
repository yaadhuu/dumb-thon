# 🧟 DEADZONE

![React](https://img.shields.io/badge/React-18-blue)
![Leaflet](https://img.shields.io/badge/Leaflet-Map-green)
![Hackathon](https://img.shields.io/badge/Event-Dumbathon%202.0-red)
![Status](https://img.shields.io/badge/Status-Prototype-orange)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

Zombie Outbreak Evacuation Navigator
**Hackathon:** Dumbathon 2.0  
**Track:** Web / App Development  

DEADZONE is a real-time emergency evacuation navigation web application built around a simulated zombie outbreak scenario. The project demonstrates how real-world navigation technologies such as GPS tracking and route optimization can be combined with interactive mechanics to create an engaging crisis navigation system.

The application integrates real-time geolocation, live route calculation, and an interactive map interface. Users navigate through a fictional outbreak environment while interacting with system challenges that simulate a compromised emergency navigation network.

---

# 📌 Project Overview

DEADZONE explores the concept of a corrupted emergency GPS system operating during a large-scale disaster.

Instead of functioning normally, the navigation system intentionally interferes with user actions. Survivors must overcome interactive challenges before accessing optimal evacuation routes.

While presented with a zombie apocalypse theme, the system architecture reflects real-world disaster response navigation systems used during floods, fires, and emergency evacuations.

---

# ✅ Hackathon Challenge Implementation

## 1️⃣ Core Application — Map Navigation System

The application includes a fully functional map-based navigation system.

### Features

- Displays the user's real-time GPS location using the **Browser Geolocation API**
- Interactive map interface using **Leaflet**
- Route generation using **OpenRouteService API**
- Displays **danger zones, safe houses, and outbreak markers**
- Provides **live route navigation**

The core functionality remains usable even after all hackathon challenge mechanics are implemented.

---

## 2️⃣ Global Dumb Challenge — Random Popup Interruptions

To simulate emergency broadcast interruptions, the application displays randomized alert messages that interrupt user actions.

### Mechanics

- Every primary action triggers a popup alert
- Actions cannot complete until the popup is dismissed
- Messages are randomly selected from a pool of **15 outbreak transmissions**
- Consecutive popups **never repeat the same message**
- Alerts follow a zombie emergency broadcast theme

---

## 3️⃣ App Specific Challenge — Paranoid GPS Routing

The navigation system operates in **Paranoid Mode** by default.

Instead of providing the shortest route, the system deliberately generates a path significantly longer than the optimal route.

### Paranoid Mode Behavior

- Default route is approximately **10× longer than optimal**
- Route appears with a **glitch-style visual indicator**
- The system periodically reactivates paranoid routing

Users must complete a rhythm-based interaction to restore normal routing.

---

# 🗺 Features

## Boot Screen

The application begins with a **terminal-style boot sequence** simulating an emergency crisis system startup.  
Typewriter-style loading messages establish the outbreak scenario before the map interface loads.

---

## Interactive Outbreak Map

The map displays several elements relevant to evacuation planning.

- 📍 User GPS location marker
- 🔴 Infected danger zones
- 🏥 Safe houses (bunkers, hospitals, supply depots)
- 💀 Zombie horde locations
- 🛣️ Live route visualization

---

## Rhythm Hack Mechanic

To temporarily restore optimal routing, users must perform a rhythmic interaction.

### Mechanic Details

- Tap the **Reboot GPS** button **5 times**
- Tap timing must remain within **300ms consistency**
- Successful rhythm input reboots the GPS system
- Optimal routing remains active for **60 seconds**
- After 60 seconds, **Paranoid Mode automatically returns**

---

# 🛠 Tech Stack

| Technology | Purpose |
|-----------|---------|
| React 18 | Frontend framework |
| Leaflet.js | Interactive map rendering |
| React-Leaflet | React integration for Leaflet |
| OpenRouteService API | Route calculation |
| Axios | API requests |
| Browser Geolocation API | Real-time GPS tracking |

---



 DEMO

 
