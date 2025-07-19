
# 🎬 Movie Recommendation App

A Fullstack Movie Recommendation Web App that lets users discover, search, and save movies using the **TMDB API**, with features like authentication, favorites, watchlist management, and a personal profile page.

This project was built as a **3MTT Month 4 Capstone** under the "Fullstack Integration & Deployment" track.

---

## 📁 Project Structure

```
movie-recommendation-app/
├── frontend/       # React + Tailwind frontend
├── backend/        # Express.js + MongoDB backend
└── README.md       # Project documentation
```

---

## 🔗 Live Demo

- **Frontend (Netlify)**: [https://zesty-cuchufli-a09284.netlify.app/](https://zesty-cuchufli-a09284.netlify.app/)
- **Backend (Render)**: [https://capstone-back-end-1-bbvp.onrender.com/](https://capstone-back-end-1-bbvp.onrender.com/)

---

## 🚀 Features

### 🔐 Authentication
- Register and login with JWT-based authentication
- Secure protected routes for logged-in users

### 🎥 Movie Discovery
- Search movies via [TMDB API](https://www.themoviedb.org/)
- View detailed movie information
- Discover popular movies and new releases

### ❤️ Favorites & Watchlist
- Save favorite movies to your profile
- Add movies to your personal **watchlist**
- View and manage watchlist items

### 👤 Profile Page
- View basic user profile (username, email)
- Access your saved movies and watchlist

---

## 🧠 Backend Overview

- RESTful API built with **Express.js**
- MongoDB for persistent user, favorites, and watchlist storage
- JWT authentication with secure tokens
- Modular route and controller structure

---

## 🛠️ Technologies Used

### Frontend
- React.js (Hooks)
- Axios for API calls
- React Router DOM
- Tailwind CSS

### Backend
- Node.js + Express.js
- MongoDB + Mongoose
- JSON Web Token (JWT)
- Dotenv for environment config

---

## 📦 How to Run the Project Locally

### 🔧 1. Clone the Repository

```bash
git clone https://github.com/your-username/movie-recommendation-app.git
cd movie-recommendation-app
```

---

### ⚙️ 2. Setup the Backend

```bash
cd backend
npm install
```

Create a `.env` file in `/backend`:

```env
PORT=5000
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/movieApp
JWT_SECRET=your_jwt_secret
TMDB_API_KEY=your_tmdb_api_key
```

Start the server:

```bash
npm run dev
```

---

### 💻 3. Setup the Frontend

```bash
cd ../frontend
npm install
npm start
```

> Make sure to update the Axios base URL in your frontend for API calls (e.g., using `.env`).

---

## 🌐 Deployment Notes

- **Frontend**: Hosted on **Netlify**
- **Backend**: Hosted on **Render**
- **Environment Variables**: Configured securely via each platform's settings

---

## 🧪 API Endpoints

### 🔒 Auth
| Method | Endpoint              | Description           |
|--------|-----------------------|-----------------------|
| POST   | `/api/users/register` | Register a user       |
| POST   | `/api/users/login`    | Authenticate a user   |

### 🎬 Movies
| Method | Endpoint             | Description                |
|--------|----------------------|----------------------------|
| GET    | `/api/movies/search` | Search for movies (TMDB)   |

### ❤️ Favorites
| Method | Endpoint           | Description                |
|--------|--------------------|----------------------------|
| GET    | `/api/favorites`   | Get user favorites         |
| POST   | `/api/favorites`   | Add a favorite movie       |
| DELETE | `/api/favorites/:id` | Remove favorite movie     |

### 📺 Watchlist
| Method | Endpoint            | Description                |
|--------|---------------------|----------------------------|
| GET    | `/api/watchlist`    | Get user watchlist         |
| POST   | `/api/watchlist`    | Add to watchlist           |
| DELETE | `/api/watchlist/:id`| Remove from watchlist      |

---

## 👨‍💻 Author

**Olayemi Lawal**  
GitHub: [@your-github-username](https://github.com/your-github-username)  
3MTT Cohort 3 – Month 4 Capstone Project

---

## 📄 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
