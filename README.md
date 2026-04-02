Introduction:
A Portuguese banking institution aims to develop a predictive model that determines whether a customer will subscribe to a term deposit based on their banking behavior. To achieve this, the bank collected a dataset of past customers containing demographic details, account information, and subscription outcomes.
The dataset used in this problem is the **Bank Marketing Data Set**, which includes 17 attributes such as age, job type, marital status, education, account balance, and past campaign outcomes. Each customer is classified as either **“yes”** (subscribed) or **“no”** (did not subscribe) to a term deposit.
The primary objective of this problem set is to build a **Logistic Regression model** that predicts whether a new customer will subscribe to a term deposit. Logistic Regression is chosen for its interpretability, allowing the bank to understand how customer attributes influence the likelihood of subscription while providing a baseline predictive performance.

Approach:
Perform exploratory data analysis (EDA) to understand distributions and correlations.
Apply feature engineering (categorical encoding, scaling, and derived features).
Train classification models: Logistic Regression, Decision Tree, and Random Forest.
Evaluate performance using ROC curves, accuracy, and feature importance.

Methodology:
The modeling process followed a structured workflow to ensure clarity, reproducibility, and interpretability:

1. Data Preprocessing
Imported the Bank Marketing dataset and inspected its structure.
Handled missing values and ensured consistent formatting.
Encoded categorical variables using one-hot encoding.
Normalized numerical features where appropriate.

2. Exploratory Data Analysis (EDA)
Visualized distributions of demographic and account-related attributes.
Examined correlations between features and the target variable (subscription outcome).
Identified potential predictors such as call duration, previous campaign outcomes, and account balance.

3. Feature Engineering
Created derived features to capture campaign history and customer behavior.
Reduced dimensionality by removing redundant or low-variance attributes.

4. Model Development
Implemented **Logistic Regression** as the primary model for prediction.
Trained additional baseline models (Decision Tree, Random Forest) for   comparison.
Split the dataset into training and testing sets to evaluate generalization.

5. Model Evaluation
Assessed performance using accuracy, precision, recall, and F1-score.
Plotted ROC curves to visualize trade-offs between sensitivity and specificity.
Analyzed feature importance to interpret which attributes most influenced predictions.

6. Interpretability & Insights
Used Logistic Regression coefficients to understand the impact of customer attributes.
Compared interpretability with Random Forest feature importance rankings.
Highlighted actionable insights for the bank’s marketing strategy.

Findings:
Random Forest → achieved the highest accuracy and AUC, outperforming Logistic Regression and Decision Tree.  
Feature Importance → revealed that attributes such as ‘duration’ (call length), ‘previous’ (previous campaign outcome), and ‘outcome’ (past marketing results) were the strongest predictors.  
ROC Curves → highlighted trade-offs: Logistic Regression offered interpretability, while Random Forest maximized predictive power.  

Conclusion & Future Work:
The Bank Marketing dataset demonstrates the importance of campaign history and call duration in predicting client subscription.  
Future improvements may include:
Hyperparameter tuning for Random Forest.  
Testing Gradient Boosting or XGBoost.  
Applying SHAP/LIME for deeper interpretability.  


