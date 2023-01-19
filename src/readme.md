Data Processing ====> data_exploratory_analysis.ipynb
*****************************************************
-> Importing necessary libraries
-> Loading the original data
-> Basic checks
-> Exploratory Data Analysis
	-> Univariate Analysis
	-> Bivariate Analysis of Continuous Variables vs Performance Rating
	-> Bivariate Analysis of Categorical Variables vs Performance Rating
	-> Multivariate Analysis
-> Department-wise performances Analysis

Data Processing ====> data_processing.ipynb
*******************************************
-> Importing necessary libraries
-> Loading the original data
-> Check the total number of distinct values
-> Check for duplicates
-> Check for missing values
-> Check for corrupted values
-> Outliers Detection
-> Feature Engineering
	-> Feature Selection
     	-> Dropping unwanted features
     	-> Independent and Dependent variable creation
     	-> Train and Test split
-> Export Train Data and Test Data

models ====> train_model.ipynb
******************************
-> Importing necessary libraries
-> Loading Training data and Testing data
-> Independent and Dependent variable creation
-> Feature Transformation using ColumnTransformer
-> Creating multiple models with default parameters with smote and without smote to see which model is performing well with the dataset
-> Model Creation
	-> Hypertuning Logistic Regression parameters using GridsearchCV
	-> Hypertuning Support Vector Classifier parameters using GridsearchCV
	-> Hypertuning KNeighborsClassifier parameters using RandomizedSearchCV
	-> Hypertuning Decision Tree Classifier parameters using RandomizedSearchCV
	-> Hypertuning Random Forest Classifier parameters using RandomizedSearchCV
	-> Hypertuning AdaBoost Classifier parameters using RandomizedSearchCV
	-> Hypertuning Gradient Boosting Classifier parameters using RandomizedSearchCV
	-> Model creation using Stacking Classifier (LogisticRegression + SVC + RandomForestClassifier)
-> Exporting Trained Models

models ====> predict_model.ipynb
********************************
-> Importing necessary libraries
-> Loading the Test data
-> Independent and Dependent variable creation
-> Importing trained models and predicting results
-> Exporting the results
-> User-defined Performance Ratings Prediction

visualization ====> visualize.ipynb
***********************************
Exploratory and Results visualizations : 
-> Importing necessary libraries
-> Loading the train and test data with predicted results from processed directory
-> Model Evaluation
	-> Performance Metrics Report
	-> Comparing the performance metrics of all models
	-> Finding out the best geralized model using Train accuracy and Test accuracy
-> Displaying the result of the best generalized model
-> Permutation importance for feature evaluation
-> Exporting the finalized model