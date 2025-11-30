This repository includes an interactive application built using Google AI Studio, designed to demonstrate the core functionality of the EdTech ML system in a simple, user-friendly interface.

The app allows users (students, educators, faculty, evaluators) to interact with the system without needing to run Python code locally.

🎯 Purpose of the App

The goal of this app is to provide a hands-on, real-time demonstration of:

✔ Student Performance Prediction

Users can input or adjust student attributes, and the app predicts whether the student is likely to Pass or Fail based on the trained ML models.

✔ Personalized Topic Recommendations

The app uses the Hybrid Recommendation System to suggest which learning topics the student should focus on:

Study Habits

Engagement

Assessment Level

Support Need

Activity Level

These align with the same categories from the main pipeline.

✔ Q-Learning Tutor Suggestions

The app also shows Q-Learning–based adaptive recommendations, learned from long-term reward patterns.

This demonstrates how an AI tutor can:

learn from data

adjust to different student states

recommend optimal interventions over time

🔗 Live Demo Link

You can launch the app here:

👉 AI Studio App:
https://aistudio.google.com/apps/drive/1hL5XIlN3tLrLLAK2Ukz8o7_OULR2v2wI?showAssistant=true&resourceKey=&showPreview=true

No installation is required.
The app runs fully in the browser.

🧩 What the App Demonstrates
1. Student Input Module

Users can set or modify:

Assessment scores

Engagement level

Study effort

Activity level

Support need

2. ML-Based Prediction Module

Shows:

Pass/Fail prediction

Confidence score

Model explanation summary

3. Recommendation Dashboard

Displays:

Top-N hybrid recommended topics

Reasoning behind each recommendation

Estimated impact on student performance

4. Q-Learning Adaptive Tutor

The app outputs:

Current student state

Best topic selected by Q-learning agent

Expected reward value

Suggestions for continuous improvement

🛠️ Behind the Scenes (Technical Summary)

Even though the app is simple for users, it communicates with a backend system powered by:

Trained ML models (best_model.pkl)

Hybrid recommender engine

Q-Learning agent (learned Q_table.csv)

Preprocessed dataset (students_with_topics.csv)

Feature engineering pipeline

This makes the app lightweight, responsive, and able to run instantly.

🎨 Why This App Matters

It provides:

A clean and interactive showcase of your project

A demo for faculty or panel members

A non-technical interface for users

A way to show real-time ML predictions and AI recommendations

This also strengthens:

Your GitHub portfolio

Case competition submissions

Academic project presentations

Resume/LinkedIn project highlights
