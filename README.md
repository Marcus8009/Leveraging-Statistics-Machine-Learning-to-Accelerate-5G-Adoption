# Leveraging Statistics & Machine Learning to Accelerate 5G Adoption

## Project Overview
Our group project, titled **"Leveraging Statistics & Machine Learning to Accelerate 5G Adoption,"** focuses on using advanced machine learning techniques to identify potential 5G users. This strategic approach aims to enhance targeted marketing campaigns and optimize resource allocation, crucial for driving 5G adoption in the telecommunications sector.

## Business Problem
The core business problem we addressed was the accurate identification of potential 5G users. This is essential for executing targeted marketing campaigns and optimizing resource allocation, ensuring efficient use of resources and maximizing the adoption rate of 5G technology.

## Dataset Introduction
We utilized a real dataset from a telecommunications company, comprising 140,000 records with 43 feature variables and one target variable. The feature variables included user identification, consumer behavior, broadband information, and more, while the target variable indicated whether a user converted to 5G in a given month.

## Data Preprocessing
Data preprocessing was a critical step to ensure data quality and reliability. We handled default values in both categorical and numerical variables:
- **Categorical Variables:** Missing values in variables like `user_level` and `segment` were filled with the mode.
- **Numerical Variables:** Missing values were filled with the median.
- **Record Removal:** Records with multiple default values were removed to maintain data integrity.

## Exploratory Data Analysis (EDA)
EDA revealed significant insights into the data distribution and key patterns:
- **User Distribution:** The dataset was highly imbalanced, with non-5G users constituting 80% of the total.
- **User Segments:** Corporate users had the highest 5G conversion rate, while campus users had the lowest.
- **User Levels:** Starting from user level 4, the 5G conversion rate was significantly higher.

## Key Variables and Trends
Several key variables were identified as influential in 5G adoption:
- **Average Revenue Per User (ARPU):** Higher ARPU correlated with higher 5G adoption.
- **Data Usage (DOU):** Users with higher data usage were more likely to switch to 5G.
- **Minutes of Usage (MOU):** Increased usage time correlated with higher 5G adoption.
- **Broadband Bandwidth:** Users with higher bandwidth were more inclined to adopt 5G.
- **User Tenure:** Longer tenure correlated with higher 5G conversion rates.

## Feature Engineering
Feature engineering involved creating new features based on past three months' data to track averages and trends:
- **Trend Features:** Monthly growth rates for ARPU, DOU, and MOU.
- **Average Features:** Three-month averages for various metrics.
- **Feature Selection:** We dropped highly correlated features to avoid issues during model training.

## Model Preparation and Evaluation
We employed several machine learning models, evaluated using 5-fold cross-validation and metrics like accuracy, precision, recall, ROC AUC, and F1 score. Here’s a detailed description of each model:

### Logistic Regression
- **Performance:** Achieved an accuracy of 81.43% and a recall of 81.18%.
- **Description:** Logistic Regression estimates class probabilities for binary classification by applying the logistic function to a linear combination of input features. It provided a balanced performance across all metrics.

### K-Nearest Neighbors (KNN)
- **Performance:** Stood out with the highest recall (96.80%) but lower precision (80.10%).
- **Description:** KNN is an instance-based learning method that classifies a sample based on the majority class of its K-nearest neighbors. It was highly effective at identifying positive class users, aligning with our business goal of accurately recognizing potential 5G users.

### Random Forest
- **Performance:** Balanced performance with an accuracy of 90.42% and a recall of 90.14%.
- **Description:** Random Forest builds multiple decision trees using different subsets of the data and combines their predictions. It reduces overfitting and performs well on both training and testing data.

### XGBoost
- **Performance:** High precision (92.09%) but lower recall (84.40%).
- **Description:** XGBoost is a gradient boosting framework that builds multiple weak learners sequentially. It excels in handling imbalanced data and is highly efficient for large datasets.

## Model Comparison
The comparison of models highlighted:
- **KNN:** Best for identifying potential 5G users due to its high recall.
- **Random Forest:** Effective at balancing sensitivity and specificity.
- **XGBoost:** Excels at minimizing false positives with the highest precision.

## Business Strategies
Based on our analysis, we proposed several business strategies:
- **Target High-Spending Users:** Promote premium 5G plans with enhanced features.
- **Focus on Home Users:** Offer family shared data plans and 5G-enabled smart home solutions.
- **Prioritize Broadband Users:** Provide prioritized data speeds and seamless network transitions.

## Model Application in Business
Our machine learning models can be applied to:
- **Network Resource Optimization:** Prioritize 5G base station deployment in areas with high potential users.
- **Targeted Outreach:** Use data-driven insights for precise marketing.
- **Precision Marketing:** Tailor 5G plans based on user behavior and provide proactive support to accelerate 5G adoption.

## Conclusion
This project demonstrates a data-driven strategy to maximize customer adoption and resource optimization, securing a competitive position in the 5G market. By leveraging machine learning, we can effectively target potential 5G users, optimize marketing efforts, and enhance network deployment strategies.

Machine Learning for 5G adoption.pdf shows a pdf version of the final presentation.
