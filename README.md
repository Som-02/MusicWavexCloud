# 🎵 MusicWavexCloud

A full-stack music streaming web application featuring curated artist pages, album browsing, and a built-in audio player — inspired by Spotify. Built with vanilla HTML/CSS/JS on the frontend and Node.js + Express + MongoDB on the backend, deployed on Vercel.

**Live Demo →** [music-wavex-cloud.vercel.app](https://music-wavex-cloud.vercel.app)

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
- [License](#license)

---

## ✨ Features

- 🎤 **Artist Pages** — Dedicated pages for artists including Arijit Singh, Diljit Dosanjh, Shreya Ghoshal, Sonu Nigam, Anuv Jain, Adele, Ed Sheeran, Shawn Mendes, Zayn, and more
- 🎬 **Album & Playlist Pages** — Browse albums and playlists with a clean card-based UI
- ▶️ **Audio Player** — Play songs directly in the browser with a persistent bottom player bar
- 🎞️ **Movie Soundtracks** — Curated pages for popular Bollywood films (Jawan, Rockstar, Shershaah, YJHD, Bhool Bhulaiyaa, and more)
- 🔐 **User Authentication** — Login page with form handling
- 📬 **Contact Page** — User-facing contact form
- 📱 **Responsive Design** — Works across desktop and mobile viewports

---

## 🛠 Tech Stack

| Layer       | Technology                              |
|-------------|-----------------------------------------|
| Frontend    | HTML5, CSS3, Vanilla JavaScript         |
| Backend     | Node.js, Express.js                     |
| Database    | MongoDB (via Mongoose)                  |
| Environment | dotenv                                  |
| CORS        | cors middleware                         |
| Hosting     | Vercel                                  |

---

## 📁 Project Structure

```
MusicWavexCloud/
├── songs/                  # Audio files (.mp3)
├── album/                  # Album cover images
├── index.html              # Home / landing page
├── playlist.html           # Playlist browser
├── newlogin.html           # Login page
├── contactus.html          # Contact page
│
├── # Artist Pages
├── arijitsingh.html
├── shreyaghoshal.html
├── sonunigam.html
├── diljit.html
├── anuv.html
├── shaan.html
├── adele.html
├── edsheeran.html
├── shawn.html
├── zayn.html
│
├── # Movie / Album Pages
├── rockstar.html
├── shershaah.html
├── jawan.html
├── yjhd.html
├── bhoolbhulaiya.html
├── jabwemet.html
├── okjaanu.html
├── veerzara.html
├── ghajini.html
├── adhm.html
│
├── data.js / data2.js      # Song metadata (title, src, cover)
├── wave.css                # Main stylesheet
├── server.js               # Express backend entry point
├── package.json
└── .env                    # Environment variables (not committed)
```

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [npm](https://www.npmjs.com/)
- A [MongoDB](https://www.mongodb.com/) instance (local or Atlas)

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
PORT=3000
```

> ⚠️ Never commit your `.env` file. Add it to `.gitignore` if not already present.

---

## 🏃 Running Locally

```bash
# Install dependencies
npm install

# Start the backend server
npm start
```

The server will run at `http://localhost:3000`.

Open `index.html` directly in your browser, or serve it with a static server:

```bash
npx serve .
```

---

## ☁️ Deployment

The app is deployed on **Vercel**. To deploy your own fork:

1. Push your code to GitHub
2. Import the repository on [vercel.com](https://vercel.com)
3. Set environment variables (`MONGO_URI`, `PORT`) in the Vercel dashboard
4. Deploy — Vercel will auto-detect the static files and `server.js`

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
  Made with 🎧 by <a href="https://github.com/Som-02">Somnath</a>
</div>
