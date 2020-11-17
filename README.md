# ironhack-project-4
Statistical Analysis

# Step-by-step process
Import and clean data
- Remove columns with high amount of null values
- Look into columns with low variance		
- Look into columns with very few unique values

Data statistical analysis
- Use Seaborn pairplot to look at visual representations of overall dataframe correlation
- Calculate overall dataframe correlation (numerical variables)
- Sort numerical independent variables in terms of correlation with SalePrice
- Perform simple OLS linear regression on top 6 numerical independent variables
- Plot data with linear regression line

Which categorical factors are most likely to affect the sale price?
- MSSubClass (16 cats)
- MSZoning (8 cats)
- Neighborhood (25 cats)
- BldgType (5 cats)
- HouseStyle (8 cats)
- SaleType (10 cats)
- SaleCondition (6 cats)

Perform multiple OLS linear regression on Neighborhoods

Which variables are measured by square feet…..
- LotArea
- TotalBsmtSF
- 1stFlrSF
- 2ndFlrSF
- GrLivArea
- GarageArea
- WoodDeckSF
- OpenPorchSF
- CombinedIntPorch

Perform multiple OLS linear regression on these variables

# Results

- The one single variable that had the biggest affect on 'SalePrice' was 'OverallQual' (R-squared value of 0.6275)
- The neighbourhood modeal had an accuracy of 53.80%
- The model using variables that measure square footage had an accuracy of 67.38%

Therefore, based on the analysis carried out up to this point, the best model to select would be the one that uses variables measuring square foot as it has the highest accuracy score.

# Future improvements
- Remove outliers prior to analysis
- Look at number/type of rooms above basement
- Look at year/month of sale (Time Series)
