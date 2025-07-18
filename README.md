
# 🎬 Movie Recommendation App

This is a Fullstack Movie Recommendation Web Application that allows users to search for movies, view details, and save their favorite picks. It integrates with the **TMDB API** to fetch movie data and uses **MongoDB** to store user information and favorites.

---

## 📁 Project Structure

```
movie-recommendation-app/
├── frontend/       # React frontend
├── backend/        # Express.js + MongoDB backend
└── README.md       # Project documentation
```

---

## 🔗 Live Demo

- **Frontend (Netlify)**: [https://zesty-cuchufli-a09284.netlify.app/] 
- **Backend (Render)**: [https://capstone-back-end-1-bbvp.onrender.com/]

> Replace the URLs above with your actual deployment links.

---

## 🚀 Features

### 🔐 Authentication
- Register and login with secure JWT-based authentication

### 🎥 Movie Features
- Search for movies via [TMDB API](https://www.themoviedb.org/)
- View movie details
- Save favorite movies (for authenticated users)

### 🧠 Backend
- RESTful API using Express.js
- MongoDB + Mongoose for database
- JWT authentication for route protection

---

## 🛠️ Technologies Used

### Frontend
- React.js
- Axios
- React Router
- Tailwind CSS or CSS Modules (depending on your setup)

### Backend
- Node.js
- Express.js
- MongoDB & Mongoose
- JSON Web Token (JWT)
- Dotenv

---

## 📦 How to Run the Project Locally

### 🔧 1. Clone the repository

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

Create a `.env` file and add the following variables:

```env
PORT=5000
MONGO_URI=mongodb+srv://your-username:your-password@cluster.mongodb.net/movieApp?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret
TMDB_API_KEY=your_tmdb_api_key
```

Start the backend:

```bash
npm start
```

---

### 💻 3. Setup the Frontend

```bash
cd ../frontend
npm install
npm start
```

---

## 📂 Deployment Notes

- Frontend is deployed to **Netlify**
- Backend is deployed to **Render**
- Environment variables are securely stored in each platform's settings

---

## 🧪 API Endpoints (Backend)

| Method | Endpoint             | Description                |
|--------|----------------------|----------------------------|
| GET    | `/api/movies/search` | Search movies from TMDB    |
| POST   | `/api/users/register`| Register a new user        |
| POST   | `/api/users/login`   | Authenticate a user        |
| GET    | `/api/favorites`     | Get user favorites (auth)  |
| POST   | `/api/favorites`     | Add favorite movie (auth)  |

---

## 👨‍💻 Author

**Olayemi Lawal**  
GitHub: [@your-github-username](https://github.com/your-github-username)  
3MTT Capstone Project (Month 4) – Fullstack Integration & Deployment

---

## 📄 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
