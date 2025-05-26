# 🧠 Predicting Digital Wellbeing with Machine Learning

This project explores how various digital behavior and psychological features influence an individual's digital wellbeing. I applied different regression models to predict the **Digital Wellbeing Score** based on features like anxiety level, focus, sleep hours, app usage, and more.

---

## 📂 Project Structure

- `dataset.csv` – The dataset containing behavioral and psychological indicators.
- `linear_regression_pipeline.pkl` – Saved model pipeline for deployment.
- Jupyter Notebook or Python scripts – Used for data analysis, model training, and evaluation.

---

## 🎯 Objective

To build a predictive model that accurately estimates digital wellbeing scores using key digital behavior and psychological metrics. I compared multiple machine learning algorithms and selected the best-performing one based on performance metrics.

---

## 📊 Dataset Summary

The dataset includes the following key features:

- `anxiety_level`
- `sleep_hours`
- `focus_score`
- `social_media_time_min`
- `mood_score`
- `num_app_switches`
- `notification_count`
- `daily_screen_time_min`
- Target: `digital_wellbeing_score`

---

## 🧪 Methodology

Here’s a summary of what I did:

1. **Data Loading & Cleaning** – Removed duplicates, explored datatypes, and handled missing values.
2. **Exploratory Data Analysis (EDA)** – Plotted histograms, correlation heatmaps, and summary stats.
3. **Feature Scaling** – Applied `StandardScaler` using a pipeline.
4. **Model Building** – Trained four regression models:
   - Linear Regression ✅ (Best)
   - Random Forest Regressor
   - Decision Tree Regressor
   - Support Vector Regressor (SVR)
5. **Evaluation Metrics** – Used `R²`, `MAE`, and `MAPE` for model comparison.
6. **Feature Importance** – Interpreted both coefficients and model-based importance.
7. **Cross-validation** – Performed k-fold validation to confirm model reliability.
8. **Model Export** – Saved the best pipeline using `joblib`.

---

## ⚖️ Model Comparison

| Model                   | R² Score | MAE   | MAPE (%) |
|------------------------|----------|-------|-----------|
| **Linear Regression**  | 0.9996   | 0.015 | 0.018     |
| Random Forest          | 0.9989   | 0.021 | 0.024     |
| Decision Tree          | 0.9910   | 0.046 | 0.050     |
| SVR                    | 0.9396   | 0.094 | 0.095     |

✅ Linear Regression performed best and was selected as the final model.

---

## ✅ Final Model: Linear Regression

- **Why I Chose It**:  
  It had the highest R² and lowest error metrics. Also, it’s interpretable — I could extract and explain the importance of each feature using the model coefficients.

- **Model Export**:  
  Saved as `linear_regression_pipeline.pkl` using `joblib` for deployment or integration.

---

## 📌 Recommendations

Based on the analysis, I recommend:

- **Focus on Mental Health Interventions**: Anxiety level is the top predictor. Programs targeting stress and anxiety may greatly improve digital wellbeing.
- **Encourage Better Sleep Habits**: Sleep hours had the second most impact. Well-rested users show better digital wellbeing.
- **Promote Digital Focus**: Reducing notifications, app switching, and unnecessary screen time could improve focus and mood.
- **Minimize Social Media Overuse**: Time spent on social platforms was negatively correlated with wellbeing. Setting limits may help.

---

## 🎯 Conclusion

This project helped me:

- Understand the key psychological and behavioral features that impact digital wellbeing.
- Successfully apply and compare different regression algorithms.
- Build a highly accurate prediction model using clean machine learning pipelines and robust evaluation metrics.

---

## 🚀 Future Work

- 🧪 Deploy the model into a web app using Streamlit or Flask.
- 🔁 Integrate real-time data from mobile sensors or apps.
- 📈 Extend the model to predict specific mental health outcomes (e.g., depression risk).

---

## 📬 Contact

Feel free to reach out if you're interested in collaborating or discussing more about this project.

**Author:** *Tolulope Emuleomo*
**Email:** *Tolulope.emuleomo@outlook.com*

---
