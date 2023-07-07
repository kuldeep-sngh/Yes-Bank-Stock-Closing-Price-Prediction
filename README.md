# Yes-Bank-Stock-Closing-Price-Prediction

![image](https://github.com/kuldeep-sngh/Yes-Bank-Stock-Closing-Price-Prediction/assets/112714096/10b35ee2-aa57-442d-aded-1f3f51ba193a)

## Problem Statement
This report presents the capstone project conducted by Almabetter, focusing on addressing an ML-Regression problem. The project centers around the analysis of Yes Bank's stock price dataset, a prominent financial institution in the Indian banking sector. Notably, Yes Bank has gained significant media attention since 2018 due to a high-profile fraud case involving Rana Kapoor. The dataset encompasses monthly stock prices spanning the bank's entire operational history, providing essential information such as monthly closing, opening, highest, and lowest stock prices. The primary goal of this project is to develop a predictive model for estimating the closing price of Yes Bank's stock for each month.

## Dataset Description
**shape :** Dataset has 185 rows and 5 columns.

**columns :**
* Date : Date of record
* Open : Opening price
* High : Highest price in the month
* Low : Lowest price in the month
* Close : Closing price

## Course of action
* Data inspection and data cleaning.
* Exploratory Data Analysis (EDA)
* Data preparation.
* Model Implementation and evaluation.
* Explain the model using SHAP model explainability tool.

our initial steps involved data inspection and data cleansing to ensure the dataset's quality and integrity. We imported the necessary libraries and loaded the dataset, followed by a thorough examination of the data for any missing values, inconsistencies, or outliers. After addressing these issues through data cleansing techniques, we proceeded to perform Exploratory Data Analysis (EDA) to gain insights into the dataset's characteristics, including statistical properties, distributions, and correlations between variables. During the EDA phase, we also conducted hypothesis testing and analyzed outliers. Subsequently, we performed data manipulation, feature engineering, and data preprocessing to prepare the dataset for modeling. We implemented various ML models, such as Linear Regression, Ridge, Lasso, ElasticNet for regularization, Random Forest Regressor, and XGBoost Regressor, recording and evaluating their respective performance metrics. Finally, to enhance model interpretability, we utilized the SHAP model explainability tool, providing valuable insights into the importance of different features in influencing stock price predictions.

![image](https://github.com/kuldeep-sngh/Yes-Bank-Stock-Closing-Price-Prediction/assets/112714096/84a4eb1d-ab73-41d9-8f3e-e0df2a9a9b90)

## Random Forest

![image](https://github.com/kuldeep-sngh/Yes-Bank-Stock-Closing-Price-Prediction/assets/112714096/2632f34b-ed31-437e-8582-ce82d5526066)

Random Forest is an ensemble learning technique that combines the predictions of multiple decision trees to enhance prediction accuracy and robustness. It operates through two main mechanisms: data sampling and feature randomness. During data sampling, subsets of the original training data are randomly selected with replacement to create bootstrap samples, which are used to train individual decision trees. Feature randomness is introduced by considering only a random subset of features at each split in a tree. By training diverse decision trees and aggregating their predictions, Random Forest reduces overfitting and improves overall performance. In classification tasks, the final prediction is determined through majority voting, while regression tasks involve averaging the predictions of all trees. The combination of diverse decision trees and ensemble prediction makes Random Forest a powerful and widely-used algorithm for various machine learning applications.

## XGBoost

![image](https://github.com/kuldeep-sngh/Yes-Bank-Stock-Closing-Price-Prediction/assets/112714096/ffac0cf5-9a6e-43b6-bf0d-66f18714cb20)

XGBoost is a powerful ensemble learning technique that combines the predictions of multiple decision trees to improve prediction accuracy. It uses a gradient boosting algorithm to iteratively train new trees, correcting the errors made by previous trees. By randomly selecting subsets of training data and considering only a subset of features at each split, XGBoost creates diverse and accurate decision trees. This approach allows XGBoost to handle regression and classification tasks effectively while capturing complex relationships in the data. With its ability to prevent overfitting and achieve high performance, XGBoost is widely recognized and utilized in various machine learning applications.

## Conclusion on model implementation
After initial evaluation with Linear Regression as our base model, we obtained moderate training and testing scores of 0.82 and 0.76, respectively. However, both the Mean Squared Error (MSE) and Mean Absolute Error (MAE) metric scores were relatively high. To enhance our predictions, we implemented Ridge, Lasso, and ElasticNet regularization models. Among these, the Lasso model emerged as the top performer, exhibiting an impressive R-squared score of 0.83 and significantly reducing the MSE and MAE compared to the base model.

Expanding our analysis, we incorporated the Random Forest Regressor and XGBoost Regressor models, which outperformed the previous approaches across various metrics. Notably, the XGBoost Regressor slightly outperformed the Random Forest Regressor, as evidenced by the metric score chart. As a result, we selected XGBoost Regression as our final model for predicting stock prices due to its superior performance compared to all other models utilized in this project.

### Evaluation metric score chart

![Screenshot (5)](https://github.com/kuldeep-sngh/Yes-Bank-Stock-Closing-Price-Prediction/assets/112714096/3b60e318-0401-462f-a630-73cc30a82115)


