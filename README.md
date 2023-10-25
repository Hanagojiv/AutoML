# AutoML for World Happiness Prediction

## Abstract

The objective of this notebook is to predict the happiness scores of countries worldwide based on various factors, such as economic production, social support, life expectancy, freedom, absence of corruption, and generosity. The analysis leverages the World Happiness Report, a publication by the United Nations Sustainable Development Solutions Network, which ranks national happiness and explores the data behind these rankings.

In this project, we employ AutoML, specifically the H2O AutoML tool, to address the following questions:

1. Is the relationship between predictor variables and happiness scores significant?
2. Are any model assumptions violated, and does multicollinearity exist in the model?
3. Do the predictor variables demonstrate independence from one another in multivariate models?
4. Can we rank the most significant predictor variables and exclude insignificant ones from the model?
5. Does the model align with the data, and does regularization improve its performance?
6. Which independent variables significantly influence happiness scores?
7. What hyperparameters are crucial for model performance?

The notebook begins by analyzing the data for correlation, multicollinearity, significance, and overall data quality. Subsequently, H2O AutoML is employed to train the data using ten different models, and the best model's performance is evaluated.

## Information about the Dataset

**Target Variable/Dependent Variable**:
- **Happiness Score**: A metric measured in 2015 by asking sampled individuals to rate their happiness on a scale of 0 to 10, where 10 represents the highest level of happiness.

**Predictor Variables/Independent Variables**:
1. **Country**: Name of the country.
2. **Region**: Region or continent to which the country belongs.
3. **Happiness Rank**: Ranking of countries according to their happiness scores.
4. **Standard Error**: Standard error of the happiness score.
5. **Economy (GDP per Capita)**: Measures the monetary value of the final goods and services and its contribution to the Happiness score.
6. **Family**: Contribution of family values to the Happiness score.
7. **Health (Life Expectancy)**: Contribution of health and life expectancy to the happiness score calculations.
8. **Freedom**: Contribution of freedom to the calculation of the Happiness score.
9. **Trust (Government Corruption)**: Impact of trust and government corruption values on the Happiness score.
10. **Generosity**: Reflects the quality of being kind and generous.
11. **Dystopia Residual**: The sum of the dystopia happiness score, representing a hypothetical country with a rank lower than the lowest-ranking country in the report.

## Understanding the Results

Several metrics are utilized to understand the performance of the model. These include Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), Root Mean Squared Log Error (RMSLE), Mean Residual Deviance, and the Coefficient of Determination (R-squared or R^2). These metrics help assess the accuracy and explanatory power of the model.

## Interpreting Feature Importance

Feature importance analysis highlights the significance of predictor variables. In this dataset, Dystopian Residual has the most substantial impact on the prediction outcome, followed by Economy (GDP per Capita), Health (Life Expectancy), Generosity, and Trust (Government Corruption).
<img width="743" alt="Screenshot 2023-10-25 at 10 05 12 AM" src="https://github.com/Hanagojiv/AutoML/assets/114262882/b767f59e-24da-40f0-bd68-f7d7dc9bef42">


## Model Significance and Assumptions

- The relationship between predictor variables and happiness scores is highly significant, with an R-squared value of 1.
- The model's assumptions are not violated, as the regression model is suitable for this dataset.
- Multicollinearity exists among predictor variables, as observed from the VIF data.

## Model Performance and Regularization

- Regularization does not improve model performance, as the RMSE for the best model is lower without regularization.
## Training 10 models by AutoML
<img width="1190" alt="Screenshot 2023-10-25 at 10 08 50 AM" src="https://github.com/Hanagojiv/AutoML/assets/114262882/6185b1b3-8301-40f0-8952-2f8efec3d2bf">

## Interpretting the above training output
The reported metrics are for the Generalized Linear model in H2O AutoML. The metrics are reported separately for the training data and the cross-validation data.

For the training data:
- Mean Squared Error (MSE) is 0.0006774, which measures the average squared difference between the predicted and actual values.
- Root Mean Squared Error (RMSE) is 0.0260, which is the square root of MSE and provides a measure of how well the model fits the data.
- Mean Absolute Error (MAE) is 0.01989, which measures the average absolute difference between the predicted and actual values.
- Root Mean Squared Log Error (RMSLE) is 0.0049, which is the RMS of the logarithmic differences between the predicted and actual values.
- R-squared (R^2) is 0.9995, which is a measure of how well the model fits the data. The Null deviance, residual deviance, and AIC are also reported.

For the cross-validation data:
- The metrics are little worse as compared to the training data, which is expected since the model was not trained on this data.
- The R^2 is 0.99, which is reasonable fit.


## Coding Professionalism

The code and project adhere to best practices in coding and data analysis, ensuring professionalism throughout.


## Conclusion

In this notebook, we harnessed H2O AutoML to train, evaluate, and explain machine learning models for predicting happiness scores based on a variety of predictor variables. The results indicate a high level of significance and provide valuable insights into the relationship between these variables and happiness scores.

## References

- AI Skunks AutoML notebook references.
- H2O.AI (https://www.h2o.ai/)
- YouTube: H2O (https://www.youtube.com/user/0xdata)
