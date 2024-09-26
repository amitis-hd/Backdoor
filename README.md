## Overview
This repository contains a machine learning workflow to train an XGBoost model for thyroid disease classification using a dataset (Thyroid_Diff.csv). The code includes data preprocessing, model training, evaluation, and a backdoor attack experiment to assess the vulnerability of the model. It also includes various visualizations of feature importance and the distribution of the data.

## Features:
- Data preprocessing and feature encoding.
- XGBoost model training with parameter tuning.
- Cross-validation and accuracy scoring.
- Backdoor attack to test the robustness of the model.
- Visualization of feature importance, age vs. prediction, and a histogram with a bell curve.
- Confidence score analysis and synthetic data generation.
- Model export and tree visualization.

## Requirements
The project uses the following libraries. You can install them using pip:
```bash
pip install pandas numpy matplotlib scipy graphviz xgboost scikit-learn catboost lightgbm torch tqdm seaborn twine
```

## Additional Requirements:
- cython==0.29.23
- configargparse==1.5.2
- xlrd==2.0.1
- openpyxl==3.0.7
- mat73==0.50

## Results
The clean XGBoost model achieves an accuracy of 97.40% on the test dataset.
The backdoor attack model also performs similarly, but with a high backdoor success rate, indicating a vulnerability to the attack.
