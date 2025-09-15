# 🎬 Movie Recommendation System

This project is a **Movie Recommendation System** that suggests movies to users based on their preferences and past ratings. It combines **Collaborative Filtering** and **Content-Based Filtering** to give better recommendations, similar to how Netflix recommends movies.

---

##  How It Works

### 1. Data Used
- **Movies Dataset** → contains movie titles, genres, keywords, cast, and descriptions.  
- **Ratings Dataset** → contains user IDs, movie IDs, and the ratings users gave.  

### 2. Content-Based Filtering
- Looks at **movie features** (genres, keywords, overview, cast, director).  
- Uses **cosine similarity** to find movies most similar to the one the user searches for.  
- Example: If you liked *Inception*, it will suggest other sci-fi thrillers.

### 3. Collaborative Filtering
- Looks at **user behavior** (ratings given by different users).  
- Finds **similar users** and recommends movies they liked.  
- Example: If User A and User B have similar tastes, User A will get recommendations based on what User B enjoyed.

### 4. Hybrid Approach
- Combines both methods so recommendations are:  
  - Based on **movies you like**.  
  - Based on **what similar users enjoy**.  
- If a movie is not in the dataset, the system allows the user to **add it manually** with details.

---

##  Steps in the Notebook
1. **Load datasets** (`tmdb_5000_movies.csv`, `tmdb_5000_credits.csv`, `ratings.csv`).  
2. **Preprocess data** (clean missing values, merge datasets, create features).  
3. **Build Content-Based Model** (TF-IDF + Cosine Similarity).  
4. **Build Collaborative Filtering Model** (User–Item matrix).  
5. **Hybrid Function** combines both results.  
6. **Interactive Function (`search_and_recommend`)** lets users search movies and get personalized results.

---

##  What This Project Does

-  The system gives **personalized hybrid recommendations**.  
-  Users can **search movies by title**.  
-  If a movie is missing, the system allows **adding new movies dynamically**.  
-  Combines both **content similarity** and **collaborative filtering** to generate recommendations.  

## Clone the repository:
   git clone https://github.com/NoorUlEmanBukhari/MoviesRecommendationSystem.git
