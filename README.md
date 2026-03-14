# 🧟 DEADZONE
## Zombie Outbreak Evacuation Navigator
### Built for Dumbathon 2.0 — Apocalypse Protocol | Web/App Development Track

---

## 🚨 What Is DEADZONE?

DEADZONE is a real-time emergency evacuation navigation 
web application built around a zombie outbreak scenario. 
It is a fully functional map application that combines 
real GPS technology, live routing, and interactive 
survival mechanics wrapped in a post-apocalyptic 
military terminal aesthetic.

The core idea: what if GPS systems survived the zombie 
apocalypse but got corrupted and paranoid? DEADZONE 
answers that question by building a navigation system 
that fights back — deliberately misleading survivors, 
interrupting every action with outbreak alerts, and 
forcing users to hack the GPS back to reality every 
60 seconds.

---

## 🎯 Hackathon Requirements Fulfilled

### ✅ Core App — Map Application
- Displays user's real current GPS location
- Provides real route navigation via OpenRouteService API
- Shows infected danger zones, safe houses, and horde 
  locations on an interactive map
- Core functionality remains usable after all dumb 
  challenges are implemented

### ✅ Global Dumb Challenge — Random Popup Interruptions
- Every primary action triggers a random outbreak alert
- Action does NOT complete until popup is dismissed
- Content randomized from pool of 15 unique messages
- No two consecutive popups show the same message
- All messages are zombie apocalypse themed

### ✅ App Specific Challenge — Paranoid GPS Routing
- Default route is 10x longer than the optimal path
- User must tap a rhythmic pattern to restore normal routing
- Paranoid mode automatically reactivates after 60 seconds
- Cannot be permanently disabled — loop continues forever

---

## 🗺️ Features

### Boot Screen
A cinematic military terminal boot sequence with 
typewriter-style loading messages that set the scene 
before the map loads. Feels like booting up a crisis 
system in the middle of an outbreak.

### Interactive Outbreak Map
A fully functional dark-themed map showing:
- 📍 Your real GPS location as a survivor marker
- 🔴 Infected danger zones as red radius circles
- 🏥 Safe houses — bunkers, hospitals, supply depots
- 💀 Zombie horde locations marked across the city
- 🛣️ Real navigable routes fetched from live API

### Paranoid Mode Routing
The GPS is corrupted by default. It routes you along 
a path 10 times longer than optimal — simulating a 
system avoiding infected roads. The route appears as 
a glitchy red dashed line with a pulsing danger border 
around the map.

### Random Popup Interruptions
Every time you try to navigate, reroute, or when 
paranoid mode reactivates — a random zombie outbreak 
transmission interrupts and blocks your action. You 
must read and dismiss the alert before proceeding. 
Messages are randomized from a pool of 15 unique 
zombie-themed broadcasts.

### Rhythm Hack Mechanic
To restore optimal routing the user must tap a REBOOT 
GPS button 5 times in consistent rhythm. The app 
detects timing consistency between taps within 300ms 
tolerance. Success triggers a GPS reboot animation 
and switches the route to a clean green optimal line. 
After 60 seconds paranoid mode automatically kicks 
back in.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| React 18 | Frontend framework and state management |
| Leaflet.js | Interactive map rendering |
| react-leaflet | React wrapper for Leaflet |
| OpenRouteService API | Real world route calculation |
| Axios | API calls |
| Browser Geolocation API | Real GPS coordinates |

---

## 🚀 How To Run

### Prerequisites
- Node.js installed
- OpenRouteService API key (free at openrouteservice.org)

### Setup
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/deadzone.git

# Navigate into project
cd deadzone

# Install dependencies
npm install

# Create .env file and add your API key
echo "REACT_APP_ORS_API_KEY=your_api_key_here" > .env

# Start the app
npm start

# Open in browser
http://localhost:3000
```

---

## 📱 How To Use
```
1. App boots with military terminal loading sequence
2. Map loads centered on your real GPS location
3. Infected zones, safe houses and hordes are visible
4. Enter any evacuation destination in the search bar
5. Click NAVIGATE
6. Dismiss the outbreak alert transmission popup
7. Paranoid route renders — red glitchy 10x longer path
8. Find the TAP TO REBOOT GPS panel
9. Tap the button 5 times in consistent rhythm
10. GPS reboots — optimal green route appears
11. You have 60 seconds before paranoid mode returns
12. Survive as long as you can
```

---

## 🎨 Design Language

DEADZONE uses a military crisis terminal aesthetic:
```
Background:    #0a0a0a  — near black
Primary text:  #00ff41  — terminal green
Danger:        #ff3333  — infected red  
Warning:       #ffaa00  — amber alert
Surface:       #0d0d0d  — dark panel
Font:          monospace throughout
Corners:       sharp — no border radius
Effects:       scanlines, glitch, pulse animations
```

---

## 🧠 Real World Application

Strip away the zombie theme and DEADZONE is a blueprint 
for a real disaster response navigation system:

| DEADZONE Feature | Real World Equivalent |
|-----------------|----------------------|
| Infected zones | Flood zones, fire areas, no-go zones |
| Safe houses | Evacuation centers, hospitals, shelters |
| Emergency popups | Government alert broadcasts |
| Paranoid routing | Worst case safety path planning |
| Rhythm hack | Cognitive check — user is alert and responsive |

---


---

## ⚙️ Environment Variables
```
REACT_APP_ORS_API_KEY = your OpenRouteService API key
Get your free key at: openrouteservice.org
```

---

## 📦 Dependencies
```json
{
  "react": "^18.0.0",
  "react-dom": "^18.0.0",
  "react-leaflet": "^4.0.0",
  "leaflet": "^1.9.0",
  "axios": "^1.0.0"
}
```

---
