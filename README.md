# 📍 Realtime Device Tracker

A real-time device tracking app built with **Node.js**, **Express**, **Socket.IO**, and **Leaflet.js**, allowing you to monitor multiple devices on an interactive map simultaneously.

---

## 🔥 Features

- 📡 **Real-time location updates** via WebSockets (Socket.IO)
- 🗺️ **Interactive map** using Leaflet.js with OpenStreetMap tiles
- 📍 **Auto marker management**: dynamically adds, updates, and removes device markers
- 👥 **Multi-device support** with unique client IDs

---

## 🧩 Tech Stack

| Component   | Technology                        |
|-------------|-----------------------------------|
| Backend     | Node.js, Express, Socket.IO       |
| Frontend    | HTML, CSS, JavaScript             |
| Mapping     | Leaflet.js, OpenStreetMap         |
| Templating  | EJS *(if using `.ejs` views)*     |

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/SuhelShaikh12/Realtime-Device-track.git
cd Realtime-Device-track
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Start the Server

```bash
node app.js
```

Or use `nodemon` for development:

```bash
npx nodemon app.js
```

### 4. Open in Browser

Navigate to:  
**http://localhost:3000**

---

## 🧠 How It Works

### Backend

- ⚙️ **Server Setup**: Express serves HTML/EJS and static assets  
- 🔌 **WebSocket Integration**: Listens for connections via Socket.IO  
- 📤 **Broadcast Updates**: Sends location data to all connected clients  
- ❌ **Handle Disconnects**: Removes markers when a device disconnects  

### Frontend

- 📍 **Geolocation API**: Tracks device using `navigator.geolocation.watchPosition()`  
- 🚀 **Emit Updates**: Sends location data to the server  
- 🗺️ **Map Rendering**: Initializes Leaflet map with markers  
- ♻️ **Live Marker Updates**: Adds/updates/removes markers in real-time  

---

## 🚀 Customization Ideas

- 🔒 Secure the app with **HTTPS/SSL**
- 🏷️ Add **device metadata** like names, status, battery info, etc.
- 📊 Add **analytics/history** to visualize routes and past locations
- ⚡ Optimize for **scalability and clusters**
- 📱 Improve **mobile responsiveness** and UI/UX

---

## 🛠️ Dependency Overview

- **Express** – Web server framework  
- **Socket.IO** – WebSocket communication  
- **Leaflet.js** – Map rendering  
- **OpenStreetMap** – Free tile provider  
- **EJS** – Templating engine (optional)

---

## ✅ Contributing

- 🐛 Open an issue for bugs or feature suggestions
- 🍴 Fork the repo, create a feature branch, and submit a pull request
- 🧼 Follow clean code standards and document your changes

---

## 📜 License

This project is **open-source**. Feel free to use, modify, and distribute it under the terms of your preferred license.
