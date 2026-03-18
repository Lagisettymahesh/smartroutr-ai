# SmartRoute AI — Complete File Guide
## AI Traffic Prediction & Route Optimization · Bengaluru

---

## YOUR KEY FILES (Use These)

| File | What it is | How to use |
|------|-----------|-----------|
| `smartroute_final.html` | ✅ MAIN FRONTEND | Double-click to open in Chrome |
| `smartroute_backend.py` | ✅ MAIN BACKEND | Run with uvicorn |
| `requirements.txt` | Python packages | pip install -r requirements.txt |
| `.env.example` | API key config | Copy to .env, add your keys |

---

Quick Start (2 steps)

Step 1 — Run Backend
```bash
pip install fastapi uvicorn requests python-dotenv
uvicorn smartroute_backend:app --reload --port 8000
```
Visit: http://localhost:8000/docs

Step 2 — Open Frontend
Double-click `smartroute_final.html` in Chrome

---

✅ Features

- 🗺 Real map (OpenStreetMap — FREE, no API key needed)
- 📍 GPS current location with pulsing dot
- 🔍 Instant autocomplete from first letter (S → Silk Board)
- 🛣 Up to 5 routes — all drawn on map in different colors
- ⚡ Shortest route selected by default
- 🚦 Live traffic layer (red/orange/green roads)
- 🔊 Voice navigation (Chrome built-in, Indian English)
- 📋 Turn-by-turn directions panel on map
- 🤖 Azure ML 10-min traffic prediction
- ⚠️ 10km radius traffic alert from your location
- 🏛 Authority dashboard with hotspots
- 📊 Historical peak hour analysis

---

🔑 Get Google Maps API Key (optional — for better routing)

1. Go to https://console.cloud.google.com
2. Create project → Enable: Maps JS API + Directions API + Places API
3. Credentials → Create API Key → Copy it
4. Open smartroute_final.html in VS Code → find YOUR_API_KEY → replace it

---

🔗 Backend API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| / | GET | Platform status |
| /api/routes | POST | Find routes (supports GPS coords) |
| /api/traffic/live | GET | Live congestion all corridors |
| /api/traffic/predict/{id} | GET | 10-min AI prediction |
| /api/traffic/hotspots | GET | Map hotspot markers |
| /api/traffic/nearby | POST | 10km GPS traffic check |
| /api/voice/instruction | POST | Build voice sentence |
| /api/voice/announcement/{type} | GET | Pre-built announcements |
| /api/analytics/peak | GET | Peak hour analysis |
| /api/nudge/send | POST | Send commuter nudge |
| /api/alerts | GET | Live alert feed |
| /api/stats | GET | Dashboard KPIs |
| /docs | GET | Interactive API documentation |

---

SDG 11 — Sustainable Cities | SDG 9 — Innovation & Infrastructure
Azure IoT Hub · Azure ML · Bengaluru Smart City Platform
---

SDG 11 — Sustainable Cities | SDG 9 — Innovation & Infrastructure  
Azure IoT Hub · Azure ML · Bengaluru Smart City Platform  

---

## 📚 Research & References

### 🔗 Technologies & Tools
- OpenStreetMap — https://www.openstreetmap.org  
- Google Maps Platform — https://developers.google.com/maps  
- FastAPI — https://fastapi.tiangolo.com  
- Leaflet.js — https://leafletjs.com  
- Azure Machine Learning — https://azure.microsoft.com  

### 📊 Research Basis
- Bengaluru traffic congestion patterns  
- Peak hour traffic analysis  
- AI-based traffic prediction models  

### 📖 Note
This project uses publicly available tools and simulated data for demonstration purposes.
