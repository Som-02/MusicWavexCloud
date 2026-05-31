# 🎵 MusicWave x Cloud

A full-stack music streaming web application that lets users browse songs and albums by artist, manage playlists, and enjoy a seamless listening experience — powered by a Node.js backend and deployed across Netlify and Render.

**🌐 Live Demo →** [music-wavex-cloud.netlify.app]((https://musicxsomxwave.netlify.app/))

---

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Environment Variables](#environment-variables)
- [Running Locally](#running-locally)
- [Deployment](#deployment)
- [Contributing](#contributing)

---

## ✨ Features

- 🎧 **Music Player** — Play songs directly in the browser with a built-in audio player
- 🎤 **Artist Pages** — Dedicated pages for artists including Arijit Singh, Adele, Ed Sheeran, Diljit Dosanjh, Shreya Ghoshal, Sonu Nigam, Shaan, Zayn, and more
- 💿 **Album Pages** — Browse albums by movie/collection (Jawan, Shershaah, Rockstar, YJHD, Veer-Zaara, etc.)
- 📋 **Playlist Management** — Create and manage personal playlists
- 🔐 **User Authentication** — Login/signup functionality with session handling
- 📬 **Contact Page** — User-facing contact form
- ☁️ **Cloud Deployed** — Frontend on Netlify, backend API on Render

---

## 🛠 Tech Stack

| Layer      | Technology                              |
|------------|-----------------------------------------|
| Frontend   | HTML5, CSS3, Vanilla JavaScript         |
| Backend    | Node.js, Express.js (ES Modules)        |
| Database   | MongoDB (via Mongoose)                  |
| Auth/Misc  | CORS, dotenv                            |
| Hosting    | Netlify (frontend), Render (backend)    |

---

## 📁 Project Structure

```
MusicWavexCloud/
├── songs/               # Audio files
├── album/               # Album art and assets
├── index.html           # Home / landing page
├── newlogin.html        # Login & signup page
├── playlist.html        # Playlist management page
├── showall.html         # Browse all songs
├── contactus.html       # Contact form page
│
├── arijitsingh.html     # Artist pages
├── adele.html
├── edsheeran.html
├── diljit.html
├── shreyaghoshal.html
├── sonunigam.html
├── shaan.html
├── zayn.html
├── shawn.html
├── anuv.html
│
├── jawan.html           # Album / movie soundtrack pages
├── shershaah.html
├── rockstar.html
├── yjhd.html
├── veerzara.html
├── okjaanu.html
├── jabwemet.html
├── bhoolbhulaiya.html
├── ghajini.html
├── adhm.html
│
├── wave.css             # Main stylesheet
├── data.js              # Song/artist data
├── data2.js             # Additional data
├── server.js            # Express backend entry point
├── package.json
└── .env                 # Environment variables (not committed)
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [npm](https://www.npmjs.com/)
- A [MongoDB](https://www.mongodb.com/) database (MongoDB Atlas recommended)

### Clone the Repository

```bash
git clone https://github.com/Som-02/MusicWavexCloud.git
cd MusicWavexCloud
```

---

## 🔑 Environment Variables

Create a `.env` file in the root directory:

```env
MONGO_URI=your_mongodb_connection_string
PORT=5000
```

> ⚠️ Never commit your `.env` file. Keep it in `.gitignore`.

---

## 🏃 Running Locally

### Install dependencies and start the backend

```bash
npm install
npm start
```

The Express server will start at `http://localhost:5000`.

### Open the frontend

Since the frontend is plain HTML, just open `index.html` directly in your browser, or use a local server like [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code.

> Make sure to update any API URLs in your JS files to point to `http://localhost:5000` when running locally.

---

## ☁️ Deployment

This project uses a split deployment setup:

### Frontend — Netlify

1. Push your code to GitHub
2. Connect the repository on [netlify.com](https://app.netlify.com)
3. Set the **publish directory** to `/` (root, since it's plain HTML)
4. Deploy — Netlify will serve your HTML/CSS/JS files globally via CDN

### Backend — Render

1. Connect the repository on [render.com](https://render.com)
2. Create a new **Web Service**
3. Set the **start command** to `npm start`
4. Add your environment variables (`MONGO_URI`, `PORT`) under the Environment tab
5. Deploy — Render will host your Express + MongoDB API

> 💡 After deploying the backend, update your frontend's API base URL to point to your Render service URL (e.g. `https://your-app.onrender.com`).

---

## 🤝 Contributing

Contributions are welcome! To get started:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m "Add: your feature description"`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

<div align="center">
  Made with 🎶 by <a href="https://github.com/Som-02">Somnath</a>
</div>
