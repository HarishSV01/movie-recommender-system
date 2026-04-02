# 🎬 Movie Recommendation System (MovieLens 1M)

A personalized movie recommendation system built using collaborative filtering techniques, including **Pearson Correlation**, **Cosine Similarity (KNN)**, and **Matrix Factorization**.  
The project evaluates models using both prediction metrics and top-K ranking metrics.

---

## 📌 Overview

This project develops a movie recommender system that suggests personalized movies based on user ratings and similarity patterns. It covers the full ML workflow: data loading, feature engineering, exploratory analysis, model building, and evaluation.

---

## 📂 Dataset

- **Dataset:** MovieLens 1M
- **Ratings:** ~1 million
- **Users:** ~6,000
- **Movies:** ~3,700
- **Sparsity:** ~95.5%

**Source:** GroupLens Research Lab, University of Minnesota

---

## ⚙️ Approach

### 1. Baseline Model
- Popularity-based recommender
- Uses average ratings and number of ratings

### 2. Collaborative Filtering
- Item-based filtering using **Pearson Correlation**
- Item-based filtering using **Cosine Similarity + KNN**

### 3. Matrix Factorization
- Latent factor model using **CMF**
- Captures hidden user-item interaction patterns

### 4. User-Based Recommendation
- Finds similar users based on common ratings
- Recommends movies liked by similar users

---

## 📊 Key Results

| Metric | Value |
|--------|-------|
| Baseline RMSE | 0.9824 |
| MF RMSE | 0.8644 |
| Improvement | 11.6% |
| Precision@5 | 0.2264 |
| Recall@5 | 0.0319 |
| Precision@10 | 0.1916 |
| Recall@10 | 0.0544 |

---

## 🧠 Key Insights

- Matrix Factorization improved prediction accuracy over the baseline.
- Ranking metrics such as **Precision@K** and **Recall@K** are more useful than RMSE for recommender quality.
- Increasing K improves recall but slightly reduces precision.
- High sparsity has a strong impact on recommendation quality.

---

## ⚠️ Limitations

- Cold start problem for new users and new items
- Sparse user-item interaction matrix
- Offline evaluation may differ from real-world behavior

---

## 🚀 Future Improvements

- Hybrid recommender system combining collaborative and content-based filtering
- Implicit feedback such as clicks, watch time, and search history
- Ranking metrics like **NDCG@K**
- Deployment using **Streamlit** or **FastAPI**

---

## 💼 Business Recommendations

- Target the **25–34 age group** with personalized recommendations
- Use **Matrix Factorization** for accurate rating prediction
- Use **KNN similarity** for “movies like this” suggestions
- Mitigate cold start by asking new users to rate 5–10 movies initially
- Focus on **Comedy** and **Drama** genres for higher engagement

