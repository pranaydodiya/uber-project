# 🚖 Uber Clone – Real-Time Ride Booking App

A modern, full-stack Uber-like ride-booking application that connects riders with nearby captains (drivers), featuring real-time geolocation, ride tracking, Google Maps integration, secure authentication, and a clean, responsive UI for both users and captains.

---

## 🔗 Live Demo

🌐 [View Live App](https://your-deployment-link.com)

---

## 🧠 Overview

This Uber Clone simulates the core functionality of a real-world ride-hailing app. Built with scalable backend architecture, efficient API handling, and modern React UI, it enables users to book rides and captains to accept and complete them in real-time.

---

## ⚙️ Features

### ✅ User Side:
- Signup/Login with JWT
- Profile view and logout
- Location search with Google Places API
- View nearby available captains
- Request a ride and track driver location
- Fare and ETA estimation

### ✅ Captain Side:
- Register/Login with authentication
- Toggle availability (online/offline)
- View ride requests and accept/reject
- Navigate to user’s pickup and drop location
- Real-time ride status updates

### ✅ Shared:
- Google Maps route rendering
- Distance & duration calculation using Directions API
- Socket.IO for real-time updates
- Protected routes with auth middleware
- Clean and mobile-responsive UI

---

## 🛠️ Tech Stack

| Layer       | Tech Used |
|-------------|------------|
| Frontend    | React.js, Tailwind CSS, Google Maps API |
| Backend     | Node.js, Express.js, MongoDB, Mongoose |
| Real-Time   | Socket.IO |
| Auth        | JWT, Bcrypt |
| Dev Tools   | Postman, VS Code, Git, Vercel/Render |

---

## 🔐 Authentication & Authorization

- JWT-based secure login for both roles (User and Captain)
- Passwords hashed using Bcrypt
- Protected API routes with custom middleware
- Role-based access in frontend navigation

---

## 🗺️ Google Maps Integration

- Location Autocomplete (Google Places)
- Real-time coordinate fetching
- Distance & time estimates
- Route drawing between pickup and drop

---

## 🚦 Ride Lifecycle

1. **User Requests Ride** → Captains notified
2. **Captain Accepts** → User gets assigned captain
3. **Captain En Route** → Real-time movement on map
4. **Ride Starts & Ends** → Status updated, ride saved in DB

---

## 🧾 API Structure

All APIs follow RESTful conventions and return JSON. Includes:
- `/api/user` – User registration/login/profile
- `/api/captain` – Captain registration/login/profile
- `/api/rides` – Ride creation, updates, and status control
- `/api/maps` – Geocoding, directions, distance matrix

---



---

## 🚀 Getting Started

### Backend Setup
```bash
cd backend
npm install
# Configure .env with MONGO_URI, JWT_SECRET
npm run dev

cd frontend
npm install
# Configure .env with REACT_APP_GOOGLE_MAPS_API_KEY
npm start

