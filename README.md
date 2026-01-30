# AI-ML-INTENSHIP-TASK--9
 Random Forest – Credit Card Fraud Detection
 # Credit Card Fraud Detection using Machine Learning

This project focuses on detecting fraudulent credit card transactions using machine learning techniques.  
Due to the highly imbalanced nature of fraud datasets, the project emphasizes **precision, recall, and F1-score** rather than accuracy.

---

##  Dataset
- **Source:** Credit Card Transactions Dataset
- **Target Column:** `Class`
  - `0` → Non-Fraud  
  - `1` → Fraud  
- The dataset is highly imbalanced, with fraud transactions forming a very small percentage.

---

##  Project Workflow

1. Load dataset and analyze fraud vs non-fraud class distribution.
2. Separate input features and target variable.
3. Remove non-useful identifier columns.
4. Split data using **stratified sampling** to preserve fraud ratio.
5. Train a **Logistic Regression** model as a baseline.
6. Train a **Random Forest Classifier** for improved performance.
7. Evaluate models using **precision, recall, and F1-score**.
8. Visualize **feature importance** to identify key fraud indicators.
9. Save the best-performing model using `joblib`.

---

##  Models Used

- **Logistic Regression** (Baseline Model)
- **Random Forest Classifier**
  - `n_estimators = 100`
  - Handles non-linear relationships and feature interactions well

---

##  Evaluation Metrics

Since fraud detection is a class-imbalanced problem, the following metrics are used:

- Precision  
- Recall  
- F1-Score  

> Accuracy is not reliable for fraud detection due to class imbalance.

---

##  Feature Importance

Random Forest feature importance is used to identify the most influential features contributing to fraud detection.

![Feature Importance](feature_importance.png)

---

##  Model Saving

The trained Random Forest model is saved for reuse:


