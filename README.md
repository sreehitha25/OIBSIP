# Task 1 — Iris Flower Classification

## Objective
Build a machine learning model that classifies an iris flower into one of three species — *Setosa*, *Versicolor*, or *Virginica* — based on four measurements: sepal length, sepal width, petal length, and petal width.

## Dataset
The classic Iris dataset (150 samples, 3 classes, 4 features). Loaded directly via `sklearn.datasets.load_iris()`, so no external download is required.

## Approach
1. Load and explore the data (shape, class balance, summary stats)
2. Visualize feature relationships (pair plots, correlation heatmap)
3. Split into train/test sets
4. Train and compare classification models (Logistic Regression, Decision Tree, KNN)
5. Evaluate using accuracy, confusion matrix, and classification report
6. Save the best-performing model

## Results
Three models were trained and compared on a held-out test set (20% of the data):

| Model | Accuracy |
|---|---|
| Logistic Regression | 96.7% |
| Decision Tree | 93.3% |
| **K-Nearest Neighbors** | **100%** |

K-Nearest Neighbors (k=5) was selected as the best model, achieving perfect classification on the test set with precision, recall, and F1-score of 1.00 for all three species.

## Files
- `iris_classification.ipynb` — full notebook with code, plots, and explanations
- `iris_model.pkl` — saved trained model (optional)

## How to run
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook iris_classification.ipynb
```
