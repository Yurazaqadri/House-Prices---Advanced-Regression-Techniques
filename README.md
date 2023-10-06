# House-Prices---Advanced-Regression-Techniques
Predict sales prices and practice feature engineering, RFs, and gradient boosting
The provided code performs the following tasks to build and evaluate a regression model for predicting house prices using the given dataset:

Importing Libraries: The code begins by importing various Python libraries required for data manipulation, visualization, and modeling. These libraries include pandas, matplotlib, seaborn, numpy, scikit-learn, XGBoost, and joblib.

Loading Data: The code loads the training and test datasets, each containing a subset of columns specified in the selected_columns list. These columns are selected for building the predictive model.

Data Preprocessing:

It separates the target variable 'SalePrice' from the features in the training dataset.
The training and test datasets are combined to ensure consistent one-hot encoding of categorical variables.
Categorical columns are one-hot encoded using pd.get_dummies.
Missing values in both training and test datasets are imputed with the median value using SimpleImputer.
The training dataset is split into a training set and a validation set using train_test_split. This allows for model evaluation during training.
Model Training:

A Linear Regression model is created and trained using the training dataset (X_train and y_train).
The model's performance is evaluated on the validation set, and the Root Mean Squared Error (RMSE) is calculated and printed.
Generating Predictions:

The trained model is used to make predictions on the test dataset (X_test).
The predictions are stored in a DataFrame (test_predictions) along with the corresponding 'Id' from the test dataset.
Printing Predictions: Finally, the code prints the DataFrame containing the 'Id' and predicted 'SalePrice' for each record in the test dataset.

This code essentially performs the entire process of data preprocessing, model training, evaluation, and prediction generation for a Linear Regression model. The predictions are then saved to a CSV file for further analysis or submission, such as in a Kaggle competition.
