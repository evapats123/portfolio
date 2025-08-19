# 📊 Predicting Advertisement Click Likelihood Using Machine Learning

## 📌 Project Overview
This project predicts whether a user will click on an online advertisement based on demographic and behavioral features.  
By accurately predicting click likelihood, companies can:
- Optimize ad targeting
- Increase conversion rates
- Reduce wasted ad spend
- Improve customer experience by showing more relevant ads

The project compares multiple ML algorithms and a deep learning model (ANN) to determine the best-performing approach.

---

## 📂 Dataset
- **Source:** [[Specify dataset source if public](https://www.kaggle.com/datasets/gabrielsantello/advertisement-click-on-ad)]
- **Key Features:**
  - Daily Time Spent on Site (minutes)
  - Age (years)
  - Area Income (USD)
  - Daily Internet Usage (MB/day)
  - Gender
  - Clicked on Ad (target variable)

---

## 🛠️ Technologies Used
- Python (NumPy, Pandas, Seaborn, Matplotlib)
- Scikit-learn
- XGBoost
- TensorFlow/Keras

---

## 🤖 Models Implemented
1. Logistic Regression
2. Support Vector Classifier (SVC)
3. K-Nearest Neighbors (KNN)
4. Decision Tree Classifier (DT)
5. Random Forest Classifier (RFC)
6. XGBoost Classifier (XGB)
7. Artificial Neural Network (ANN)

---

## 📈 Model Performance

| Model               | Accuracy | Sensitivity | Specificity |
|---------------------|----------|-------------|-------------|
| Logistic Regression | 0.98     | 0.98        | 0.99        |
| SVC                 | 0.97     | 0.96        | 0.98        |
| KNN                 | 0.87     | 0.85        | 0.90        |
| Random Forest       | 0.99     | 0.99        | 0.99        |
| Decision Tree       | 1.00     | 1.00        | 1.00        |
| XGBoost             | 1.00     | 1.00        | 1.00        |
| ANN                 | 0.45     | 0.00        | 1.00        |

---

## 🔍 Insights from the Data
- **Age is a strong predictor:** Older users are more likely to click ads, possibly due to higher engagement with online offers or different browsing behavior.
- **High daily internet usage** correlates with lower click likelihood — frequent internet users may be more ad-aware and less likely to click.
- **Area income** shows patterns — users from middle-income areas click slightly more often than those from high-income areas.
- **Time spent on site**: Shorter browsing sessions are more associated with clicks, suggesting impulse engagement.

---

## 🏢 Business Insights & Recommendations

1. **Targeting Strategy**
   - Prioritize ad impressions for users in specific **age brackets** with higher click rates.
   - Consider adjusting ad creative for high-frequency internet users to overcome "banner blindness".

2. **Personalization**
   - Use income-based segmentation to tailor offers — middle-income groups may respond more to discount-driven messaging.
   - Deploy time-sensitive or impulse-driven ad creatives for users with short site visits.

3. **Budget Allocation**
   - Allocate a higher percentage of ad spend to segments with higher predicted click probabilities.
   - Reduce budget on low-likelihood segments to avoid wasted impressions.

4. **A/B Testing Focus**
   - Test different ad formats for high-frequency users to see if engagement improves.
   - Experiment with dynamic pricing or personalized offers for middle-income areas.

5. **Future Model Integration**
   - Integrate the best-performing model (Random Forest or XGBoost) into the ad delivery system to automatically adjust targeting in real-time.

---

## 📝 Notes
- Tree-based models achieved **100% accuracy** on this dataset, but this may indicate **overfitting**. Cross-validation or testing on a larger, unseen dataset is recommended before production use.
- ANN underperformed due to small dataset size — larger datasets and tuning could improve results.

---

## 📌 Conclusions
- **Best Models:** Decision Tree and XGBoost (highest accuracy) — suitable for quick, high-accuracy predictions.
- **Business Value:** Predictive modeling can significantly improve ROI by reducing wasted ad impressions.
- **Next Steps:** Deploy model into a live ad-serving environment, monitor results, and retrain periodically with new data.

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/ad-click-prediction.git
