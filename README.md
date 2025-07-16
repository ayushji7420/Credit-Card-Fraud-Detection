# Credit Card Fraud Detection

This project focuses on detecting fraudulent transactions in a highly imbalanced dataset using various machine learning models and techniques.

## 📌 Dataset

- The dataset contains transactions labeled as **Fraudulent** and **Legitimate**.
- Due to severe class imbalance (~0.17% fraud), custom sampling strategies were used for splitting.

## 📊 Data Splitting

- **Training Set:** 70% of fraud cases + 50% of legit transactions.
- **Testing Set:** 30% of fraud cases + 50% of legit transactions.
- **Balancing:** Applied **ADASYN (Adaptive Synthetic Sampling)** on the training data to handle class imbalance.

## ⚙️ Models Used

- Logistic Regression
- Random Forest
- Decision Tree
- XGBoost
- Artificial Neural Network (ANN)

## 🔍 EDA and Feature Selection

- Performed Exploratory Data Analysis to understand patterns in the data.
- Removed columns with low or no correlation with the target class to improve model performance.

## 📈 Performance

- **Initial Results:**  
  - Best Recall: 90% (Logistic Regression)  
  - Best ROC-AUC: Logistic Regression (0.87), ANN (0.86)  
  - Other models performed poorly on raw data.

- **Post Feature Selection:**  
  - All models showed significant improvement.  
  - Recall scores for all models were above **70%**.  
  - ROC-AUC scores for all models exceeded **0.80**.  
  - Logistic Regression achieved the highest recall, while ANN and XGBoost achieved the highest ROC-AUC.

## ✅ Conclusion

- Demonstrates the critical role of feature selection in improving fraud detection performance.
- Shows the value of comparing multiple models and balancing precision-recall trade-offs for imbalanced data.

## 📚 Libraries Used

- Python (pandas, scikit-learn, XGBoost, Keras/TensorFlow)
- Matplotlib / Seaborn for visualization

---

**Author:** [Ayush Sharma]  
**Contact:** [aaayushsharmaji@gmail.com]
