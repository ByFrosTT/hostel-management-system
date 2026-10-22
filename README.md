# Hostel Management System

A college MERN project for hostel room management, student registration, room allocation and fee tracking. Includes visitor, movement and leave interfaces.

## Run locally

Use Node.js compatible with the package engine requirements and a running MongoDB instance.

Backend:

```powershell
cd server
npm install
Copy-Item .env.example .env
npm run dev
```

Set MONGO_URI in server/.env for your database. The backend listens on http://localhost:5000 by default.

Frontend, in a second terminal:

```powershell
cd client
npm install
npm run dev
```

Open the URL printed by Vite.

## Scope

Rooms, students and fees use MongoDB. Visitor, movement and leave records are held in frontend state and reset after reloading. The login UI is a demonstration and needs backend authentication before production use.

## Structure

- client/: React and Vite frontend
- server/: Express API, Mongoose models and database connection

Environment files, dependencies and build output are excluded from version control.
