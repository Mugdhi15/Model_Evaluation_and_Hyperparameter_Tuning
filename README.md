# Model_Evaluation_and_Hyperparameter_Tuning
This experiment aimed to identify the best-performing machine learning model for predicting survival on the Titanic dataset. The workflow included data preprocessing, baseline model training, hyperparameter tuning, evaluation, and visualization.

The dataset was cleaned and preprocessed by removing irrelevant columns and handling missing values. Categorical features such as sex and embarked were label-encoded, and the data was standardized using StandardScaler.

Four baseline classification models were trained and evaluated:
- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

Each model was assessed using accuracy, precision, recall, and F1-score. Random Forest and SVM emerged as the top performers and were selected for further tuning.

To optimize these models:
- Random Forest was tuned using GridSearchCV over a defined parameter grid for n_estimators, max_depth, and min_samples_split.
- SVM was tuned using RandomizedSearchCV across C, kernel, and gamma values.
- Post-tuning, the models were evaluated again using F1-score on cross-validation, confusion matrices, and ROC curves. A final comparison table and bar chart highlighted that Tuned SVM outperformed the other models across key metrics.

This systematic experimentation provided insights into model behavior and showed the effectiveness of hyperparameter tuning in improving predictive performance.
