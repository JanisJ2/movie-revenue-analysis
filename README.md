# 🎬 Movie Revenue Analysis  

## 🖥️ Live Demo  
🌐 **Deployed Website:** [https://janisj2.github.io/movie-revenue-analysis/](https://janisj2.github.io/movie-revenue-analysis/)

## 📌 Project Overview  
This project investigates factors that influence a movie's box office revenue using data from **The Movie Database (TMDB) API**. The analysis examines predictors such as **budget, popularity, runtime, release season, and genres**, along with actor and crew information. The goal is to understand the relationships between these features and financial success, and to build predictive models that estimate revenue based on movie attributes.

## 🔍 Research Question  
**How do factors such as budget, popularity, release season, runtime, genres, actors, and crew influence a movie’s box office revenue?**  

## 📊 Data Collection & Processing  
- **Data Source:** TMDB API  
- **Endpoints Used:**
  - `/discover/movie` – to collect top-revenue movie IDs and titles.
  - `/movie/{movie_id}` – for movie-level details (revenue, budget, popularity, etc.).
  - `/movie/{movie_id}/credits` – for cast and crew data.
- **Key Features Extracted:**  
  - Revenue, budget (inflation-adjusted), popularity, runtime, release date, genres.  
  - Top 5 actor and crew names with average popularity scores.  
- **Data Cleaning & Wrangling:**  
  - Converted dates; removed missing/invalid values; adjusted budget using CPI data.  
  - One-hot encoded genres; created release season variable.  
  - Excluded the “adult” rating due to lack of variation in the dataset.  

## 📈 Analysis & Modeling  
### 🧪 Exploratory Data Analysis (EDA)  
- Visualized revenue distribution (raw and log-transformed).  
- Plotted revenue against budget, popularity, and runtime.  
- Boxplots and ANOVA to explore seasonal and genre-related trends.  
- Heatmaps and feature correlations.  

### 📊 Predictive Modeling  
- **Multiple Linear Regression:** To establish baseline associations and interpret coefficients.  
- **Random Forest & XGBoost:** For modeling complex, nonlinear relationships and feature interactions.  
- Compared model performance and variable importance across approaches.  

## ✅ Final Results Summary  
- **Budget and popularity** are strong, consistent predictors of revenue.  
- **Release season and genres** show some effect—movies released in **Summer** generally perform better.  
- Tree-based models (especially **XGBoost**) offered improved predictive accuracy over linear regression.  
- Actor and crew popularity added some predictive value, but were less influential than core features like budget.  

## 🛠️ Tools & Libraries  
- **Language:** R  
- **Libraries:** `tidyverse`, `randomForest`, `xgboost`, `lubridate`, `ggplot2`, `caret`, `httr`, `jsonlite`, etc.  
- **Data Source:** [TMDB API](https://developer.themoviedb.org/docs/getting-started)  

## 🔗 GitHub Repository  
[https://github.com/JanisJ2/movie-revenue-analysis](https://github.com/JanisJ2/movie-revenue-analysis)

## 📌 Acknowledgments  
Special thanks to **The Movie Database (TMDB)** for providing access to comprehensive movie data.
