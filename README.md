## Quality of Wine
Estimated a linear regression and used model selection to filter out which variables best explain the quality of wine.

## How It's Made
* Packages
  - Boruta
  - AER
  - lmvar
  - MASS
## Key Features
* Descriptive Statistics
  - Boxplots
  - Histograms
* Boruta Algorithm
* Mallows CP
* AIC/BIC
* Heteroskedasticity
  - Breusch Pagan Test
  - Residuals plotted
  - White Test
*Training/Testing Split
  - RMSE
* 5 Fold Cross Validation

Observed data through boxplots and histograms which eliminated outliers from the model to increase R^2.
Applied the Boruta algorithm to identify the most significant variable (alcohol) and eliminate insignificant variables.
Then, used the Mallows CP Test to continue to filter out the best predictors for the model. 
Detected heteroskedasticity from the residuals plotted and confirmed through the BP test.
Performed the White test to fix heteroskedasticity and reduce standard errors. This also made all variables significant.
Visually, the residuals and y hat plot suggested a log-linear model would better fit the model. Tested this through AIC and BIC and the log linear was the best model.
Split data into testing and training to then calculate the RMSE.
Applied a 5 fold cross validation to obtain RMSE. Both testing RMSE, training RMSE, and 5 fold cross validation RMSE were small, meaning there is only a small amount of error in the model.
Small RMSE = the predicted value is only a small amount off from the actual value.
