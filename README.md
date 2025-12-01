# Location Tracker


A consent-first Location Tracker platform for sharing live GPS positions between consenting users (family, delivery agents, employees). Built as a full-stack demo with a Node.js/Express backend, MongoDB, and React frontend (Leaflet map + Socket.IO for realtime updates).


> **Important:** This project requires explicit user consent for location sharing. It does not, and will not, support tracking via phone number alone.


## Features
- User registration & authentication (JWT)
- Opt-in location sharing (per-session, revocable)
- Real-time location updates via WebSockets (Socket.IO)
- Map UI (Leaflet) showing live positions
- Role modes: personal, family-sharing, delivery/agent
- Minimal mobile-ready structure (React Native placeholders)
- Basic rate-limiting and permission checks


## Tech stack
- Backend: Node.js, Express, Socket.IO
- Database: MongoDB (Atlas or local)
- Frontend: React + Leaflet + Socket.IO client
- (Optional) Mobile: React Native skeleton


## Quickstart (local)


### Prerequisites
- Node >= 16, npm or pnpm
- MongoDB connection (local or Atlas)


### Backend
```bash
cd backend
cp .env.example .env
# Edit .env to set MONGO_URI and JWT_SECRET
npm install
npm run dev
