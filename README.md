# 🎬 Movie Revenue Analysis  

## 📌 Project Overview  
This project explores factors that influence a movie's box office revenue using data from **The Movie Database (TMDB) API**. The analysis examines key predictors such as **budget, popularity, runtime, release season, and genres**, along with actor and crew information. The goal is to identify patterns and relationships that contribute to a film’s financial success.  

🚧 **Note:** This project is currently at the **midterm stage** and will be expanded in the final project with additional analysis and refined predictive modeling.  

## 🔍 Research Question  
**How do factors such as budget, popularity, release season, runtime, genres, actors, and crew influence a movie's box office revenue?**  

## 📊 Data Collection & Processing  
- **Data Source:** TMDB API  
- **Key Features Collected:**  
  - **Movie-Level Data:** Revenue, budget, popularity, runtime, release date (processed into seasons), and genres (one-hot encoded).  
  - **Actor & Crew Data:** Top 5 actors and crew members per movie, with average popularity scores.  
- **Data Cleaning & Processing:**  
  - Converted dates, handled missing values, removed inconsistencies.  
  - Applied one-hot encoding for genres and categorized release seasons.  

## 📈 Current Progress (Midterm)  
- **Exploratory Data Analysis (EDA):**  
  - Revenue distributions (raw and log-transformed).  
  - Scatter plots for revenue vs. budget, popularity, and runtime.  
  - Boxplots for revenue by **season** and **genre**.  
  - Correlation heatmaps and actor/crew analysis.  
- **Statistical Analysis:**  
  - Multiple regression to assess numeric predictors (budget, popularity, runtime, etc.).  
  - Genre-based regression analysis.  
  - ANOVA to evaluate seasonal revenue differences.  

## 🚀 Next Steps (Final Project)  
- **Refining the regression model** (considering interaction terms, polynomial basis functions).  
- **Testing tree-based models** (Decision Trees, Random Forest, XGBoost).  
- **Improving feature selection** (better actor/crew popularity metrics).  
- **Exploring long-term revenue trends** and refining seasonal effects.  

## 🛠️ Tools & Libraries  
- **Programming Language:** R  
- **Data Source:** [TMDB API](https://developer.themoviedb.org/docs/getting-started)  

## 📌 Acknowledgments  
Special thanks to **The Movie Database (TMDB)** for providing access to movie data.  

---
