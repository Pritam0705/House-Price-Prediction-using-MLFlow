## House Price Prediction
This project utilizes machine learning to predict house prices using the California housing dataset. The workflow integrates MLflow to streamline experiment tracking, model versioning, and reproducibility. Key models and metrics are logged in MLflow to compare their performance effectively and select the best-performing model.  

### Features
- **Data Exploration and Visualization:** Detailed EDA with correlation analysis and visualization to identify key factors influencing house prices.
- **MLflow Integration:** Tracks experiments, hyperparameters, and performance metrics for reproducible workflows.
- **Model Development and Evaluation:** Implements models like Random Forest and evaluates them with metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R^2
- **Model Tuning:** Hyperparameter optimization using GridSearchCV for improved model performance.

### Dataset
1. Source: California Housing Dataset (from sklearn.datasets).

2. Structure:
- Features: Housing-related attributes (e.g., median income, number of bedrooms).
- Target: Median house price.

3. Preprocessing:
- Checked for missing values.
- Analyzed distributions and correlations among features.

Workflow
1. Data Exploration
- Performed descriptive statistics and correlation analysis to identify trends.
- Visualized distributions and outliers using seaborn and matplotlib.

2. Model Development
- Implemented a Random Forest Regressor as the primary predictive model.
- Logged the model and its parameters to MLflow for comparison and tracking.

3. Hyperparameter Tuning
- Optimized hyperparameters using GridSearchCV to improve prediction accuracy.
- Logged the best parameters and associated metrics in MLflow.

4. Model Evaluation   
Metrics used for evaluation:
- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- 𝑅^2 (Coefficient of Determination)

5. MLflow Integration  
Set up MLflow to track:
- Experiment parameters (e.g., number of estimators, max depth).
- Metrics for model performance.
- Serialized models for deployment.
