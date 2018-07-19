# Housing Prices Prediction
Analysis of the housing prices from the Ames dataset

[Here's the Kaggle page](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) for this challenge.

----------

### My Approach:

**1. Data Exploration -**
    Here, I separate out the features as belonging to one of the 3 classes -
    
    * `num_cont_columns` for numerical continuous features
    * `num_discrete_columns` for numerical discrete features
    * `categ_columns` for categorical features
       
   I do this because there are different steps of preprocessing required for each of those features. By separating them, I am able to create a clean analysis of the data.

**2. Preprocessing -**
    After the separation, I divide the preprocessing stage into 3 steps where I analyse-
    
     * Continuous valued numeric features
     * Discrete valued numeric features
     * And finally, the Categorical features
        
   In each of those steps, I do the missing values imputation and feature engineering as required.

**3. Modelling -**

   I will train the following regression models -
    * Simple regression
    * Ridge regression
    * ElasticNet regression
    * Lasso regression
    
   And the following ensemble models - 
    * Random Forest
    * XGBoost
    
   Finally, I took the top 3 best performing models and stacked them up for the final submission model.
    
   ### Results:
    
   My final model scored an RMSE score of 0.12562 and is in the top 26% of the Kaggle leaderboard.
    
   I have included [my final predictions](https://github.com/nityeshaga/housing_prices_prediction/blob/master/submission.csv) 
   for the test data along with [the kernel that I used](https://github.com/nityeshaga/housing_prices_prediction/blob/master/analysis_housing_prices.ipynb)
   and the datasets with this repository.
