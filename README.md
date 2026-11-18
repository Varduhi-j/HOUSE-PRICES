# House Prices - Advanced Regression Techniques

## Project Overview
This project predicts house sale prices using the Kaggle House Prices dataset.

The goal is to build machine learning regression models and evaluate their performance using 5-fold cross-validation.

## Dataset
The dataset was obtained from the Kaggle House Prices - Advanced Regression Techniques competition.

- Training data: 1460 rows
- Test data: 1459 rows
- Target variable: SalePrice

## Project Structure
- `data/raw/` - Original Kaggle datasets
- `data/processed/` - Cleaned and processed datasets
- `notebooks/01_EDA.ipynb` - Exploratory Data Analysis and feature engineering
- `notebooks/02_Models.ipynb` - Model training, tuning and evaluation
- `results/figures/` - Saved visualizations
- `results/model_comparison.csv` - Model comparison results
- `submissions/` - Kaggle submission and score screenshot

## Data Preparation
- Handled missing values
- Investigated outliers
- Created new features:
  - TotalSF
  - TotalBathrooms
  - HouseAge
  - TotalPorchSF
- Applied one-hot encoding to categorical variables

## Models
The following models were evaluated:
- Baseline (Dummy Regressor)
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- Tuned Gradient Boosting Regressor

## Model Evaluation

The best model was Tuned Gradient Boosting.

- Best parameters:
  - n_estimators: 400
  - learning_rate: 0.05
  - max_depth: 2
  - min_samples_leaf: 2
- 5-fold Cross-Validation RMSE: 0.11906
- Kaggle Public Score: 0.13388

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- VS Code

## AI Assistance
ChatGPT was used for guidance, code explanations, debugging assistance, and project documentation. All project steps and code were reviewed and executed by the student.

## Conclusion
The tuned Gradient Boosting model achieved the best cross-validation performance among the evaluated models and was used to generate the final Kaggle submission.
