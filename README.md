# Early Retention Prediction using Sequence Models (LSTM)
**Status: Active Development (Model Architecture & Feature Engineering Complete)**

## Project Overview
While standard models look at "what" a user did, this project looks at the "sequence" of how they did it. Using Long Short-Term Memory (LSTM) networks, I predict Day-7 retention based solely on the sequence of events from a player's first 24 hours.

## Technical Metrics
* **Model Quality:** 0.78 AUC-ROC (Area Under Curve).
* **Baseline Comparison:** 14% improvement over standard Logistic Regression.
* **Prediction Window:** Predicts long-term churn using only Day-1 behavioral sequences.

## Tech Stack
* **Deep Learning:** Python (TensorFlow/Keras).
* **Data Processing:** NumPy, Pandas (Sequence padding and time-series transformation).
* **Analysis:** Matplotlib/Seaborn for loss/accuracy curve visualization.

## Why LSTM?
Traditional models lose the temporal context of player behavior. LSTMs allow the model to understand the *frustration path* (e.g., three consecutive level fails followed by an app close), providing an "early warning" system for the product team.

## Roadmap
- [x] Sequence feature engineering (Event-to-Integer mapping).
- [x] LSTM Model architecture design.
- [ ] Hyperparameter tuning and Cross-validation.
- [ ] Interpretability analysis (SHAP/Feature Importance).
