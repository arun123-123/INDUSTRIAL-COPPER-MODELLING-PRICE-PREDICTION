# INDUSTRIAL-COPPER-MODELLING-PRICE-PREDICTION

KEY TECHNOLOGIES AND SKILLS

  1. Python
  2. Numpy
  3. Pandas
  4. Matplotlin
  5. Seaborn
  6. Scikit-Learn
  7. Streamlit

EXPLANATION

 1. Import Necessary libraries for data manipulation, model training and evaluation.
 2. Loads the copper price dataset into a Pandas DataFrame
 3. Selects the Date feature as an independent variable and Price as the dependent variable
 4. Convert the  "Date" feature into a numerical representation suitable for the model time series features like year, month, day.
 5. The Dataset may contain missing values that need to be addressed. Th Choice of handling these null values, whether through mean, median or mode imputation, depends on the nature of the data and the specific feature.
 6. To prepare categorical feature for modelling, we employ ordinal encoding. This technique transforms categorical values into numerical representations based on their intrinsic nature and their relationship with the target variable. Additionally, it's essential to convert data types to ensure they match the requirements of our modelling process.
 7. Outliers can significantly impact model performance. We tackle outliers in our data ny using the Interquartile Range(IQR) method.  This method involves identifying data points that fall outside the IQR boundaries and then converting them to values that are more in line with the rest of the data.  This step aids in producing a more rebust and accurate model.

EXPLORATORY DATA ANALYSIS(EDA):  

  1. Skewness Visualization: To enchance data distribution uniformity, we visualize and correct skewness in continous variables using Seaborn distplot. By applying the Log Transformation method, we achoeve improved balance and normal distribution, while ensuring data integrity.
  2. Our focus is on improving our dataset for more effective modelling. We achieve this by creating new features to gain deeper insights from the data while making the dataset more efficient.  Notably, our evaluation, facilitated by Seaborn's Heatmap, confirms that no columns, with the highest correlation values.

CLASSIFICATION:

 1. WON AND LOST CLASSIFICATION:  In our predictive journey, we utilize the "status" variable definiing "WON" and "LOST".  Data points with status values other than "WON" and "LOST" are excluded from our dataset to focus on the core classification task. Making the predictions on the testing set using the trained model
 2. Hyperparameter tuning with GridSearchCV and Cross-Validation: To fine-tune ourmodel and mitigate overfitting, we employ GridSearchCV with cross-validation for hyperparameter tuning.  This function allows us to systematically explore multiple parameter values and return optimal set of parameters.
 3. Calculates the Mean Squared Error(MSE) R2_score to access the model's performance
    
