# Realtime-Device-track

A real-time device tracking app built with Node.js, Express, Socket.IO, and Leaflet.js, allowing you to monitor multiple devices on an interactive map simultaneously.

#Features
Real-time location updates via WebSockets (Socket.IO).

Interactive map using Leaflet.js with OpenStreetMap tiles.

Auto marker management: adds, updates, and removes device markers dynamically as devices connect/disconnect.

Multi-device support with unique client IDs.




#🧩 Tech Stack
Component -	Technology
Backend	- Node.js, Express, Socket.IO
Frontend - HTML, CSS, JavaScript
Mapping	- Leaflet.js, OpenStreetMap
Templating - EJS (if using .ejs views)

#⚙️ Setup Instructions
Clone the repo

git clone https://github.com/SuhelShaikh12/Realtime-Device-track.git
cd Realtime-Device-track


Install dependencies
npm install


Start the server
node app.js

You can also use nodemon for development:
npx nodemon app.js
Open in browser

Navigate to http://localhost:3000 to launch the app.

#🧠 How It Works
Backend
Server Setup: Express serves HTML/EJS pages and static files.

Socket.IO Integration: Listens for client connections and location updates.

Broadcast Updates: When a client sends location data, broadcast it to all connected clients.

Handle Disconnects: Notify clients to remove device markers on disconnect.

Frontend
Geolocation API: Uses browser's geolocation.watchPosition() to track device.

Emit Updates: Sends latitude/longitude to server via Socket.IO.

Map Rendering: Initializes a Leaflet map and clusters device markers.

Live Marker Updates: Adds, updates, or removes markers based on server data.

#🚀 Customization Ideas
Secure with HTTPS – Use SSL for production.

Device metadata – Add custom labels, names, or statuses.

Analytics & history – Store and visualize past routes.

Scalability – Optimize for clusters and larger user bases.

Mobile layout – Improve responsiveness for phones/tablets.

#🛠️ Dependency Overview
Express: Web framework

Socket.IO: WebSockets for live updates

Leaflet.js: Map library

OpenStreetMap: Free map tiles

EJS: Optional templating engine

#✅ Contributing
Open an issue for bugs or feature requests

Fork the repo, create a branch for your feature, then submit a PR

Follow coding standards and add proper documentation or tests

📜 License
This project is open-source. Feel free to use, modify, and distribute under the terms of your chosen license.

