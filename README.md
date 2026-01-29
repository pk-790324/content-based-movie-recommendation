# Content-Based Movie Recommendation System (Deep Learning)

A content-based movie recommendation system built with a two-tower neural network: one tower for users and one for movies. The system learns dense embeddings for users and movies and recommends movies by comparing embeddings (dot product / cosine similarity).

---

## Key features

- Two-tower deep learning architecture (user and movie networks)
- Learned dense embeddings for personalization
- Support for:
  - Recommendations for existing users
  - Cold-start recommendations for new users (based on provided features)
  - Finding similar movies using cosine similarity
- Scalable and modular design suitable for iteration and extension

---

## Tech stack

- Python
- TensorFlow / Keras
- NumPy
- Pandas

---
## How it works (high level)

- User features → User Neural Network → user embedding
- Movie features → Movie Neural Network → movie embedding
- Similarity between user and movie embeddings is computed using dot product or cosine similarity to produce ranked recommendations
- For movie-to-movie suggestions, compare movie embeddings using cosine similarity

---

## Typical inputs

- User features: explicit ratings, demographic info, viewing history, or feature-engineered vectors
- Movie features: genres, tags/keywords, textual metadata (title, description), cast/crew, year, etc.
---

## Example workflows

- Recommend for an existing user:
  1. Encode user features
  2. Compute user embedding with the user tower
  3. Rank candidate movies by similarity to the user embedding

- Cold-start (new user):
  1. Build a user profile from available metadata (preferences, demographic, or quick survey)
  2. Use the user tower to produce an embedding from that profile
  3. Rank movies as above

- Similar movies:
  1. Compute or load precomputed movie embeddings
  2. Use cosine similarity to find nearest neighbors in embedding space

---
## Dataset

This project was designed to work with MovieLens or any custom movie metadata dataset. Preprocessing steps depend on the dataset structure; typical tasks include merging rating logs, extracting item features, tokenizing text, and building feature pipelines.

---

## Author

Pappu Yadav  
Aspiring Data Scientist
---
