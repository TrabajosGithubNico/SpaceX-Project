This module focuses on building and optimizing supervised learning models to predict the success of SpaceX Falcon 9 first-stage landings. By leveraging historical data, we transition from exploratory analysis to predictive modeling, identifying the most reliable algorithm for forecasting mission outcomes.

Data Standardization: Applied StandardScaler to the feature set $X$ to normalize the data, ensuring that all features contribute equally to the model's performance. 

Predictive Modeling: Developed and trained four distinct classification algorithms: Logistic Regression, Support Vector Machine (SVM), Decision Tree, and K-Nearest Neighbors (KNN).

Hyperparameter Tuning: Utilized GridSearchCV with 10-fold cross-validation to systematically test various parameter combinations and prevent overfitting.

Model Evaluation: Measured performance using accuracy scores on test data (splitting the dataset into 80% training and 20% testing sets).

Error Analysis: Generated Confusion Matrices for each model to visualize the distribution of True Positives, True Negatives, and misclassifications (False Positives/Negatives).

Algorithm Comparison: Compared validation accuracies across all models—identifying that while most models achieved an 84.8% accuracy during tuning, the Decision Tree reached a peak of 87.6%.

Output
A finalized predictive pipeline capable of determining the probability of a successful Falcon 9 landing. This model serves as the project’s technical conclusion, providing a data-driven tool to estimate launch costs based on the likelihood of booster recovery.
