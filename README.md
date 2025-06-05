# Server Performance Anomaly Detection

This project explores anomaly detection techniques applied to server performance metrics. Using a synthetic dataset that simulates real-world server conditions, the goal was to build a robust model that could identify potential system incidents or abnormal behavior across various metrics such as CPU usage, memory, disk I/O, and network traffic.

## Objective

Develop and evaluate a classification model that can accurately detect anomalies in server performance data, enabling early identification of potential failures or performance degradation.

## Methodology

- **Synthetic Data Generation**: Simulated metrics over a fixed time window to include both normal and anomalous patterns.
- **Exploratory Data Analysis (EDA)**: Identified key distributions, correlations, and temporal behaviors in the dataset.
- **Feature Engineering**: Created lag features, moving averages, and statistical derivatives to improve model interpretability and performance.
- **Modeling**: Used a Random Forest classifier due to its robustness with imbalanced data and ability to capture complex feature interactions.
- **Hyperparameter Tuning**: Employed grid search with cross-validation to optimize model parameters.

## Evaluation

The model achieved high accuracy across multiple threshold settings. Evaluation was conducted using classification metrics (precision, recall, F1-score) and confusion matrices. At thresholds of 70%, 90%, and 40%, the classifier maintained strong performance, demonstrating both sensitivity and specificity.

## Technologies

- Python, Pandas, NumPy, Matplotlib
- scikit-learn (Random Forest, GridSearchCV)
- Data visualization and performance evaluation tools
