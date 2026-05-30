# Wine Quality Prediction

A regression and classification pipeline that predicts wine quality scores from physicochemical properties, demonstrating feature selection, model benchmarking, and evaluation on a real-world chemical dataset.

## Problem Statement
Wine quality assessment is traditionally done by human experts, which is subjective and expensive. This project builds an ML model to predict quality scores from measurable chemical properties — enabling objective, scalable quality assessment.

## Dataset
- **Source:** UCI Wine Quality Dataset (red wine)
- **Records:** ~1,599 samples
- **Features:** 11 physicochemical properties — fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol
- **Target:** Quality score (0–10 scale)

## Methodology
1. **EDA** — correlation heatmaps, quality score distribution, outlier detection
2. **Feature Selection** — identifying highest-weight predictors
3. **Model Training** — classification/regression model(s) with Scikit-learn
4. **Evaluation** — accuracy score, model comparison

## Results
> ⚠️ Add your actual accuracy and model name here after running the notebook.

| Model | Accuracy |
|---|---|
| [Your model] | [Your accuracy]% |

**Key finding:** Alcohol content and sulphates were identified as the strongest predictors of wine quality.

## Tech Stack
`Python` `Pandas` `NumPy` `Scikit-learn` `Jupyter Notebook`

## Files
| File | Description |
|---|---|
| `wine quality prediction.ipynb` | Full ML pipeline notebook |

## How to Run
```bash
# Clone the repo
git clone https://github.com/Preet-Kanwal-Singh/Machine-Learning-Projects.git

# Navigate to project
cd Machine-Learning-Projects

# Install dependencies
pip install pandas numpy scikit-learn jupyter

# Launch notebook
jupyter notebook "wine quality prediction.ipynb"
```

---
*Built by [Preet-Kanwal-Singh](https://github.com/Preet-Kanwal-Singh) · B.Tech AI & ML · Amity University, Punjab*
