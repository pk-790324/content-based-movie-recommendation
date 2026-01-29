🎬 Content-Based Movie Recommendation System (Deep Learning)

This project implements a content-based movie recommendation system using a two-tower neural network architecture — one model for users and one for movies.

📌 Project Overview

The system learns dense embeddings for users and movies and recommends movies based on similarity in the embedding space.

It supports:

✅ Recommendations for existing users

✅ Recommendations for new users (cold start)

✅ Similar movie search using cosine similarity

🧠 How It Works

User features are passed through a User Neural Network

Movie features are passed through a Movie Neural Network

Both networks produce embeddings of the same dimension

Recommendations are generated using dot product / cosine similarity

Similar movies are found by comparing movie embeddings

🛠 Tech Stack

Python

TensorFlow / Keras

NumPy

Pandas

📂 Features

Two-tower deep learning model

Learned embeddings for personalization

Cosine similarity for movie-to-movie recommendations

Scalable and modular design

🚀 Future Improvements

Add collaborative filtering signals

ANN search (FAISS) for large-scale similarity

Deployment using FastAPI

UI for interactive recommendations

📎 Dataset

MovieLens dataset (or custom movie metadata)

📌 Author

Pappu Yadav
Aspiring Data Scientist / ML Engineer
