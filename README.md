# House-Pricing-Advanced-Regression

This project builds machine learning models to predict house prices using the **Ames Housing dataset**.  
The goal is to explore how different regression approaches and preprocessing techniques affect prediction accuracy.

---

## Project Structure

Two versions of the pipeline are included:

| Version | Description |
|------|------|
| **Baseline** | Linear regression models with standard preprocessing |
| **Improved** | Ensemble models and dimensionality reduction |

---

## Dataset

Kaggle: **House Prices – Advanced Regression Techniques**

The dataset includes:

- Property size and area
- Construction year
- Quality ratings
- Neighborhood
- Structural features

Target variable:

**SalePrice**

---

## Baseline Model

Pipeline:

- Data cleaning
- Missing value handling
- One-hot encoding for categorical variables
- Feature scaling
- Model training

Models used:

- **Linear Regression**
- **SGDRegressor**

---

## Improved Model

Enhancements:

- Removal of highly sparse features
- Additional preprocessing
- **Dimensionality reduction using PCA**
- Ensemble modeling

Models explored:

- **Random Forest Regressor**
- **KNN Regressor**
- **Bagging / AdaBoost experiments**

---

## Model Performance Comparison

Both pipelines were evaluated using the **same validation split and metrics**.

| Version | Models | Validation R² | Validation RMSE |
|------|------|------|------|
| **Baseline** | Linear Regression, SGDRegressor | ~0.89 | ~29,400 |
| **Improved** | Random Forest, KNN, Bagging / AdaBoost | ~0.91 | ~28,300 |

The improved pipeline reduces prediction error by using stronger models and improved feature processing.

---

## Key Insights

- Tree-based models captured non-linear relationships better than linear models
- Removing noisy features improved stability
- PCA reduced dimensionality while keeping most variance

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook
