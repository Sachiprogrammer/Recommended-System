# Recommended-System

## movie recommended system

The Movie Recommendation System is a content-based recommendation engine designed to suggest movies based on various features like genres, keywords, cast, and crew. The system leverages data preprocessing, feature extraction, and similarity calculations to provide personalized movie recommendations.

## Data Sources
- **TMDB 5000 Movies Dataset**: Contains movie metadata such as title, genres, and overview.
- **TMDB 5000 Credits Dataset**: Includes cast and crew information for movies.

## Implementation Details

### **1. Data Preprocessing**
- Drops missing values from the datasets.
- Merges the movies and credits datasets using the movie title.
- Extracts and processes columns like `genres`, `keywords`, and `cast`.

### **2. Feature Engineering**
- Converts JSON-like strings into lists of names (e.g., genres and cast members).
- Generates visualizations for:
  - **Genre distribution**
  - **Top 10 most frequent actors**
  - **Keywords and genre WordClouds**

### **3. Recommendation System**
- Vectorizes textual data using `CountVectorizer`.
- Computes cosine similarity between movie feature vectors.
- Suggests movies based on the similarity scores.

### **4. Model Saving**
- Serializes the recommendation model using the `pickle` library for future use.

## Project Setup

### **Prerequisites**
- Python >= 3.7
- Libraries:
  - `numpy`, `pandas`, `matplotlib`, `scikit-learn`, `ast`, `wordcloud`, `pickle`



