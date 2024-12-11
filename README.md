# 🤖 AutoML for 🌍 World Happiness Prediction

## 📄 Abstract

This study 🧠 predicts national 😊 happiness scores by evaluating key 💰 socio-economic indicators, including 🏭 economic output, 👨‍👩‍👧‍👦 social support, 🏥 life expectancy, 🗽 individual freedoms, ⚖️ governmental integrity, and 🤲 societal generosity. Data from the World Happiness Report, published by the 🏢 United Nations Sustainable Development Solutions Network, enables predictive modeling through the ⚙️ H2O AutoML platform, revealing complex variable interactions.

The research explores several key 🔍 questions:

1. 📊 How do 💰 socio-economic predictors explain national 😊 happiness?
2. 🧩 Are core statistical assumptions (e.g., multicollinearity) violated?
3. 🔗 How do predictors interact in complex multivariate contexts?
4. ⭐ Which variables are the most significant contributors to 😊 happiness?
5. 📈 Does regularization enhance model performance?
6. ⚙️ What hyperparameters optimize predictive accuracy?
7. 🌐 How generalizable is the model across diverse geopolitical contexts?

The study begins with 📚 dataset evaluation, followed by 🤖 machine learning model development using ⚙️ H2O AutoML. Predictive performance is assessed using advanced 🔬 statistical metrics.

## 🗂️ Dataset Information

### 🎯 Target Variable (Dependent Variable):
- **😊 Happiness Score:** Self-reported life satisfaction on a 0-🔟 scale, with 🔟 indicating maximum well-being.

### 📊 Predictor Variables (Independent Variables):
1. **🌍 Country:** Nation being evaluated.
2. **📍 Region:** Geopolitical classification.
3. **🏆 Happiness Rank:** Relative ranking by happiness score.
4. **📐 Standard Error:** Measurement variability.
5. **💰 Economy (GDP per Capita):** National economic output.
6. **👨‍👩‍👧‍👦 Family:** Social and familial support.
7. **🏥 Health (Life Expectancy):** Public health indicators.
8. **🗽 Freedom:** Perceived personal autonomy.
9. **🚫 Trust (Government Corruption):** Institutional integrity and absence of corruption.
10. **🤲 Generosity:** Charitable behavior and social goodwill.
11. **🏚️ Dystopia Residual:** Minimum theoretical happiness benchmark.

## 📏 Model Performance Metrics

Model performance is evaluated using several key 📈 statistical measures:

- **📉 Mean Squared Error (MSE):** Average prediction error.
- **📊 Root Mean Squared Error (RMSE):** Standard deviation of prediction errors.
- **📐 Mean Absolute Error (MAE):** Average prediction magnitude.
- **🔢 Root Mean Squared Log Error (RMSLE):** Log-scaled prediction error.
- **📈 R-squared (R²):** Explained variance proportion.

## 🌟 Feature Importance Analysis

The following features significantly impact 😊 happiness prediction:

<img width="743" alt="Screenshot 2023-10-25 at 10 05 12 AM" src="https://github.com/Hanagojiv/AutoML/assets/114262882/b767f59e-24da-40f0-bd68-f7d7dc9bef42">

- **🏚️ Dystopia Residual:** Most critical determinant.
- **💰 Economy (GDP per Capita):** Key economic indicator.
- **🏥 Health (Life Expectancy):** Vital well-being metric.
- **🤲 Generosity:** Reflects societal altruism.
- **🚫 Trust (Government Corruption):** Indicates public trust.

## 🔍 Model Assumptions & Insights

- **📊 Predictive Significance:** All variables meaningfully impact 😊 happiness.
- **📐 Assumption Validity:** Statistical tests confirm model assumptions.
- **🧩 Multicollinearity:** Managed through dimensionality reduction and regularization.
- **🛠️ Regularization Impact:** Enhances stability while reducing overfitting.

## 🤖 Model Training with ⚙️ H2O AutoML

The project used ⚙️ H2O AutoML for 🤖 model training, selecting a Generalized Linear Model (GLM) as the best-performing algorithm.

<img width="1190" alt="Screenshot 2023-10-25 at 10 08 50 AM" src="https://github.com/Hanagojiv/AutoML/assets/114262882/6185b1b3-8301-40f0-8952-2f8efec3d2bf">

### 📊 Training Data Metrics:

- **📉 MSE:** 0.0006774
- **📊 RMSE:** 0.0260
- **📐 MAE:** 0.01989
- **🔢 RMSLE:** 0.0049
- **📈 R²:** 0.9995

### 📈 Cross-Validation Metrics:

- Slightly lower scores on unseen data (**📈 R² = 0.99**), indicating strong generalization.

## 💻 Coding & Documentation Standards

The project follows best practices in 📊 data science, 💾 software engineering, and 🎓 academic research. The codebase is modular, scalable, and well-documented to ensure 📑 reproducibility and 🔬 methodological transparency.

## 🏁 Conclusion

The ⚙️ H2O AutoML framework demonstrates exceptional performance in predicting 😊 happiness scores using 💰 socio-economic indicators. The findings reveal complex relationships among economic, social, and political factors, offering significant insights for evidence-based 🌍 policy development aimed at improving global well-being.

## 📚 References

- ⚙️ H2O.AI: [https://www.h2o.ai/](https://www.h2o.ai/)
- 🎥 YouTube: H2O Channel [https://www.youtube.com/user/0xdata](https://www.youtube.com/user/0xdata)

