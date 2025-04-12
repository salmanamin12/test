# 🎬 Building a Movie Recommendation System Using Flask and Machine Learning

Are you a movie buff who loves discovering new films? In this blog, I’ll walk you through how I built a **Movie Recommendation System** using **Flask**, **Python**, and **Machine Learning** — and even containerized it with **Docker**!

---

## 🚀 Project Overview

The goal of this project is to recommend similar movies based on a user's selection. It uses a content-based recommendation approach, meaning it suggests movies with similar content (genres, keywords, etc.) rather than relying on user ratings.

---

## 🛠 Tech Stack

- **Python**
- **Flask (Web Framework)**
- **Pandas & NumPy (Data Handling)**
- **Scikit-learn (Machine Learning)**
- **NLTK (Natural Language Processing)**
- **Docker (Containerization)**

---

## 🧠 How It Works

1. **Preprocessed Movie Data**: The dataset contains movie titles, genres, and metadata.
2. **Feature Engineering**: The system creates a similarity matrix using `scikit-learn` to compare movie content.
3. **Model Serialization**: The trained model is saved using `pickle`.
4. **Web Interface**: Users interact with the app via a simple Flask front-end.
5. **Poster Integration**: Movie posters are fetched using the **TMDB API** for a visually rich experience.

---

## 🖼 User Interface

The front-end is built using HTML and Bootstrap. The user selects a movie from the dropdown, and upon submitting, the app displays a list of 20 recommended movies along with their posters.

---

## 🐳 Docker Support

To make deployment easy and consistent, I created a **Dockerfile** to containerize the application. With Docker, this app can run anywhere — your laptop, a server, or the cloud — without any dependency issues.

---

## 🗂 Folder Structure

```
movie-recommender/
├── analysis.ipynb
├── app.py
├── requirements.txt
├── model.pkl
├── similarity.pkl
├── Dockerfile
├── templates/
    └── index.html
└── data/
    ├── tmdb_5000_credits
    └── tmdb_5000_movies
```

---

## ▶ How to Run

### 🔧 Build Docker Image:
```bash
docker build -t movie-recommender .
```

### ▶ Run the Container:
```bash
docker run -p 5000:5000 movie-recommender
```

Then go to `http://localhost:5000` in your browser!

---

## 🎯 Future Improvements

- Add user-based collaborative filtering
- Enable login system and movie rating
- Deploy on a cloud platform like Heroku or AWS

---

## 📌 Final Thoughts

This project is a fun and practical way to apply machine learning in the real world. It combines data processing, recommendation systems, web development, and deployment — all in one package!

If you're interested in the source code or want to try the app yourself, feel free to [contact me](#) or check out the GitHub repo (if available).
