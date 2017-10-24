## Part 1
* Is there any missing (NaN)? If so, how would you remove it?
 * No, in the above table you can see that the count of missing entries for each column is zero.
 * If there were any columns with missing values you could drop them from the dataframe by calling df.dropna(axis=1, how='any')
* What columns appear to offer the best hope of a linear approximation of price?
 * bathrooms, sqft_living, grade, sqft_above, and sqft_living15
* Which columns data are categorical? Which are numerical?
 * The categorical columns would be floors, waterfront, view, condition, zipcode, grade
 * The remaining columns would be numeric.
* Which is the best column for prediction? 
 * sqft_living seems to be the best column for predicting house price. Looking at the graph of house price and sqft_living, there seems to be a strong linear relationship between the two values, generally showing that lower housing prices and lower sqft_living values go together and higher living prices going together with higher sqft_living. There are other columns that seem to follow this pattern as well, but this one seems to have the points most closely bunched around the line through the points.
 
 ## Part 2
* How might you choose which column is best for the predictive model?
* Can you compare the quality of the different columns as predictors before you train a model? How?
* How many rows are in the training data? How many rows in the test data?
* What do the metric scores tell you about the model?