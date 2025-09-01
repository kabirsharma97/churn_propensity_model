## Churn Propensity Model (OTT Platform)

## An end-to-end pipeline to predict customer churn for an OTT subscription platform.
## This project covers data preprocessing, feature engineering, ML modeling, evaluation, and deployment — built with BigQuery, PySpark, and Vertex AI.

## Project Overview
## The Churn Propensity Model predicts the likelihood of a customer unsubscribing in the next 30 days.
## Helps business teams design targeted retention strategies.
## Enables proactive interventions via personalized marketing & offers.

## Pipeline Workflow
## Data Ingestion & Preprocessing

## Sources: Customer Portfolio, Clickstream, Viewership, Marketing tables
## Handled missing values, outliers, scaling & encoding (dynamic BigQuery SQL + PySpark)
## Feature Engineering
## Segmented features: first week, penultimate week, last week
## Marketing email engagement, search frequency, device usage, billing patterns

## Modeling
## Baseline: Decision Tree, Random Forest, XGBoost
## Hyperparameter tuning: Grid, Random, Bayesian Search
## Target Encoding + Class imbalance handling (17.7% churners)

## Evaluation

## Metrics: ROC-AUC, PR-AUC, Precision@K, Recall@K, Decile Lift
## Temporal validation (train past → test future snapshots)

## Deployment
## Vertex AI Pipelines + GCP Monitoring
## Automated BigQuery feature pipeline with parameterized SQL
## Slack-based incident alerts for query runtime & resource usage

## Tech Stack
## Languages: Python, SQL, PySpark
## Cloud & Tools: Google BigQuery, Vertex AI, GCP Monitoring
## Libraries: XGBoost, Scikit-learn, SHAP, Pandas, NumPy
