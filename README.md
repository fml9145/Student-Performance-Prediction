# Student-Performance-Prediction

Predicting students’ final grades using machine learning regression models.

## 📌 Project Overview
This project predicts students’ final numeric grades (G3) using demographic, social,
and academic features from the UCI Student Performance Dataset.  
Unlike many prior works that frame this as a pass/fail classification problem, this project
treats it as a **regression task**, producing more informative predictions for educators
and students.

## 📊 Dataset
- Source: UCI Student Performance Dataset
- Target variable: **Final Grade (G3)**, range 0–20
- Features:
  - Categorical: school, sex, address, parental jobs, support indicators, etc.
  - Numerical: age, study time, absences, prior grades (G1, G2), health, alcohol use

## ⚙️ Preprocessing
- One-hot encoding for categorical features (drop-first to avoid multicollinearity)
- Feature scaling for numerical variables
- 80/20 train-test split
- End-to-end preprocessing implemented using a pipeline

## 🤖 Models Used
- **Random Forest Regressor**
- **XGBoost Regressor**

Hyperparameters were tuned to optimize performance.

## 📈 Results
| Model          | RMSE  | R²   |
|----------------|-------|------|
| Random Forest  | 1.447 | 0.785 |
| **XGBoost**    | **1.226** | **0.846** |

XGBoost achieved the best performance with lower prediction error and tighter residuals.

## 🧠 Key Takeaways
- Prior grades (G1, G2) are strong predictors of final performance
- Ensemble regression models outperform simpler approaches
- Numeric grade prediction provides more actionable insights than pass/fail classification

## 🔗 Notebook
[Google Colab Notebook](https://colab.research.google.com/drive/1Vk1eo4oIv17sWLzVQWKXDhg7cPcRxjXo)

## 🛠️ Technologies
- Python
- scikit-learn
- XGBoost
- Pandas, NumPy
- Matplotlib / Seaborn

## 👤 Author
**Faith Leverett**  
Sole contributor
