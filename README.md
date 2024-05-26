# Home-Credit--CreditRisk-Model-Stabilit

**Introduction**

The motivation behind this project is to expand access to financial services for individuals with limited or no credit history. Traditional methods often exclude these individuals from the formal banking sector. By leveraging machine learning, we can analyze diverse client characteristics to make more informed lending decisions, promoting financial inclusion and empowerment.

**Dataset and Features**

The dataset includes a comprehensive collection of financial and personal data used to predict client default risk. It comprises multiple files categorized by data source and detail level. Features include financial metrics like credit amount, days past due, income types, and loan statuses, as well as personal attributes like employment details, marital status, and residence information.

**Data Preparation**

We employed several approaches to manage and preprocess the data:

Data Type Management and Handling Missing Data

Feature Engineering and Aggregation

Dimensionality Reduction and Data Cleaning

Memory Optimization and Efficient Data Handling

**Methodology**

Approach 1

Gradient Boosting Models: Utilized LightGBM, XGBoost, and CatBoost for binary classification.

Model Configuration: Employed GPU acceleration and early stopping.

Ensemble Prediction: Combined predictions using weighted averages.

Approach 2

Stratified and Group-wise Cross-validation: Used LightGBM with hyperparameters to optimize AUC.


Model Validation and Predictive Model Assembly: Employed a voting mechanism for model outputs.

Approach 3

AutoML with AutoGluon: Focused on ROC AUC as the evaluation metric.

Data Preparation and Cross-validation: Ensured group integrity and optimized feature engineering.

Approach 4

Model Tuning and Validation: Used LightGBM with a focus on AUC.

Stability Analysis and Predictive Aggregation: Evaluated predictions using a custom Gini coefficient metric.

Approach 5

Weighted Ensemble Method: Combined predictions from multiple models using a complex weighting scheme.

Temporal Adjustment: Adjusted predictions based on the distribution of weeks in the test set.

**Results**

The performance of each approach was measured using AUC scores:

Ensemble of CatBoost, XGBoost, and LightGBM: 0.392

Tuned LGBM models: 0.565

Model with Gini stability metrics: 0.503

AutoGluon models: 0.567

Ensemble of all models: 0.576

**Conclusion**

**The project demonstrated the effective use of advanced machine learning techniques to assess consumer finance default risks. The ensemble method proved particularly beneficial, leveraging the strengths of each model to enhance prediction accuracy. Future work could explore more sophisticated ensemble techniques, expand the feature set, and incorporate feedback loops to refine the models continually.
**
