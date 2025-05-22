# Card Swipe Chronicles — Credit Card Fraud Analysis

## 🔍 Project Overview

**Card Swipe Chronicles** is a comprehensive data analysis project focused on detecting and understanding credit card fraud patterns within a highly imbalanced transaction dataset. This project explores key fraud indicators through statistical analysis and visualizations, laying the groundwork for more advanced machine learning-based fraud detection.

---

## 📊 Dataset Summary

* **Total Transactions:** 284,807
* **Fraudulent Transactions:** 492
* **Fraud Rate:** 0.17% (highly imbalanced dataset)

---

## 💡 Key Insights

### 1. Class Distribution & Imbalance

* Fraudulent transactions are extremely rare (only 0.17%).
* Imbalance necessitates sensitive methods to detect subtle fraud patterns.
* Outliers are critical signals for identifying fraudulent activity.

### 2. Amount vs Fraud

* Most fraud transactions occur within the ₹100–₹500 range.
* High-value frauds (>₹1,000) are less frequent but still significant.
* Legitimate transactions cover a much wider amount range.

### 3. Time-based Fraud Patterns

* Fraud incidents cluster during specific hours, especially at night or early morning.
* These temporal patterns offer potential time windows for enhanced monitoring.

### 4. Feature Correlations with Fraud

| Feature | Correlation with Fraud | Interpretation                                          |
| ------- | ---------------------- | ------------------------------------------------------- |
| V17     | -0.33                  | Strong negative correlation (lower values during fraud) |
| V14     | -0.30                  | Strong negative correlation                             |
| V12     | -0.26                  | Moderate negative correlation                           |
| V10     | -0.22                  | Moderate negative correlation                           |
| V11     | +0.15                  | Mild positive correlation                               |

* Fraud transactions typically show **lower values in V17, V14, V12, V10**, which can be treated as fraud fingerprints.

### 5. Outlier Detection

* Boxplots reveal distinct outliers in fraud class for V14, V10, and V17.
* Outliers could be used as early warning indicators in real-time fraud detection systems.

### 6. Correlation Heatmap

* Most features are largely uncorrelated, which is beneficial for independent analysis.
* Slight negative correlation between `Class` and key features validates the feature importance.

---

## 🎯 Conclusion & Takeaways

* Fraudulent transactions are rare but leave identifiable patterns in the data.
* Certain features drop sharply in value during fraud events — these are strong fraud indicators.
* Time and amount data provide critical context for fraud occurrence patterns.
* This exploratory analysis narrows down key features and timeframes for future automated fraud detection models.

---

## 📸 Visualizations Included
![output](https://github.com/user-attachments/assets/0ad5b67b-5f99-463b-9ef9-594ee4825f89)
![output4](https://github.com/user-attachments/assets/8cdd49fb-901c-4ffe-9ddc-57e8d8447290)
![output3](https://github.com/user-attachments/assets/207d1bad-d4ee-4e59-89b0-4b685de58b2b)
![output2](https://github.com/user-attachments/assets/cce0aecf-ffa2-411a-a27c-ac9a0ef9f315)
![output6](https://github.com/user-attachments/assets/ff7f59bb-9b1e-44d9-adef-ddf660bab1ac)
![output5](https://github.com/user-attachments/assets/57332e59-8afa-4316-a4be-152ccdb3cbdb)

---

## 🚀 Next Steps

* Implement machine learning models using identified key features.
* Develop real-time alert systems utilizing outlier and time-based patterns.
* Explore feature engineering to enhance fraud detection accuracy.

---

## 🙌 Acknowledgements

Dataset inspired by [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud).
