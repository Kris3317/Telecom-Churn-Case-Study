# Telecom-Churn-Case-Study
> To build ML models to predict churn for a telecom company. 

## Table of Contents
* [Problem Statement & Objeective](#1)
* [Analysis Steps](#2)
* [Libraries Used](#3)
* [Conclusions & Recommendations](#4)
* [Acknowledgements](#5)
* [Contact](#6)

## <a name="1">Problem Statement & Objective</a>
- In a highly competitive telecommunications market, customer churn poses a significant challenge for companies seeking to maintain profitability and market share. To address this issue, a leading telecom company aims to leverage machine learning (ML) models to predict customer churn and identify key factors driving customer attrition.

- Churn Prediction Model:
  * Develop ML models to predict whether high-value customers are likely to churn in the near future.
  * Utilize predictive analytics to anticipate churn behavior, enabling proactive intervention strategies such as tailored retention offers and personalized services.
  * Evaluate model performance using metrics like accuracy, precision, recall, and F1-score to assess predictive capability and identify customers at risk of churn with higher accuracy.
- Identification of Churn Drivers:
  * Construct a model to identify important predictor attributes that influence customer churn decisions.
  * Utilize techniques such as logistic regression or decision trees to interpret and extract actionable insights from the data.
  * Analyze feature importance to understand the underlying factors contributing to churn, enabling strategic decision-making and targeted interventions.

## <a name="2">Analysis Steps</a>
-Missing Values Handling: Columns with more than 30% missing values were dropped.
-Variance Thresholding: Columns with less than 25% variance were removed.
-Isolating Non-Numerical Variables: Non-numerical columns were identified.
-Handling Date Variables: Date variables were transformed to only include the day of the month.
-Handling Missing Values: Missing values were identified and analyzed.
    
## <a name="3">Libraries Used</a>
-pandas
-numpy
-matplotlib
-seaborn
-scikit-learn
-xgboost
-imbalanced-learn

## <a name="4">Conclusions & Recommendations</a>
- Logistic regression was applied as the first model.
- Hyperparameter tuning was performed using GridSearchCV to find the best parameters.
- The logistic regression model was evaluated using various metrics like AUC, accuracy, precision, recall, F1 score, and root mean squared error (RMS).
- XGBoost classifier was applied as another model.
- Hyperparameter tuning was performed using RandomizedSearchCV.
- Since the primary concern is to ensure that positives (e.g., identifying customers who will churn) are correctly classified, rather than focusing on minimizing false negatives, then precision becomes the most important metric. Precision measures the proportion of true positive predictions out of all positive predictions made by the model. In other words, it evaluates the model's ability to avoid false positives. A higher precision indicates fewer false positives, meaning that the model is better at correctly identifying customers who will churn without mistakenly classifying too many non-churners as churners.
- Therefore, in this scenario, where the emphasis is on getting the positives right, the model with the highest precision would be considered the best choice and therefore we can proceed with the XGBoost model with the hyperparameters seen above.

## <a name="5">Acknowledgements</a>
- This project is a part of the Executive PG Programme in Machine Learning & AI curated by upGrad.
- If you too would like to be a part of this extremely informative and detailed Exec Programme, enroll yourself [here](https://app.upgrad.com/4Xxq/4zgb85pa) and feel free to use my referral code (ZlrGO7) to avail high fee waivers.

## <a name="6">Contact</a>
- Created by the [owner](https://github.com/Kris3317/) of this Repo, surprise.
- Feel free to contact me on [LinkedIn](https://www.linkedin.com/in/krismichaeldsilva/)
