# 🍔 Food Review Recommendation System

This project is a **Collaborative Filtering Recommender System** that suggests food products to users based on their past review ratings. It uses **Singular Value Decomposition (SVD)** to generate personalized recommendations from a sparse user-item matrix.

> 📁 Project Files:
> - `Food_Review_Recommendation.ipynb` – Jupyter notebook with the full implementation  
> - `Reviewss.csv` – Dataset containing food product reviews

🔗 **GitHub Repository**: [github.com/majumdarjoyeeta/-Food-Review-Recommendation-System](https://github.com/majumdarjoyeeta/-Food-Review-Recommendation-System)

---

## 🚀 Features

- Personalized recommendations using SVD
- Sparse matrix handling for efficient computation
- Easy-to-use recommendation function
- Ready for future extensions like model evaluation or deployment

---

## 🗂️ Dataset

The dataset `Reviewss.csv` contains food product reviews. Relevant columns used:

- `UserId`: Unique identifier for each reviewer
- `ProductId`: Unique identifier for each product
- `Score`: User rating (typically 1–5)

Other columns like `Summary`, `Text`, or `ProfileName` are not used in this model but can be integrated later for hybrid systems.

---

## 📌 How It Works

1. **Preprocess** the data and build a user-item rating matrix
2. **Apply SVD** to reduce dimensionality and find latent features
3. **Predict** missing ratings based on the learned features
4. **Recommend** top-rated products the user hasn't rated yet

---

## 💡 Sample Usage

In the notebook, you can generate top 5 recommendations for a user:

```python
recommend_items(user_id='A3SGXH7AUHU8GW', pivot_df=pivot_df, preds_df=preds_df, num_recommendations=5)
Replace the user_id with any valid ID from the dataset.

🛠️ Requirements
Install necessary libraries using:

bash
Copy
Edit
pip install numpy pandas scipy scikit-learn matplotlib seaborn
Or use the included requirements.txt (if added).

📈 Potential Extensions
Evaluation metrics (RMSE, Precision@K, Recall@K)

Popularity-based baseline model

Content-based filtering integration (hybrid system)

Web app (Streamlit or Flask) for interactive recommendations

📜 License
This project is open-source and available under the MIT License.

🙌 Acknowledgments
Built as a simple and scalable prototype of a recommendation system using collaborative filtering techniques, similar to those used by platforms like Amazon and Yelp.

