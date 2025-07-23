# Regression Modeling on Suicide Rates Dataset
In this assignment, I developed multiple linear regression models to predict the suicide rate per 100k population using the pre-processed Suicide Rates Overview dataset.

First, I built a regression model using one-hot encoded categorical variables (sex, age group, generation) and determined the number of regression coefficients it contained. Using this model, I predicted the suicide rate for a 20-year-old male from Generation X and calculated the mean absolute error (MAE) for that prediction.

Next, I created a new regression model by transforming the original nominal variables into numerical features, reducing dimensionality and re-examining the number of coefficients. I used this model for the same prediction scenario and compared its MAE to the previous model.

I also used this numerical-feature model to predict the suicide rate for a 33-year-old male from the Alpha generation.

Throughout the assignment, I discussed the advantages of regression over classification for modeling continuous target variables, and the benefits of using numerical features instead of one-hot encoding in regression contexts.

Finally, I provided a recommendation on whether to use classification or regression for predicting suicide rates, considering the nature of the problem and the data.

