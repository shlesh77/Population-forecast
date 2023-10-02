# Population-forecast
Population forecast 
**STEPS:**
1. Set up global knitr chunk to control code display options
2. Load the necessary packages to perform the modeling
3. Import the original data as 'popdata'
4. Check the data type of each variable
5. Change the data structure of year and washoe from character to numeric
6. Using the Keyfitz three parameter population model
        Population = a/{1+b*exp^(-ct)} 
7. Fit the nonlinear regression model using nls2() and predict **model 1**
8. Plot the model 1 and extend to 2100
9. Create model 2 by using the first iteration and calibrating the logistic curve to the present day population
10. Based on the results of Model 1, model parameters (b and c) are adjusted to improve the fit of Model 2. An iterative process is used to find the optimal population ceiling 
11. With new values of adjusted a, predict the model 2. Compare it with how it changes from original model
12. Run a short-run linear model (**Model 3**) for the five years from current population data available to estimate the logistic  curve
13. Re-calibrate the new population ceiling to 2027 and make prediction
14. Smoothen the curve by moving average smoothing technique
15. Plot the final projection
16 Export the final table to csv
