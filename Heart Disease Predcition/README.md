# Heart Disease Prediction

A binary classification model that predicts the likelihood of heart disease from patient clinical data, built to support data-driven diagnostic assistance in healthcare.

## Problem Statement
Heart disease is one of the leading causes of mortality globally. Early prediction using patient health parameters can enable timely intervention. This project builds a machine learning pipeline to classify patients as at-risk or not at-risk based on 13 clinical features.

## Dataset
- **Source:** Cleveland Heart Disease Dataset (UCI Machine Learning Repository)
- **Records:** ~303 patients
- **Features:** 13 clinical parameters — age, sex, chest pain type (cp), resting blood pressure (trestbps), cholesterol (chol), fasting blood sugar (fbs), resting ECG (restecg), max heart rate (thalach), exercise-induced angina (exang), ST depression (oldpeak), slope, number of vessels (ca), thalassemia (thal)
- **Target:** Binary — 0 (no disease), 1 (disease present)

## Methodology
1. **Exploratory Data Analysis** — correlation heatmaps, distribution plots, outlier detection
2. **Feature Engineering** — MinMax scaling, handling missing values
3. **Model Training** — Logistic Regression with train/test split
4. **Evaluation** — Accuracy score on held-out test set

## Results
| Model | Accuracy |
|---|---|
| Logistic Regression | **81.97%** |

## Tech Stack
`Python` `Pandas` `NumPy` `Scikit-learn` `Jupyter Notebook`

## Files
| File | Description |
|---|---|
| `heart_disease_data.csv` | Cleveland UCI dataset |
| `heart_disease_prediction.ipynb` | Full ML pipeline notebook |

## How to Run
```bash
# Clone the repo
git clone https://github.com/Preet-Kanwal-Singh/Machine-Learning-Projects.git

# Navigate to project
cd Machine-Learning-Projects/Heart\ Disease\ Predcition

# Install dependencies
pip install pandas numpy scikit-learn jupyter

# Launch notebook
jupyter notebook heart_disease_prediction.ipynb
```

---
*Built by [Preet-Kanwal-Singh](https://github.com/Preet-Kanwal-Singh) · B.Tech AI & ML · Amity University, Punjab*
