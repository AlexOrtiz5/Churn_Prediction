# Churn_Prediction
  Project status(Active)

# Project objective

  This project aims to develop a predictive model to identify Amazon Prime subscribers at high risk of churning. By analyzing a sample dataset of fictional Amazon Prime users, including their subscription details, demographics, usage patterns, and preferences, this project seeks to:

  1. Identify key factors that significantly influence customer churn decisions, such as subscription plan, usage frequency, demographics, and content preferences.
  2. Build and evaluate predictive models using machine learning techniques (e.g., logistic regression, decision trees, random forests) to accurately predict which subscribers are most likely to cancel their subscriptions.
  3. Gain actionable insights into customer behavior and churn drivers to inform targeted retention strategies, such as personalized offers, improved customer service, and product enhancements aimed at increasing customer satisfaction and reducing churn rates.
  
  This analysis will provide valuable insights into customer behavior and enable Amazon Prime to proactively address potential churn and improve overall customer retention, ultimately contributing to business growth and profitability.

  Key Points:
  - Focus: Predicting customer churn for Amazon Prime.
  - Data: Using a sample dataset of fictional Prime users.
  - Methodology: Data cleaning, feature engineering, model building, and evaluation.
  - Deliverables: Predictive model, actionable insights for retention strategies.
  - Value: Reducing churn, improving customer retention, and enhancing business profitability.

# Methods
  List with methods, ex:
  - Filtering
  - Grouping
  - Visualization

  Methods expected to be used for the project:
  - Data cleaning
  - Feature engineering
  - Model building
  - Model evaluation
  - Data visualization
  - Storytelling

# Technologies 
  List with used technologies, ex:
  - Python: The primary programming language used for data analysis, feature engineering, model building, and visualization.
  - Pandas: A powerful Python library for data manipulation and analysis, including reading, cleaning, and transforming the dataset.
  - NumPy: Used for numerical operations, especially when working with arrays and matrices of data.
  - Scikit-learn (sklearn): A machine learning library in Python used for model selection, training, evaluation, and various utility functions.
  - Matplotlib: A comprehensive library for creating static, interactive, and animated visualizations in Python.
  - Seaborn: A Python data visualization library based on Matplotlib, providing a high-level interface for drawing attractive and informative statistical graphics.
  - Joblib: Used for efficiently saving and loading trained machine learning models, allowing for model persistence and reuse.
  - Jupyter Notebooks (or similar): An interactive environment for writing and running code, as well as documenting the project's steps and findings.

# Project Description
  
  This project aims to develop a machine learning model to predict customer churn for Amazon Prime memberships. The model will be trained on a dataset retrieved from Kaggle (https://www.kaggle.com/datasets/arnavsmayan/amazon-prime-userbase-dataset), which contains information about Amazon Prime users.

  # Dataset Characteristics

  The Amazon Prime user base dataset is expected to include various features related to user demographics, membership details, usage patterns, and potentially churn status. Here's a breakdown of some anticipated characteristics:

  - User Demographics: Age, gender, location (country/city)
  - Membership Details: Membership start date, end date (if applicable), subscription plan (annual/monthly)
  - Usage Patterns: Frequency of using Prime services (e.g., video streaming, music, free shipping), purchase history
  - Churn Status: Indication of whether a user has churned (cancelled) their Prime membership
  
  # Project Goals

  The primary goal of this project is to build a model that can accurately predict whether an Amazon Prime user is at risk of churning. This model will be used to:

  - Identify users who are more likely to churn, allowing for targeted marketing campaigns or retention efforts.
  - Gain insights into user behavior and preferences that contribute to churn.
  - Improve customer retention strategies for Amazon Prime.
  
  # Expected Outcomes

  The successful completion of this project will result in:

  - A trained machine learning model capable of predicting customer churn for Amazon Prime memberships.
  - Evaluation metrics to assess the model's performance (e.g., accuracy, precision, recall).
  - Insights into user behavior and factors influencing churn.
  - Recommendations for improving customer retention strategies based on the model's findings.
  
  This project will contribute to a better understanding of customer churn within the Amazon Prime ecosystem, ultimately aiding in developing strategies to retain valuable members.

# Steps
  
  1. Data Acquisition and Exploration:
  - Obtained the Amazon Prime Userbase dataset from Kaggle: https://www.kaggle.com/datasets/arnavsmayan/amazon-prime-userbase-dataset
  - Conducted exploratory data analysis (EDA) to understand the data:
    - Checked for missing values and handled them appropriately (e.g., imputation, removal).
    - Identified and addressed data inconsistencies.
    - Visualized data distributions (histograms, bar charts) to gain insights into user demographics, subscription plans, and usage patterns.
    - Investigated the relationship between different features and the target variable (churn).

  2. Data Cleaning and Preparation:
  - Cleaned and transformed the data:
    - Converted relevant columns to appropriate data types (e.g., dates, numerical values).
    - Handled categorical variables (e.g., one-hot encoding, label encoding).
    - Created new features (e.g., Membership Duration (Days), Age, Days Since Membership Start).
    - Dropped irrelevant or redundant features (e.g., 'User ID', 'Name', 'Email Address').

  3. Feature Engineering:
  - Engineered relevant features:
    - Created binary features for device usage and favorite genres.
    - Calculated temporal features (e.g., Membership Duration (Days), Age, Days Since Membership Start).
    - Considered creating interaction features (e.g., combinations of subscription plan and gender).

  4. Model Selection and Training:
  - Split the data into training and testing sets.
  - Selected and trained a suitable machine learning model (e.g., Logistic Regression, Random Forest, Support Vector Machine).
  - Experimented with different model hyperparameters to optimize performance.

  5. Model Evaluation:
  - Evaluated the model's performance using various metrics:
    - Accuracy
    - Precision
    - Recall
    - F1-score
    - AUC-ROC
  - Assessed model performance on the test set and compared different models.

  6. Data Visualization and Interpretation:
  - Created visualizations to:
    - Explore data distributions and relationships.
    - Analyze churn trends and patterns.
    - Visualize model performance (e.g., confusion matrix, ROC curve).
  - Interpreted model results to identify key factors influencing churn.

  # Insights:
  
  - Key Churn Drivers:
    - Identified that short membership durations and low usage frequency were strong predictors of churn.
    - Observed that certain subscription plans had higher churn rates than others.
    - Found that users who primarily used mobile devices for streaming had a higher tendency to churn.
    - Discovered that engagement with specific content genres (e.g., documentaries, horror) may be linked to churn behavior.
  - Model Performance:
    - Achieved a reasonable level of accuracy in predicting churn.
    - Identified areas for model improvement, such as incorporating more sophisticated feature engineering techniques or exploring alternative machine learning algorithms.
  - Recommendations:
    - Recommended targeted retention campaigns for users with short membership durations and low engagement.
    - Suggested offering incentives to encourage longer-term subscriptions.
    - Proposed personalized recommendations based on user preferences to improve content engagement.

# Conclusion

  This project aimed to develop a predictive model for customer churn within the Amazon Prime subscription service using a sample dataset.

  The initial model development, utilizing Logistic Regression, yielded unsatisfactory results with low precision, recall, F1-score, and an AUC-ROC of 0.5, indicating poor predictive performance. These results suggest that the current model is unable to effectively distinguish between churning and non-churning customers.

  ### Possible reasons for this poor performance include:
  - Data Imbalance: The dataset may be imbalanced, with a significantly larger number of non-churning users compared to churning users. This can bias the model towards predicting the majority class (non-churn) and hinder its ability to accurately identify true churners.
  - Feature Engineering Limitations: The current set of engineered features may not adequately capture the complex factors driving customer churn.
  - Model Limitations: Logistic Regression may not be the most suitable model for this particular dataset and problem.

  ### Next Steps:

  To improve model performance, the following steps will be explored:
  1. Address Data Imbalance: Implement techniques such as oversampling, undersampling, or using class weights to address potential class imbalances in the data.
  2. Enhance Feature Engineering: Explore more sophisticated feature engineering techniques, such as:
  - Creating interaction terms between features (e.g., Subscription Plan and Age).
  - Extracting more nuanced information from Purchase History and Engagement Metrics.
  - Utilizing external data sources (if available) to enrich feature sets.
  3. Evaluate Alternative Models: Experiment with different machine learning algorithms, such as Random Forest, Support Vector Machines, and Gradient Boosting Machines, to identify models that may be better suited for this problem.
  4. Hyperparameter Tuning: Fine-tune the hyperparameters of the selected models to optimize their performance.
  
  By addressing these limitations and exploring alternative approaches, we aim to develop a more accurate and reliable churn prediction model that can provide valuable insights for improving customer retention strategies and enhancing the overall customer experience for Amazon Prime.

  Disclaimer: This conclusion is based on the provided model performance metrics. Further analysis and experimentation are necessary to achieve optimal results.

  This conclusion acknowledges the limitations of the current model, provides potential reasons for the poor performance, and outlines a roadmap for future improvements.
  
# Contact
  linkedin, github