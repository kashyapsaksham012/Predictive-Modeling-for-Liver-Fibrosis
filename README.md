# Predictive-Modeling-for-Liver-Fibrosis
This Python script implements a comprehensive pipeline for predicting liver fibrosis severity. It begins by installing necessary packages for machine learning, dimensionality reduction, interpretability, and handling imbalanced data. The script then defines functions for:

Package Availability Check: Verifying the availability of optional libraries like UMAP, XGBoost, LightGBM, CatBoost, SHAP, LIME, and imbalanced-learn.
Enhanced File Upload and Validation: Handling dataset upload (with Colab support and local file fallback) and performing basic validation checks on the input CSV file.
Medical Domain Feature Creation: Generating new features based on medical domain knowledge, such as ratios and composite scores derived from liver function tests.
Multiple Model Training: Training various regression models (XGBoost, LightGBM, CatBoost, Random Forest, Linear Regression, and an Ensemble) on the processed data.
Interpretability Analysis: Utilizing SHAP and LIME (if available) to analyze feature importance and provide local explanations for model predictions.
Fairness and Subgroup Analysis: Evaluating model performance across different demographic groups (gender and age) to assess fairness.
Saving Results: Serializing trained models, performance metrics, and analysis results for later use.
The main execution block orchestrates these steps, handling data loading, preprocessing (including handling duplicates, feature engineering, scaling, and SMOTE for imbalanced data), data splitting, severity score creation using dimensionality reduction (UMAP/PCA), model training, evaluation, interpretability, and fairness analysis. Finally, it saves the results and provides a summary of the analysis.
