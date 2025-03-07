# Project Scope: Predictive Safety Risk Classifier

## Overview
This project develops a machine learning prototype to predict high-risk safety zones based on historical crime data, aligning with the TruLight Project’s focus on data-driven safety. The workflow will be built in Jupyter Notebooks, version-controlled with Git, and showcased as a production-ready pipeline on GitHub.

## Goals
- **Primary**: Build an ML model to classify locations as "high-risk" or "low-risk" for safety incidents.
+  - **ML Problem**: Predict whether a Chicago location is high-risk for crime using spatial (latitude, longitude) and temporal (time of day, day of week) features, solved via binary classification.
- **Secondary**:
  - Demonstrate end-to-end ML skills: ETL, feature engineering, modeling, and pipeline development.
  - Visualize risk predictions for clear communication.
  - Create a scalable, reproducible pipeline for potential production use.

## Dataset
- **Source**: Chicago Crime Dataset (City of Chicago Data Portal)
- **Problem**: Binary classification (high-risk vs. low-risk zones)
- **Details**: Historical crime records with timestamps, locations (latitude/longitude), and crime types. Subset to a manageable size (e.g., 1 year or 10,000 rows) for prototyping.

## Analytical Steps
1. **ETL**: Load crime data, clean missing values, extract time-based features (e.g., hour, day).
2. **Feature Engineering**: Aggregate crime counts by location, define risk labels based on thresholds.
3. **ML Workflow**: Train and evaluate a classifier (e.g., random forest) on location and time features.
4. **Pipeline**: Use `scikit-learn` to build a preprocessing and prediction pipeline.
5. **Communication**: Generate a heatmap of risk zones and summarize findings in a notebook.

## Adjustments
- If model performance is weak, experiment with additional features (e.g., crime type) or models (e.g., XGBoost).
- Scale dataset size or scope as needed based on prototype results.