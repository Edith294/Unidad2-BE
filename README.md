# Ejercicios-Unidad2_Brenda
Ejercicios de estudio clase aplicaciones web orientadas a servicios
# 🚀 API Hub — Collection of Integrated Applications

> A unified web platform integrating 10 APIs in a single interface. Built with **Flask** and **Python**.

![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-2.x-000000?style=flat-square&logo=flask&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)
![APIs](https://img.shields.io/badge/APIs-10-f97316?style=flat-square)

---

## 📸 Preview

<!-- Dashboard screenshot here -->

---

## ✨ Integrated Apps

| App | Description | API |
|-----|-------------|-----|
| 🎵 **Spotify** | Search songs, artists, albums & playlists. 30s preview. | Spotify Web API |
| 🎬 **Movies** | Explore films, trailers, cast & recommendations. | TMDB API |
| 🌤️ **Weather** | Real-time weather for your current location. | OpenWeather API |
| 💱 **Currency** | Convert between currencies with live rates. | ExchangeRate API |
| 💻 **GitHub** | Search users, repos & explore open source. | GitHub API |
| 📚 **Books** | Find books, reviews & previews. | Google Books API |
| 📍 **Places** | Locate nearby restaurants, hospitals & services. | OpenStreetMap API |
| 🛍️ **Products** | Full CRUD inventory management system. | SQLite |
| 🤖 **Reddit** | Explore trending posts & subreddits. | Reddit API |
| 💬 **Chat** | Real-time chat powered by Firebase. | Firebase Realtime DB |

---

## 📋 Prerequisites

- Python 3.8+
- `pip` package manager
- `git`
- API keys for: Spotify, TMDB, OpenWeather, ExchangeRate, Firebase

---

## ⚡ Quick Start

**1. Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/api-hub.git
cd api-hub
```

**2. Create virtual environment**
```bash
python -m venv venv

# Windows:
venv\Scripts\activate

# Mac/Linux:
source venv/bin/activate
```

**3. Install dependencies**
```bash
pip install -r requirements.txt
```

**4. Configure environment variables**
```bash
cp .env.example .env
```

Edit `.env` and add your keys:
```env
SPOTIFY_CLIENT_ID=your_client_id
SPOTIFY_CLIENT_SECRET=your_client_secret
TMDB_API_KEY=your_api_key
WEATHER_API_KEY=your_api_key
EXCHANGE_API_KEY=your_api_key
```

**5. Run the app**
```bash
python app.py
```

**6. Open in browser → [http://127.0.0.1:5000](http://127.0.0.1:5000)**

---

## 📁 Project Structure

```
api-hub/
│
├── app.py                  # Main application entry point
├── spotify_app.py          # Spotify module
├── peliculas_app.py        # Movies module
├── clima_app.py            # Weather module
├── divisas_app.py          # Currency module
├── github_app.py           # GitHub module
├── libros_app.py           # Books module
├── lugares_app.py          # Places module
├── productos_api.py        # Products CRUD module
├── reddit_app.py           # Reddit module
├── chat_app.py             # Chat module
│
├── templates/              # HTML templates
├── static/                 # CSS, JS, images
├── requirements.txt
├── .env.example
└── productos.db            # Auto-generated SQLite DB
```

---

## 🔌 API Endpoints

<details>
<summary><strong>🎵 Spotify</strong></summary>

```
GET /api/spotify/buscar?q={query}&tipo={track|artist|album|playlist}
GET /api/spotify/artista/<artist_id>
GET /api/spotify/album/<album_id>
```
</details>

<details>
<summary><strong>🎬 Movies</strong></summary>

```
GET /api/peliculas/buscar?q={query}
GET /api/peliculas/<movie_id>
GET /api/peliculas/populares
```
</details>

<details>
<summary><strong>🌤️ Weather</strong></summary>

```
GET /api/clima
```
</details>

<details>
<summary><strong>💱 Currency</strong></summary>

```
GET /api/divisas/convertir?monto={amount}&de={from}&a={to}
GET /api/divisas/monedas
```
</details>

<details>
<summary><strong>💻 GitHub</strong></summary>

```
GET /api/github/usuario/<username>
GET /api/github/buscar/repos?q={query}
```
</details>

<details>
<summary><strong>📚 Books</strong></summary>

```
GET /api/libros/buscar?q={query}
```
</details>

<details>
<summary><strong>🤖 Reddit</strong></summary>

```
GET /api/reddit/posts?subreddit={name}&filtro={hot|new|top}
GET /api/reddit/subreddits/populares
```
</details>

<details>
<summary><strong>🛍️ Products (CRUD)</strong></summary>

```
GET    /api/productos          # List all
GET    /api/productos/<id>     # Get one
POST   /api/productos          # Create
PUT    /api/productos/<id>     # Update
DELETE /api/productos/<id>     # Delete
```
</details>

<details>
<summary><strong>📍 Places</strong></summary>

```
GET /api/lugares?lat={lat}&lon={lon}&tipo={restaurant|hospital|cafe}
```
</details>

---

## 📱 App Screenshots

### 🎵 Spotify
<img width="1899" height="972" alt="image" src="https://github.com/user-attachments/assets/2401e912-8a07-4ca8-8ff4-d71c0bcaed45" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a230ba3f-4088-4393-9d3b-e3ce164484ab" />


### 🎬 Movies
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/c5aaf7ac-f42e-45fe-90c1-8edd5c309ca9" />
<img width="1915" height="1006" alt="image" src="https://github.com/user-attachments/assets/b28e46cb-cbe0-4260-9a3f-1a847b31ea33" />


### 🌤️ Weather
<img width="1919" height="1020" alt="image" src="https://github.com/user-attachments/assets/f10a2948-ceb3-480a-bc02-162c3ed37a1e" />
<img width="1919" height="1009" alt="image" src="https://github.com/user-attachments/assets/536a8368-a6ff-4759-9d94-e7e15b5fd25b" />


### 💱 Currency
<img width="1905" height="950" alt="image" src="https://github.com/user-attachments/assets/6e99128a-9d45-47d9-b036-c590a9c0acf9" />


### 💻 GitHub
<img width="1908" height="970" alt="image" src="https://github.com/user-attachments/assets/15450ab3-1bca-43fd-9e05-4b30edd30dff" />


### 📚 Books
<img width="1919" height="966" alt="image" src="https://github.com/user-attachments/assets/c1a864b2-78e9-4214-bc3a-06ea9c1afa6e" />
<img width="1919" height="961" alt="image" src="https://github.com/user-attachments/assets/4fcfa5bd-db85-4a5f-a51e-de3ae11017fe" />


### 📍 Places
<img width="1919" height="960" alt="image" src="https://github.com/user-attachments/assets/a30f2af8-3457-49cd-bdd7-ab8de4742bc5" />


### 🛍️ Products
<img width="1908" height="967" alt="image" src="https://github.com/user-attachments/assets/6f24f595-88dc-4d7d-a6ec-1aa396ceb7c8" />


### 🤖 Reddit
<img width="1919" height="974" alt="image" src="https://github.com/user-attachments/assets/8aad2495-a5a2-486e-969f-13ea3162b988" />


### 💬 Chat
<img width="1915" height="964" alt="image" src="https://github.com/user-attachments/assets/8bff1c7d-c0b5-40db-a4bc-43019c5f9596" />


---

## 🛠️ Tech Stack

**Backend** — Python, Flask, SQLite

**Frontend** — HTML5, CSS3, JavaScript

**External Services** — Spotify API · TMDB · OpenWeather · ExchangeRate · GitHub API · Google Books · Reddit API · Firebase · OpenStreetMap

---

## 🗺️ Roadmap

**✅ Phase 1 — Complete**
- 10 integrated APIs
- Unified dashboard
- CRUD system with SQLite
- Real-time chat with Firebase

**🚧 Phase 2 — In Progress**
- User authentication
- Favorites & personal lists
- Dark mode
- Global search across all apps

**📅 Phase 3 — Future**
- Mobile app with React Native
- Push notifications
- Docker containerization
- Admin panel

---

## ⚠️ Important Notes

> **Security:** Never push your `.env` file to GitHub. Use `.env.example` as a template and keep all API keys private.

**Free tier API limits:**

| Service | Limit |
|---------|-------|
| Spotify | 1,000 req/day |
| TMDB | 1,000 req/day |
| OpenWeather | 1,000 req/day |
| ExchangeRate | 1,500 req/month |

---

## 🤝 Contributing

1. Fork the project
2. Create your branch: `git checkout -b feature/new-feature`
3. Commit your changes: `git commit -m 'Add: amazing new feature'`
4. Push to the branch: `git push origin feature/new-feature`
5. Open a Pull Request

**Guidelines:** Write clean, documented code · Follow existing style · Test before submitting · Describe your changes clearly.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

Made with ❤️ and ☕ by **Marlon Rojas**

⭐ If this project helped you, give it a star on GitHub!

</div>
