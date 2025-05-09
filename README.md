# Employee Attrition Prediction

This project aims to predict employee attrition using various machine learning models including MLP, LSTM, and GridSearch-optimized classifiers. The dataset contains HR-related features, and the goal is to identify whether an employee is likely to leave the company.

## 🔍 Problem Statement
High employee turnover can be costly and disruptive. By predicting attrition early, organizations can take proactive steps to retain talent.

## 🧠 Models Used
- **MLP (Multi-layer Perceptron)**: Basic neural network model
- **LSTM (Long Short-Term Memory)**: Deep learning model for sequence data
- **GridSearchCV**: For hyperparameter tuning of classic ML models

## 🧪 Results Summary
After balancing the dataset and testing several models:

| Model       | Accuracy | F1-score (class 1) |
|-------------|----------|--------------------|
| MLP         | 15.9%    | 0.27               |
| LSTM        | 86.8%    | 0.38               |
| GridSearch  | 85.4%    | 0.49               |

⚠️ Class 1 (employees who leave) had lower recall, indicating the challenge of class imbalance.

## 🛠 Requirements
- Python 3.x
- pandas
- numpy
- scikit-learn
- keras / tensorflow
- matplotlib / seaborn (for visualizations)

You can install dependencies with:
```bash
pip install -r requirements.txt
📊 Observations
Dataset was highly imbalanced, requiring SMOTE-style oversampling

LSTM offered best overall accuracy, but classic models performed more consistently

✍️ Author
Zahra Jamalou
