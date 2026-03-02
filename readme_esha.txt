README
Project Overview

This project presents a large-scale distributed machine learning analysis of traffic fatality data using the Fatality Analysis Reporting System (FARS) dataset provided by the National Highway Traffic Safety Administration. The study addresses a real-world big data classification problem focused on predicting fatal crash outcomes and identifying high-risk factors influencing crash severity. The dataset exceeds 1GB in size and contains multi-level structured records including accident-level, vehicle-level, and person-level attributes such as crash time, environmental conditions, vehicle type, and driver demographics. Due to its volume and complexity, scalable distributed processing techniques were required for efficient analysis.

The main objective of this project was to design and implement a scalable machine learning framework capable of processing large transportation safety datasets, comparing multiple algorithms, and generating actionable insights for policy and decision-making. Four classification algorithms were implemented: Logistic Regression, Decision Tree, Random Forest, and Gradient-Boosted Trees. Logistic Regression served as a baseline model, while ensemble-based methods were applied to improve predictive accuracy and model robustness. Experimental findings demonstrated that ensemble models achieved superior performance across multiple evaluation metrics.

Technical Implementation

The complete workflow was implemented in Google Colab using Python and PySpark MLlib for distributed computation. The pipeline includes data ingestion, schema validation, preprocessing, feature engineering, categorical encoding, stratified data splitting, distributed model training, and evaluation. Derived features such as time-based crash categories and aggregated risk indicators were engineered to enhance predictive capability.

Performance was evaluated using Accuracy, Precision, Recall, F1-score, and AUC. Cross-validation with parallel execution was applied to ensure model stability and reduce overfitting. Scalability experiments were conducted to assess strong and weak scaling performance, and optimization strategies such as caching, partition tuning, and shuffle management were incorporated to improve computational efficiency.

Visualization and Dashboards

Four interactive Tableau dashboards were developed to support analytical interpretation and decision-making:

Data Quality and Pipeline Monitoring

Model Performance and Feature Importance

Transportation Safety Insights and Risk Patterns

Scalability and Computational Efficiency Analysis

These dashboards provide interactive visual exploration of crash trends, predictive results, and system performance, demonstrating a complete end-to-end big data analytics framework integrating distributed machine learning and business intelligence.