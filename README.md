# credit_card_fraud_analysis

2. Project Description: This project focuses on performing an in-depth exploratory data analysis (EDA) and visualization on a real-world credit card transaction dataset to detect fraudulent activities. The primary goal is to understand patterns, trends, and anomalies within the data that can distinguish fraudulent transactions from legitimate ones, addressing the critical challenge of credit card fraud.

3. Dataset: The dataset creditcard.csv contains credit card transactions over two days in September 2013 by European cardholders. It features 28 principal components (V1-V28) obtained with PCA transformation, along with Time (seconds elapsed from the first transaction), Amount, and Class (0 for legitimate, 1 for fraudulent).

Key Characteristic: The dataset is highly imbalanced, with only about 0.17% of transactions being fraudulent. This imbalance is a central challenge in fraud detection.

4. Analysis Rubric & Methodology:This analysis adheres to the following rubric points, ensuring a comprehensive and systematic approach to data visualization and analysis:

Identifying and sourcing relevant datasets
Ensuring data integrity and consistency
Cleaning and handling missing values
Feature selection and engineering
Handling outliers and data transformations
Summary statistics and insights
Identifying patterns, trends, and anomalies
Initial visual representation of key findings

5. Key Findings & Visualizations:Through detailed exploratory data analysis and visualization, several critical insights were uncovered:

Class Imbalance: The dataset exhibits extreme class imbalance, a fundamental challenge for fraud detection models

Transaction Amount Patterns: Fraudulent transactions, on average, tend to involve smaller amounts compared to legitimate transactions, possibly an evasion tactic by fraudsters. The Amount feature was robustly scaled to mitigate the impact of its skewed distribution and outliers.

Time-Based Anomalies: While legitimate transactions show clear daily peaks correlating with business hours, fraudulent activities are more dispersed throughout the 24-hour cycle, hinting at operations outside conventional times.

Discriminative V-Features: Several anonymized V-features (e.g., V17, V14, V12, V10 exhibiting negative correlations; V4, V11 showing positive correlations) display distinct distributions between fraudulent and non-fraudulent classes, confirming their strong predictive power.

Feature Correlations: A comprehensive correlation matrix further highlighted the strong linear relationships between certain 'V' features and the 'Class' variable.

6. Technologies Used:Python 3.x
Jupyter Notebook / Google Colab
pandas (for data manipulation and analysis)
numpy (for numerical operations)
matplotlib (for static visualizations)
seaborn (for enhanced statistical data visualization)
scikit-learn (for data preprocessing: StandardScaler, RobustScaler)
