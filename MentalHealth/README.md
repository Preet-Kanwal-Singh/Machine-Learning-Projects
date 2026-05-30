# Mental Health Prediction

A 7-class classification model that predicts mental health condition likelihood and treatment-seeking behaviour from workplace and lifestyle survey data, enabling early risk detection at scale.

## Problem Statement
Mental health conditions are underdiagnosed, particularly in workplace settings. This project uses survey data to predict which condition (if any) a respondent is likely experiencing, and whether they are likely to seek treatment — providing interpretable, data-driven insights into at-risk population patterns.

## Dataset
- **Source:** Combined mental health survey dataset (OSMI-style)
- **Records:** 9,203 survey responses
- **Features:** 20+ categorical and numerical variables — remote work status, company size, family history, work interference, self-employed status, benefits availability, and more
- **Target:** 7 classes — Anxiety, Bipolar, Depression, Normal, Personality Disorder, Stress, Suicidal

## Methodology
1. **Data Preprocessing** — label encoding on 20+ categorical features, null handling
2. **EDA** — class distribution analysis, correlation mapping, feature importance
3. **Model Benchmarking** — Decision Tree, Logistic Regression, Linear SVM
4. **Evaluation** — accuracy, precision, recall, F1-score (macro and weighted averages)

## Results
| Model | Accuracy | Macro F1 | Weighted F1 |
|---|---|---|---|
| Linear SVM | **71%** | 0.65 | **0.70** |
| Logistic Regression | ~68% | — | — |
| Decision Tree | ~65% | — | — |

**Best per-class F1 scores (Linear SVM):**
| Class | Precision | Recall | F1 |
|---|---|---|---|
| Normal | 0.81 | 0.92 | **0.86** |
| Anxiety | 0.77 | 0.76 | **0.76** |
| Bipolar | 0.81 | 0.65 | 0.72 |
| Depression | 0.66 | 0.68 | 0.67 |

## Key Findings
- Remote work status and company size were the highest-weight predictors of mental health risk
- The model performs strongest on "Normal" and "Anxiety" classes, with lower recall on rarer conditions (Stress, Personality Disorder) due to class imbalance

## Tech Stack
`Python` `Pandas` `NumPy` `Scikit-learn` `Jupyter Notebook`

## Files
| File | Description |
|---|---|
| `Combined Data.csv` | Survey dataset (9,203 records) |
| `MentalHealthAnalysis.ipynb` | Full ML pipeline notebook |

## How to Run
```bash
# Clone the repo
git clone https://github.com/Preet-Kanwal-Singh/Machine-Learning-Projects.git

# Navigate to project
cd Machine-Learning-Projects/MentalHealth

# Install dependencies
pip install pandas numpy scikit-learn jupyter

# Launch notebook
jupyter notebook MentalHealthAnalysis.ipynb
```

---
*Built by [Preet-Kanwal-Singh](https://github.com/Preet-Kanwal-Singh) · B.Tech AI & ML · Amity University, Punjab*
