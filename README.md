# MechaCar_Statistical_Analysis
 
## Linear Regression to Predict MPG
![Linear_Regression](/analysis/Linear_Regression.PNG)
![Linear_Regression_summary](/analysis/Linear_Regression_summary.PNG)

Looking at the output of the linear regression it has been determined from the Pr(>|t|) values that the ground_clearance and vehicle_length values are likely to provide a non-random amount of variance to the mpg values. The resulting overall p-value of this multiple linear regression is below the 0.05 significance therefore the null hypotheses for the linear regression can be rejected and the slope of the linear model is therefore not 0 while the r-squared value is 0.7 which means roughly 70% of our mpg predictions can be explained using the multiple linear regression model.

## Summary Statistics on Suspension Coils
![total_summary](/analysis/total_summary.PNG)
![lot_summary](/analysis/lot_summary.PNG)

According to the summary of all the PSI data in the dataset the variance for the suspension coils is 62 which does not exceed the design specifications but when the variance is calculated per manufacturing lot it has been determined the suspension coils produced by manufacturing lot 3 exceed the 100 pound per square inch design specification with a variance of 170 while the variance for manufacturing lot 1 and 2 are within the design specification with variance values of 1 and 7 respectively.

## T-Tests on Suspension Coils
![t_test_all](/analysis/t_test_all.PNG)

The one-sample t-Test for all manufacturing lots within the provided dataset returned a p-value of 0.06 which is above the 0.05 significance level indicating the dataset provided is statistically similar to the population.

![t_test_lot1](/analysis/t_test_lot1.PNG)
![t_test_lot2](/analysis/t_test_lot2.PNG)
![t_test_lot3](/analysis/t_test_lot3.PNG)

The one-sample t-Test for each manufacturing lot returned p-values for Lot1, Lot2 and Lo3 of 1, 0.6 and 0.04 respectively indicating manufacturing lot1 and lot2 are statistically similar to the population but the p-value for lot 3 is below the 0.05 significance level indicating the mean of the PSI reading for lot3 is statistically different from the population.

## Study Design: MechaCar vs Competition
In order to quantify how the MechaCar performs against other brands in the market the following statistical study can be used.

The study will use the following metrics to compare to competitors
 - acceleration time (0 to 60mph)
 - MSRP
 
The study will look to proof/disprove the following hypotheses
 - Null hypothesis: the mean amount of time it takes the MechaCar to accelerate to 60 mph is the same or more than competitor vehicles within the same price range.
 - Alternative hypothesis: the mean amount of time it takes the MechaCar to accelerate to 60 mph is less than competitor vehicles in the same price range.
 
The following statistical test will be used to test the hypothesis
 - A two-way ANOVA statistical test will be used to test the hypothesis as the ANOVO test will determine if there is a statistical difference of multiple independent variables such as the vehicle name and the MSRP between the distribution mean of the different samples of acceleration time from each vehicle in the study.
the following data will need to be collected from for each vehicle manufacture by competitive brands
 - The average time it takes the MechaCar and competitor cars to accelerate to 60 mph
 - The MSRP of vehicles on the market within $5000 of the MSRP of the MechaCar
 - The brand and model name of each vehicle