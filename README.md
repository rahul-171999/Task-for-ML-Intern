# Task-for-ML-Intern
Objective
This assignment assesses your ability to process hyperspectral imaging data, perform dimensionality reduction, and develop a machine learning model to predict mycotoxin levels (e.g., DON concentration) in corn samples.
Problem Statement
You are provided with a compact hyperspectral dataset containing spectral reflectance data from corn samples across multiple wavelength bands. Your task is to:
Preprocess the data (e.g., handle missing values, normalize features).
Visualize spectral bands to explore data characteristics.
Reduce dimensionality using PCA or t-SNE and interpret the results.
Train a machine learning model (e.g., simple neural network) for regression.
Evaluate the model and present actionable insights.
Data Preparation
Loading and Inspection: Data from 'TASK-ML-INTERN.csv' was loaded into a DataFrame, providing an initial view and statistical summary of the features and target variable, vomitoxin_ppb.
Feature Standardization: Non-relevant columns were dropped, and the remaining features were standardized to have zero mean and unit variance.
Data Visualization
Spectral Reflectance: A plot was created to visualize the average spectral reflectance across different wavelength bands, indicating how reflectance varies.
Dimensionality Reduction
PCA Implementation: PCA was applied to reduce the dataset to components that explain 95% of the variance, visualized through a plot showing cumulative explained variance.
3D Data Visualization
PCA Scatter Plot: The first three PCA components were used to generate a 3D scatter plot, visually encoding the target variable to examine data distribution and clustering.
Model Training and Evaluation
LSTM Network: An LSTM model was configured and trained to predict vomitoxin levels, with performance evaluated using MAE, RMSE, and R² metrics.
Performance Visualization: Training and validation losses were plotted over epochs to monitor model convergence.
Results
Model Accuracy: The LSTM model demonstrated a specific level of accuracy in predicting vomitoxin ppb, assessed by error metrics and explained variance through PCA.
Conclusion
The analysis effectively standardized and reduced the dimensionality of the data, facilitating an LSTM-based predictive modeling that yielded quantifiable predictions of vomitoxin concentrations. Further improvements might involve tuning model parameters or exploring alternative feature selection techniques.
