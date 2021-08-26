### Real Estate Price Prediction

Housing prices in Bangalore are predicted using *linear regression* algorithm with 84% accuracy. The price varies with location, number of bedrooms, square foot area etc.The dataset, taken from Kaggle is cleaned to remove inaccurate and erroneous data. The model is trained using linear regression module in *scikit-learn* library in *python*. *Jupyter notebook* and *matplotlib* library is used for organization and visualization of data. The model is split using the *train_test_split* method and *K fold cross validation* is used to measure the accuracy of the model. Using *Grid Search CV* the best model and corresponding parameters were found. Source code link

## Steps or Approach
- **Loading** : Load the dataset from Kaggle into a dataframe in Jupyter notebook
- **Data Cleaning** : Handling the NA values and other erroneus data
- **Feature Engineering** : Added new feature for bhk, price per square feet
- **Dimensionality Reduction** : All locations having lower than 10 data points are tagged as "other"
- **Outlier Removal Using Business Logic** : Removal of outliers by keeping our minimum threshold per bhk to be 300 sqft
- **Outlier Removal Using Standard Deviation and Mean**
- **Model Building** : Training the model after splitting the data into training and test dataset
- **Measure the accuracy of the model** : Use K Fold cross validation to measure accuracy of our LinearRegression model
- **Find best model using GridSearchCV** : Finding the model with highest accuracy using GridSearchCV
- **Test the model**
- **Export the tested model to a pickle file** : Export the model into a pickle file to make predictions on housing prices in Bangalore.

## Tools used
- Python
- Jupyter notebook
- Scikit learn(Linear_model, GridSearch CV, K fold cross validation, train_test_split)
- Matplotlib




