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

* Class distribution pie chart
* Boxplots comparing V14, V10, V17 feature distributions by transaction class
* Histogram of fraud occurrences by hour of day
* Correlation heatmap of key features and fraud class

---

## 🚀 Next Steps

* Implement machine learning models using identified key features.
* Develop real-time alert systems utilizing outlier and time-based patterns.
* Explore feature engineering to enhance fraud detection accuracy.

---

## 📂 Project Files

* `card_swipe_analysis.ipynb` — Jupyter notebook with full exploratory data analysis
* `visualizations/` — Folder containing all charts and graphs
* `data/` — (Link or instructions to download dataset if public)

---

## 🙌 Acknowledgements

Dataset inspired by [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud).

---

Feel free to copy this directly or ask me if you want me to tailor it with badges, contribution guidelines, or install instructions! Would you like help drafting those too?
