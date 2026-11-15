## Customer Renewal Data Preparation

## Project Overview

This project demonstrates the preparation of customer subscription data for a supervised machine-learning classification task using Python and pandas.

The objective is to transform raw customer and subscription-history records into a clean feature matrix (`X`) and target variable (`y`).

**This is a data-preparation project. No predictive model is trained or evaluated.**

## Technologies

- Python
- pandas
- NumPy
- Jupyter Notebook

## Project Workflow

1. Inspect customer and subscription-history datasets.
2. Identify and handle missing customer information.
3. Merge datasets using customer identifiers and validate the relationship.
4. Identify customers without known renewal outcomes.
5. Encode categorical features using one-hot encoding.
6. Convert renewal outcomes into binary classification labels.
7. Separate labeled observations into features (`X`) and target (`y`).
8. Validate the resulting data.

## Results

- 6 customer records in the merged dataset.
- 5 customers with known renewal outcomes.
- 1 customer excluded from the labeled dataset because the renewal outcome is unknown.
- 7 prepared input features.
- 3 positive renewal labels and 2 negative renewal labels.
- No missing values in the final feature matrix or target.

## Limitations

The dataset is synthetic and contains only five labeled observations. It is insufficient for meaningful model training, testing, or performance evaluation.

Missing ages were imputed during data preparation. In a future predictive-modeling workflow, imputation parameters should be learned from training data only to avoid leakage.

Additional real-world data would be required before developing and evaluating a reliable predictive model.

## Future Improvements

- Obtain a larger, representative dataset.
- Introduce a proper training and testing workflow.
- Fit preprocessing transformations using training data only.
- Train and evaluate a supervised classification model.

## Purpose

This project was developed as part of my preparation for further studies in supervised machine learning, with an emphasis on understanding data quality, feature preparation, and reproducible Python workflows.
