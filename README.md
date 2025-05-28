# 🎥 Movie Recommendation System

![machine-learning-project-movie-recommendation-system](https://github.com/user-attachments/assets/769e9021-b5e8-4aa1-aea9-aaef5e02e4e7)


<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue.svg" />
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen.svg" />
  <img src="https://img.shields.io/badge/Machine_Learning-Content_Based-orange.svg" />
</p>

---

## 🧠 Overview

In the era of streaming platforms, the amount of available content is overwhelming. Ever spent more time deciding what to watch than actually watching something? 🎬

This project builds a **Content-Based Movie Recommendation System** that helps users find movies similar to their favorite ones using **textual metadata** such as:

* Genre 🎭
* Cast 👨‍🎤
* Crew 🎬
* Overview 📜
* Keywords 🔑

By combining this information and applying **Natural Language Processing (NLP)**, the system computes similarities and suggests top relevant movies instantly!

---

## ✨ Features

✅ Recommend movies based on content
✅ Intuitive Jupyter Notebook for analysis
✅ Uses Cosine Similarity with CountVectorizer
✅ Cleans and preprocesses movie metadata
✅ Easy-to-use `recommend()` function

---

## 🛠️ Tech Stack

| Tool / Library     | Purpose                               |
| ------------------ | ------------------------------------- |
| `Python`           | Core language for logic & computation |
| `Pandas`           | Data wrangling & merging              |
| `NumPy`            | Numeric computations                  |
| `Scikit-learn`     | Text vectorization & similarity       |
| `NLTK`             | Natural language processing           |
| `Jupyter Notebook` | Visualization and iterative coding    |

---

## 🗃️ Dataset

* **movies.csv** – Metadata like genres, titles, overviews
* **credits.csv** – Details on cast and crew
* Source: [TMDb API](https://www.themoviedb.org/)

These datasets are merged and cleaned for a richer feature set used in recommendations.

---

## 🧪 How It Works

### 🧹 1. Data Preprocessing

* Merge datasets
* Extract genres, keywords, cast, crew
* Convert text to lowercase, remove stopwords, apply stemming

### 🧬 2. Feature Engineering

* Combine all textual metadata into a `tags` column
* Use `CountVectorizer` to convert tags into numeric vectors

### 📏 3. Similarity Computation

* Calculate **cosine similarity** between movies based on their tag vectors

### 🎯 4. Recommendation Engine

```python
recommend("Inception")
```

🎉 Output:

```
1. Interstellar  
2. The Prestige  
3. The Matrix  
4. Memento  
5. The Dark Knight
```

---

## 📈 Visualizations (Optional Add-ons)

* Bar plots of similarity scores 📊
* Word clouds for popular tags ☁️

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/movie-recommendation.git
   cd movie-recommendation
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   ```bash
   jupyter notebook MovieRecommendation.ipynb
   ```

---

## 🔧 Improvements for the Future

* Add fuzzy search for movie title input
* Develop a web UI using **Streamlit** or **Flask**
* Support user-based collaborative filtering
* Incorporate real-time data from TMDb API

---

## 🧑‍💻 Author

**Your Name**
📫 [GitHub](https://github.com/yourusername) | [LinkedIn](https://linkedin.com/in/yourprofile)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
