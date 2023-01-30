# AutoPricePrediction-ML-Project
## Used Automobile Price Prediction

### Problem Statement
The problem at hand is to predict the price of a used car based on various features such as year of manufacture, km driven, fuel type, etc.

### Dataset
The dataset used is a collection of used car prices and their corresponding features.

### Data Type
The data includes 10 features and 1 target column (price). 
The features include

* year of manufacture
* km driven
* fuel type
* seller type
* transmission
* owner count
* seats
* torque
* engine
* mileage

### Algorithms Used
In this project, the following algorithms were used:

* Linear Regression
* Random Forest Regression
* XGBoost
* Lasso Regression

### Training Model
The algorithms were trained on the dataset using a train-test split, with 80% of the data used for training and 20% for testing. 
The best model was selected based on performance metrics such as root mean squared error (RMSE) and R-squared score.
**Hyperparameter** tuning was also performed using RandomizedSearchCV to get the best hyperparameters for the Random Forest Regression model.

### Outputs
The results of the models are shown below:

#### Linear Regression
*RMSE: 85277.05160166239*
*R2 score: 0.8546298500803426*

#### Random Forest Regression (after hyperparameter tuning)
*Best hyperparameters: {'n_estimators': 500, 'min_samples_split': 2, 'min_samples_leaf': 1, 'max_features': 'log2', 'max_depth': None}*
*RMSE: 77736.08259917068*
*R2 score: 0.8984801752097382*

### Conclusion
Based on the results, the Random Forest Regression model performed better than the Linear Regression model, 
with a lower RMSE and higher R-squared score. 
The model can be used to predict the prices of used cars based on their features, with a high degree of accuracy.
