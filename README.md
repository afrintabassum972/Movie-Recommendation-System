# Movie Recommendation System 🎬

A Content-Based Movie Recommendation System built using Python, Streamlit, and the TMDB dataset. This application suggests five movies similar to a user-selected title, complete with movie posters fetched via the TMDB API.

## 🚀 Features
- **Smart Recommendations:** Recommends 5 similar movies based on content (genres, keywords, cast, etc.).
- **Poster Integration:** Fetches and displays real-time movie posters using the TMDB API.
- **Interactive UI:** Simple and clean web interface built with Streamlit.
- **Fast Search:** Uses precomputed similarity matrices for instant results.

## 🛠️ Tech Stack
- **Language:** Python
- **Web Framework:** Streamlit
- **Data Analysis:** Pandas, NumPy
- **Machine Learning:** Scikit-learn (Cosine Similarity)
- **API:** TMDB (The Movie Database)
- **Storage:** Pickle (for precomputed similarity matrices and movie data)

## 📂 Project Structure
- `app.py`: The main Streamlit application script.
- `movie_dict.pkl`: Pickled dictionary containing movie metadata.
- `similarity.pkl`: Pickled similarity matrix computed using Content-Based Filtering.
- `tmdb_5000_movies.csv`: Raw dataset used for training the model.
- `requirements.txt`: List of dependencies required to run the project.

## ⚙️ How to Run Locally

Since this project is hosted on GitHub, you can run it on your local machine by following these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd Movie-Recommendation-System
'''pip install -r requirements.txt'''
TMDB_API_KEY = "your_api_key_here"
streamlit run app.py
