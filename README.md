## 🎬 MovieLens Feature Engineering & Exploratory Data Analysis (EDA)

### 📘 Overview

This project is part of the **HNG Data Analytics Track – Stage 1 Task**.
The goal is to clean, explore, and engineer features from the **MovieLens Dataset**, uncovering insights that can later support recommendation systems and analytics.

---

### 📊 Dataset Description

The dataset used is a subset of the [MovieLens dataset](https://grouplens.org/datasets/movielens/), which contains movie ratings, genres, tags, and external links.
The main CSV files include:

| File            | Description                                                           |
| --------------- | --------------------------------------------------------------------- |
| **ratings.csv** | Contains user ratings for movies (userId, movieId, rating, timestamp) |
| **movies.csv**  | Contains movie titles and genres (movieId, title, genres)             |
| **tags.csv**    | User-generated tags for movies                                        |
| **links.csv**   | Links MovieLens IDs to IMDb and TMDb IDs                              |

---

### ⚙️ Step 1: Data Preparation

* Loaded all four datasets using **Pandas**.
* Merged them on `movieId` to form a unified dataset.
* Checked for **missing values** and **duplicates**.
* Converted timestamps to readable **datetime** format for analysis.

---

### 🧠 Step 2: Feature Engineering

Created **6 new features** to enrich the dataset and enable deeper insights:

| Feature           | Description                                                      | Why It’s Useful                         |
| ----------------- | ---------------------------------------------------------------- | --------------------------------------- |
| `release_year`    | Extracted from the movie title (e.g., *Toy Story (1995)* → 1995) | Helps analyze movie trends over time    |
| `num_genres`      | Count of genres per movie                                        | Indicates genre diversity               |
| `main_genre`      | Extracted first genre as the dominant one                        | Useful for grouping and visualization   |
| `rating_year`     | Extracted from the rating timestamp                              | Enables time-based rating analysis      |
| `rating_month`    | Extracted month from timestamp                                   | Reveals seasonal trends in ratings      |
| `avg_user_rating` | Average rating per user                                          | Helps understand user behavior patterns |

---

### 🔍 Step 3: Exploratory Data Analysis (EDA)

Explored the dataset to uncover patterns and insights:

#### Key Insights:

1. ⭐ **Most ratings fall between 3.0 and 4.0**, indicating users tend to rate movies positively.
2. 🎭 **Drama, Comedy, and Action** are the top 3 most frequent genres.
3. 🕰️ **Movies from the 90's** dominate the dataset.
4. 👥 **Highly active users** tend to rate consistently across different genres.
5. 🎥 **Movies with multiple genres** tend to receive slightly higher ratings.
6. 📅 **Ratings increased steadily between 2000–2015**, suggesting growing user engagement.

---

### 📈 Visualizations

* Distribution of ratings (Histogram)
* <img width="716" height="524" alt="image" src="https://github.com/user-attachments/assets/da8d49ff-21fa-4fe4-9a29-f999b6f62a04" />
* Top 10 genres by frequency (Bar Chart)
 <img width="807" height="707" alt="image" src="https://github.com/user-attachments/assets/87fe4721-eca4-469d-aca1-e659c0ac248b" />
* Average rating by release year (Line Plot)
* Genre vs. Average Rating (Bar Chart)
 <img width="675" height="546" alt="image" src="https://github.com/user-attachments/assets/054bf2c8-97a4-49a0-b521-3b30d0240c64" />
* Number of movies released per year (Area Chart)
* User activity by rating count (Histogram)

---

### 🧩 Tools & Libraries

* **Python**
* **Jupyter Notebook**
* **Pandas**, **NumPy**
* **Matplotlib**, **Seaborn**
* **Datetime**

---

### 👨‍💻 Author

**Enoch Chukwuebuka**
 Data Analyst | Machine Learning Enthusiast
🔗 [LinkedIn]([https://www.linkedin.com/](https://www.linkedin.com/in/chukwuebuka-enoch/)) 

