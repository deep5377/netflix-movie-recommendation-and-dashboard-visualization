# Netflix Movie Recommendation System & Dashboard Visualization

This project is a full-stack web application that recommends movies on Netflix based on Natural Language Processing (NLP) techniques. It also includes an interactive Tableau dashboard to visualize Netflix's catalog and revenue insights.

---

## 📌 Project Highlights

✅ Web-based movie recommendation system (Flask + HTML + JS)  
✅ Content-based recommendation using NLP (TF-IDF + Cosine Similarity)  
✅ Tableau dashboard visualizing Netflix catalog and revenue trends  
✅ Clean, modular code with reusable components  
✅ Visual and interactive frontend (autocomplete, loader, UI styling)


![Python](https://img.shields.io/badge/Python-3.8-blueviolet)
![Framework](https://img.shields.io/badge/Framework-Flask-red)
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)
![API](https://img.shields.io/badge/API-TMDB-fcba03)

  ### Sources of the datasets 

1. [IMDB 5000 Movie Dataset](https://www.kaggle.com/carolzhangdc/imdb-5000-movie-dataset)
2. [The Movies Dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset)
3. [List of movies in 2018](https://en.wikipedia.org/wiki/List_of_American_films_of_2018)
4. [List of movies in 2019](https://en.wikipedia.org/wiki/List_of_American_films_of_2019)
5. [List of movies in 2020](https://en.wikipedia.org/wiki/List_of_American_films_of_2020)


## Project Structure

netflix-movie-recommendation-and-dashboard-visualization-main/

├── app.py # Flask backend

├── main_data.csv # Cleaned movie dataset

├── movie_metadata.csv # Raw dataset

├── nlp_model.pkl # Trained NLP model

├── transform.pkl # TF-IDF vectorizer

├── Netflix Revenue.csv # Revenue data for Tableau

├── NETFLIX DASHBOARD.twb # Tableau dashboard

├── preprocessing/ # Jupyter Notebooks & CSVs

│ ├── preprocessing 1–4.ipynb

│ ├── final_data.csv

│ ├── sentiment.ipynb

│ └── reviews.txt

├── static/ # JS, CSS, images

│ ├── style.css

│ ├── loader.gif

│ ├── recommend.js, autocomplete.js

├── templates/ # HTML Templates
│ ├── home.html
│ └── recommend.html

├── requirements.txt # Python dependencies
├── Procfile # For deployment (Heroku-compatible)


---

## 💡 How it Works

1. **Preprocessing**:
   - Movie data is cleaned, transformed, and processed.
   - NLP pipeline uses TF-IDF Vectorizer + Cosine Similarity for generating recommendations.

2. **Web Interface**:
   - `home.html`: Search bar with autocomplete
   - `recommend.html`: Returns top similar movies for a selected title

3. **Recommendation Logic**:
   - Input: Movie Title
   - Output: Top N recommendations based on plot similarity

4. **Dashboard**:
   - Built in Tableau using `Netflix Revenue.csv`
   - Includes genre trends, release patterns, and revenue over time

---

## 🛠 Technologies Used

- **Python**, **Flask**, **Pandas**, **Scikit-learn**, **Numpy**
- **HTML**, **CSS**, **JavaScript** (Autocomplete & UI logic)
- **Tableau** for data visualization
- **Pickle** for model persistence

---

## ⚙️ Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/netflix-movie-recommendation-and-dashboard-visualization.git
cd netflix-movie-recommendation-and-dashboard-visualization

Run the Flask app

python app.py
Visit http://127.0.0.1:5000/ in your browser.

Tableau Dashboard
To explore the Tableau dashboard:

Open NETFLIX DASHBOARD.twb using Tableau Desktop or Tableau Public

Analyze:

Revenue trends

Genre distribution

Popular release years

FAQ
Q: Can I add more movies to this system?
Yes, add them to main_data.csv and regenerate the model.

Q: Can I deploy this online?
Yes, use Heroku. Procfile included.

Q: How are recommendations made?
TF-IDF vectorizes plot summaries, and cosine similarity identifies the closest titles.

📄 License
This project is open-source under the MIT License.


