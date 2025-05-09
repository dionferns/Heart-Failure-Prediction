# Heart Failure Prediction

This project builds and evaluates machine-learning models to predict heart failure from clinical and exercise test data.

## Overview

1. Load the `heart_failure.csv` dataset.
2. Explore data: summary statistics, missing-value report, class balance.
3. Preprocess features:
   • Impute missing values (mode, median, conditional)
   • Encode categorical fields (one-hot for nominal, ordinal for ordered)
   • Scale numeric columns with StandardScaler
4. Engineer and select features:
   • Create flags for missingness
   • Correlation analysis and univariate plots
5. Train and tune models via grid search with cross-validation:
   • Logistic Regression
   • Random Forest
   • CatBoost Classifier
6. Evaluate results:
   • Accuracy, precision, recall, F1 score
   • ROC curves and AUC
   • Confusion matrices
   • Feature importance rankings

## Files and folders

• Heart\_Failure.ipynb    — Jupyter notebook with full workflow
• data/heart\_failure.csv — Raw dataset
• requirements.txt       — List of Python package dependencies

## Setup and use

1. Clone or unpack this folder.
2. Create and activate a Python 3 virtual environment if desired.
3. Install dependencies:
   pip install -r requirements.txt
4. Open and run the notebook:
   jupyter lab Heart\_Failure.ipynb
   or
   jupyter notebook Heart\_Failure.ipynb

## Results

• Final CatBoost model achieves around 91 % accuracy.
• Detailed evaluation metrics (ROC AUC, confusion matrices) appear in the final sections of the notebook.

## Next steps

• Additional feature engineering (interaction terms, polynomials)
• Ensemble or stacking of multiple classifiers
• Deployment as a simple web API or dashboard

## License

Released under the MIT License. Feel free to use, modify, or distribute.
