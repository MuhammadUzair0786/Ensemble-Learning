# Ensemble Learning: Classifier & Regressor

This notebook demonstrates how to use ensemble learning techniques for both classification and regression tasks using Python and scikit-learn.

---

## What is Ensemble Learning?

- Ensemble learning combines predictions from multiple models to improve overall performance, robustness, and generalization.
- The main types are **Bagging** (e.g., Random Forest), **Boosting** (e.g., AdaBoost, Gradient Boosting), and **Voting/Averaging**.

---

## Types of Ensemble Learning

### 1. Bagging
- Builds multiple independent models (usually of the same type) on random subsets of the data and averages their predictions.
- Example: Random Forest.

### 2. Boosting
- Builds models sequentially, each new model focusing on correcting errors made by previous ones.
- Example: AdaBoost, Gradient Boosting.

### 3. Voting & Averaging
- **Voting Classifier:** Combines predictions from multiple classifiers (classification).  
  - *Hard voting:* Majority class wins.
  - *Soft voting:* Average of predicted probabilities.
- **Averaging Regressor:** Combines predictions from multiple regressors (regression) by averaging or weighted averaging.

---

## Steps Covered

### Classification (Voting Classifier)
- Load and explore the dataset.
- Train individual classifiers (e.g., Decision Tree, SVM, Naive Bayes).
- Combine them using `VotingClassifier`.
- Evaluate and compare individual and ensemble model performance.
- Visualize decision boundaries.

### Regression (Voting Regressor)
- Load and explore the dataset.
- Train individual regressors (e.g., Linear Regression, Decision Tree Regressor, Random Forest Regressor).
- Combine them using `VotingRegressor`.
- Evaluate and compare individual and ensemble model performance.

---

## Notes

- Ensemble methods often outperform single models, especially on complex datasets.
- Voting and averaging are simple but effective ways to combine different models.
- Bagging and boosting can further improve performance and reduce overfitting.

---

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- mlxtend (for decision boundary plots)
- Jupyter Notebook

---

This notebook is a practical guide for beginners to understand and apply ensemble learning techniques for both classification