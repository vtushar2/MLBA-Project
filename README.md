Hybrid Learning Analytics: Student Success Prediction, Personalized Recommendations & Q-Learning Tutor

An end-to-end Machine Learning + Recommender System + Reinforcement Learning EdTech project that predicts student performance, recommends personalized learning topics, and learns adaptive intervention strategies using Q-Learning.

This project uses a synthetic OULAD like dataset (automatically generated) to avoid dataset download issues while retaining realistic EdTech behavior.

🚀 Project Highlights

✔ Large synthetic OULAD-like dataset (5,000 students)

✔ Student Success Prediction using 7 ML models

✔ Hybrid Recommendation System (Collaborative Filtering + Content-Based)

✔ Q-Learning Tutor that learns optimal interventions

✔ Automatic feature engineering for 5 learning topics

✔ All outputs saved as CSV/PNG (easy for reports & dashboards)

✔ One-click runnable script, no external data downloads required

📂 Project Structure
edtech_ml_project/
│── edtech_project.py               # Main pipeline script
│── students_with_topics.csv        # Engineered dataset
│── interactions.csv                # Student-topic interaction matrix
│── items.csv                       # Topic metadata
│── hybrid_recommendations.csv      # Hybrid recommended topics
│── qlearning_recommendations.csv   # RL tutor recommendations
│── Q_table.csv                     # Learned Q-table
│── model_scores.csv                # ML model evaluation metrics
│── best_model.pkl                  # Saved ML model
│── feature_importance.csv          # Feature importance
│── feature_importance.png          # Feature importance plot
│── README.md                       # This file

🧠 1. Problem Statement

Modern EdTech systems must:

Predict which students are at risk of failing

Recommend personalized learning interventions

Continuously improve recommendations over time

Traditional ML systems fail at (3).
This project solves all three using:

ML models for prediction

Hybrid recommender system for personalization

Q-Learning reinforcement agent for adaptive tutoring

🛠️ 2. Technologies Used

Python

NumPy / Pandas

Scikit-Learn

TruncatedSVD

TF-IDF Vectorizer

Q-Learning

Matplotlib

Joblib

📊 3. Dataset Description

Since many users face issues downloading OULAD, this project uses:

✔ Synthetic OULAD-like dataset

Generated automatically with:

Student demographics

Engagement (VLE clicks)

Assessment scores

Credits studied

Attempts

IMD socioeconomic band

➡️ No need to download anything — project runs instantly.

🧱 4. Feature Engineering

5 Learning Topics are created:

Topic	Meaning
Study Habits	Based on assessment scores
Engagement	Based on VLE clicks
Assessment Level	Credits studied & difficulty
Support Need	IMD socioeconomic band
Activity Level	Previous attempts

Each topic is scaled 1–5, producing a:
✔ Student × Topic matrix
✔ Suitable for ML + CF + RL

🤖 5. Machine Learning Models

The project trains and evaluates:

Logistic Regression

Random Forest

MLP Neural Network

SVM

KNN

Naive Bayes

Decision Tree

Each model outputs:

Accuracy

F1-Score

ROC-AUC

📄 Results saved in:
model_scores.csv

🏆 Best model (RandomForest) is saved as:
best_model.pkl

🎯 6. Hybrid Recommendation System

Uses two engines:

🔹 Collaborative Filtering (CF)

Matrix factorization using Truncated SVD

🔹 Content-Based Filtering

TF-IDF embedding of topic descriptions
Cosine similarity for semantic boost

🔹 Hybrid Formula
final_score = 0.7 * CF + 0.3 * ContentBoost


📄 Output:
hybrid_recommendations.csv

🧭 7. Q-Learning Reinforcement Tutor

The RL agent learns which intervention (topic) leads to the best long-term outcome (Pass).

State (S):

Based on study habit level:

High

Low

Actions (A):

Recommend one of the 5 topics

Reward (R):
+1  → student passed
-1 → student failed


📄 Outputs:

Q_table.csv

qlearning_recommendations.csv

📈 8. Visualizations

Generated automatically:

Feature importance plot

Confusion matrices (per model)

Recommendation frequency

Q-table heatmap

Main plot saved as:
feature_importance.png
