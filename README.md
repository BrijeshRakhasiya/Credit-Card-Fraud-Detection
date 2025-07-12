# 💳 Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using supervised machine learning techniques. Given the highly sensitive and imbalanced nature of the dataset, special considerations were taken to preserve data authenticity while applying robust classification models.

---

## 📂 Project Overview

Credit card fraud is a serious issue in the financial sector, costing billions of dollars each year. This project explores multiple machine learning algorithms to detect potential fraudulent activities. Since the data is confidential and sensitive, balancing techniques were intentionally avoided to retain real-world behavior.

---

## 🔍 Objectives

- Understand the distribution of fraud vs. non-fraud transactions.
- Preprocess the dataset using scaling techniques.
- Train and compare various classification models.
- Evaluate model performance using precision-based metrics due to class imbalance.

---

## 🧰 Technologies Used

- **Python**
- **Jupyter Notebook**
- **Pandas**, **NumPy** for data manipulation
- **Scikit-learn** for ML models and evaluation
- **Matplotlib**, **Seaborn** for visualization

---

## 📊 Dataset

The dataset consists of anonymized credit card transactions labeled as fraudulent or non-fraudulent. For privacy reasons:
- No class balancing was performed.
- Feature scaling was applied to standardize feature distribution.

> ⚠️ Dataset contains highly imbalanced data — fraud cases are very rare compared to genuine ones.

---

## ⚙️ Preprocessing

- **StandardScaler** was applied to normalize the numerical features.
- No balancing (e.g., SMOTE/undersampling) was done to preserve original fraud distribution.
- The dataset was split into training and testing sets with stratification.

---

## 🧠 Models Used

| Model                    | Description                              |
|-------------------------|------------------------------------------|
| Logistic Regression     | Baseline model using linear decision boundary |
| Decision Tree Classifier| Non-linear, interpretable model using decision nodes |
| Random Forest Classifier| Ensemble of trees providing robustness and high accuracy |

---

## 📈 Model Performance

| Model                  | Accuracy     | Precision (Fraud) | Recall (Fraud) | F1-Score (Fraud) |
|------------------------|--------------|-------------------|----------------|------------------|
| Logistic Regression     | 0.99918      | 0.55              | 0.88           | 0.68             |
| Decision Tree Classifier| 0.99913      | 0.78              | 0.70           | 0.74             |
| Random Forest Classifier| **0.99952**  | **0.73**          | **0.95**       | **0.83**         |

> ✅ **Random Forest** delivered the best fraud detection capability with the highest recall and F1-score, which is critical in fraud detection tasks.

---

  
# Clone the repository:
 ```bash
 git clone https://github.com/BrijeshRakhasiya/Credit-Card-Fraud-Detection.git
 cd credit-card-fraud-detection
```

## 📄 License

This project is licensed under the MIT License.

---
**Made ❤️ by Brijesh Rakhasiya**
