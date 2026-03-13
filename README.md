**Flipkart Customer Support Data Analysis (CSAT Prediction)**
This project focuses on analyzing customer support interactions for Flipkart to identify the key drivers of Customer Satisfaction (CSAT) scores. The project includes a comprehensive Exploratory Data Analysis (EDA) and the development of Machine Learning (ML) models to predict user satisfaction.

**Project Overview**
The primary goal is to understand what factors influence a customer's rating (on a scale of 1-5) and to build a predictive model that can estimate the CSAT score based on interaction details.

**Key Objectives:**
1. Operational Excellence: Identify specific ticket categories and channels that underperform.
2. Service Quality: Analyze the impact of agent experience (tenure) and response times on satisfaction.
3. Predictive Modeling: Develop a reliable model to predict CSAT scores for proactive service management.

**Dataset Description**
The dataset consists of 85,907 customer support interactions with the following key attributes:
  1. Channel: Inbound, Outbound, Email, etc.
  2. Issue Category: Returns, Refunds, Technical Glitches, etc.
  3. Agent Metrics: Name, Supervisor, Manager, Tenure Bucket, Agent Shift.
  4. Transactional Data: Item Price, Customer City, Product Category.
  5. Performance Metrics: Connected Handling Time, Response Time (Minutes).
  6. Target Variable: CSAT Score (1-5).

**Project Structure**
1. EDA.ipynb: contains the Exploratory Data Analysis, including 20 detailed visualizations, data cleaning, and business insights.
2. ML.ipynb: contains the Machine Learning pipeline, including feature engineering, hypothesis testing, model training (Logistic Regression, Random Forest, XGBoost), and evaluation.
3. Customer_support_data.csv: Source dataset (ignored by git).
4. best_model.pkl: Serialized best-performing model (ignored by git).

**Key Findings**
1. Resolution Time is Critical: There is a strong negative correlation between response time and CSAT score. Faster resolutions lead to significantly higher ratings.
2. Channel Performance: Real-time channels (like Inbound) generally yield higher satisfaction than asynchronous ones (like Email).
3. Experience Matters: Agents with higher tenure (>90 days) consistently maintain higher average CSAT scores compared to new hires.
4. Volume vs. Quality: High-volume urban centers (Metros) show distinct satisfaction patterns, requiring optimized regional logistics.

**How to Run**
1. Clone the repository.
2. Ensure you have the required dependencies installed (pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost).
3. Open EDA.ipynb to view the initial data analysis.
4. Open ML.ipynb to train and evaluate the predictive models.
