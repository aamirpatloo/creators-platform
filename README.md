# Fullstack Creators Platform

Simple full-stack creator-focused social platform (React + Express + MongoDB + Socket.IO).

## 🧩 Project structure

- `client/`: React frontend (Vite, React Router, API and socket services, auth context).
- `server/`: Express backend (REST routes for auth/users/posts, image upload, JWT auth, sockets).

## ⚙️ Prerequisites

- Node.js 18+ (or compatible)
- npm
- MongoDB (local or Atlas)

## 🚀 Run locally

1. Clone repo

```bash
git clone <repo-url>
cd Fullstack Creators-platform
```

2. Install dependencies

```bash
npm install
npm install --prefix server
npm install --prefix client
```

3. Create server `.env` file

```
PORT=5000
MONGODB_URI=mongodb+srv://<user>:<pass>@<cluster>.mongodb.net/<db>?retryWrites=true&w=majority
JWT_SECRET=your-secret
CLIENT_URL=http://localhost:5173
```

4. Start app

```bash
npm run dev
```

5. Open frontend

- http://localhost:5173

## 📦 Available scripts

- `npm run dev`: runs server and client with concurrently
- `npm run server --prefix server`: run backend with nodemon
- `npm run client --prefix client`: run Vite front-end

## 🛠 Features

- JWT authentication (register/login)
- CRUD posts with image links (Cloudinary upload integration)
- Real-time updates using Socket.IO
- CORS allowed origins and protected routes

## 🐛 Troubleshooting

- `querySrv ENOTFOUND _mongodb._tcp.xxxx`: check `.env` `MONGODB_URI` and DNS access.
- Ensure `.env` values are correct and server started after dependencies.

## 🙌 License

MIT
