# UFC Match Predictor (Machine Learning Project)

This is a personal project, created as part of my AI studies, to predict the winner of UFC matches using machine learning.

## Project Goal
The goal was to build an end-to-end ML pipeline, from data cleaning and feature engineering to model training and evaluation, based on a real-world dataset.

## Key Technologies
* **Data Processing:** Pandas
* **ML Model:** XGBoost (XGBClassifier)
* **Evaluation:** Scikit-learn (Cross-Validation, Confusion Matrix, Log Loss)

## Workflow
1.  **Data Loading:** Loaded several CSV files, including historical fight and fighter stats.
2.  **Data Cleaning:** Handled missing values using `SimpleImputer` and dropped irrelevant columns (e.g., identifiers, data leakage sources).
3.  **Preprocessing:** Encoded the target variable 'winner' from 'Red'/'Blue' to 1/0.
4.  **Model Training:** Trained an `XGBClassifier` on the final feature set.
5.  **Evaluation:**
    * Achieved a **[plak hier je accuracy, bv: 88.8%]** accuracy on the test set.
    * Analyzed the `ConfusionMatrix` which showed a well-balanced model with no significant predictive bias, despite an imbalanced dataset.

## How to Run
1.  Ensure you have the required libraries (Pandas, XGBoost, Scikit-learn).
2.  Run the `main.ipynb` (or `UFC_Forecaster.ipynb`) notebook.
3.  The notebook uses the datasets located in the `/data` folder.