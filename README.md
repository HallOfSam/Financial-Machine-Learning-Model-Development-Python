# Overview

- The project aims to predict European call option values on the S&P 500 using machine learning models. A few variables in Black-Scholoes (BS) formula are used as predictors in our models, including current option value (Value), current asset value (S), strike price of the option (K), annual interest rate (r), time to maturity (tau), and the prediction made by the Black-Scholes equation (BS) denoted as “under” or “over''.

- We build regression models to predict option values, and classification models to classify whether Black-Scholes equation prediction overestimated (“over”) or underestimated (“under”) the European call option value. 

- To select the best regression model, we compare various models based on the mean R-squared of 5-fold Cross-Validation, including linear regression, Decision Tree, Random Forest, KNN regression, Boosting (XGBoost), and SVM. For the classification model selection, we evaluate different models -including KNN, Logistic, LDA, Naive Bayes, Decision Tree, Random Forest, Boosting, and SVM- based on the mean classification error of Stratified 5-fold CV. We found out in terms of predicting European options values and classifying BS’s prediction (using 0 for “under” and 1 for “over”), Random Forest regressor (mean R-squared of 0.9959) and Boosting (mean classification error of 6.57%) classifier performed the best.

- In conclusion, machine learning models can enhance investment decision-making by helping us detect whether traditional statistical methods (such as the Black-Scholes equation) overestimate or underestimate option prices. More importantly, machine learning models might offer more accurate predictions when traditional models don’t work well, given their high mean R-squared of 0.9959 in our prediction of European call option prices.

# Note

- For more details, please refer to "report.pdf".
