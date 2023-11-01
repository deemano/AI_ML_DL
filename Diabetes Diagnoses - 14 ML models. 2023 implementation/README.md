# Implementation of 14 different ML models

# CONTENT: 
0. System Setup - Set model to run on GPU (skip this to run on CPU)
1. Inception - Preparing the Working Environment
2. Importing the Dataset, Checks and Optimizations
3. Dataset Cleaning & Optimization

   Features Scaling:
   - Normalize 'BMI' feature with Min_Max
   - Normalize 'BMI' feature with Z-score
   - Normalize 'BMI' feature with Power Transformer - Yeo-Johnson transformation

4. Exploratory Data Analysis (EDA):<br>
   4.1. Target Variable Distribution & Visualization<br>
   4.2. Visualize Numerical Features Distribution<br>
   4.3. Correlation Matrix<br>
   4.4. Pair Pilot Visualization<br>
   4.5. Visualize features across classes - Box-plots<br>
   4.6. Categorical Features - Count-plots <br>

6. Data Partitioning
7. Features Selection Methods<br>
   6.1. Feature Importance with Random Forest<br>
       6.1.1. Testing Random Forest with GridSearchCV - determine best ML model hyperparameters<br>
   6.2. Dropping irrelevant columns

8. Hierarchical classification (2 stages)
   - Building the Model structure

   Stage 1 Classification Models (various tried)
   7.1. Random Forest Classifier
       Additional Operations:
       - Filter Data for Second Stage Classification modeling
       - Prepare Data for Second Stage

   7.2. Logistic Regression
   7.3. Support Vector Machines (SVM)
   7.4. K-Nearest Neighbors
   7.5. Stochastic Gradient Descent (SGD)
   7.6. Naive Bayes
   7.7. Decision Trees
   7.8. Gradient Boosted Trees
       - Evaluate the Best model from Stage 1 (Gradient Boost Trees)
       - Models Accuracy Metrics: Accuracy, Precision, Recall, F1-Score, AUC-ROC
   7.9. Neural Network
   7.10. XGBoost
   7.11. LightGBM
   7.12. CatBoost
   7.13. Anomaly Detection Models: Isolation Forest
   7.14. Transformers

   Stage 2
   - Determine important features between Pre-Diabetes & Diabetes classes
   - Building Testing Models for Stage 2 Binary Classification
   7.2.1. Random Forest Classifier
   7.2.2. Logistic Regression
   7.2.3. Gradient Boost Trees
   7.3. Evaluate the Best model from Stage 2 (Gradient Boost Trees)

## NOTES: 
The dataset is provided by the CDC - Centers For Disease Control And Prevention
Link: https://www.kaggle.com/datasets/cdc/behavioral-risk-factor-surveillance-system
