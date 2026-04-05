# Movie Recommendation System 🎬
![Demo Screenshot](images/Screenshot.png)

A Machine Learning-based web application that recommends the top 5 similar movies based on your selection. It uses **Content-Based Filtering** and a clean UI built with **Streamlit**.

## ✨ Features
*   **User-friendly Interface:** Simple and clean UI built using Streamlit.
*   **Accurate Recommendations:** Finds similar movies using movie metadata.
*   **Dynamic Posters:** Fetches real-time movie posters using the TMDB API.

## 🛠️ Tech Stack
*   **Language:** Python
*   **Libraries:** Pandas, Scikit-learn, Streamlit, Requests, Pickle
*   **Data Source:** [The Movie Database (TMDB)](https://themoviedb.org)

## 📁 Project Structure
```text
├── .streamlit/
│   └── secrets.toml      # API Keys (Ignore in Git)
├── app.py                # Main Streamlit application code
├── movie_dict.pkl        # Processed movie data dictionary
├── similarity.pkl        # Cosine similarity matrix
├── requirements.txt      # List of dependencies
├── .gitignore            # Files to ignore in Git
└── README.md             # Project documentation
```
## ⚙️ Setup Instructions

1. **Install Dependencies:**
   Run the following command in your terminal or command prompt:
   ```bash
   pip install streamlit pandas requests
2. **API Key Setup:**
   Add your TMDB API Key to the `.streamlit/secrets.toml` file as follows:
   ```toml
   TMDB_API_KEY = "your_api_key_here"
3. **Run the App:**
   Navigate to the project folder and run this command in your terminal:
   ```bash
   streamlit run app.py
4. **Data Preparation:**
   Ensure that `movie_dict.pkl` and `similarity.pkl` are present in your project directory. If they are missing, run your data processing notebook to generate them.

## 🧠 How it Works?
When you select a movie, the system uses the `similarity.pkl` file to calculate the **Cosine Similarity** (distance) between that movie's vector and all other movie vectors. It then displays the top 5 closest matches along with their posters fetched from the TMDB API.

---
**Developed by [Afrin Tabassum]**
