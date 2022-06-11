# MechaCar_Statistical_Analysis
 
## Linear Regression to Predict MPG
![screenshot of output](screenshot of output)
Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? ground_clearance, vehcile_length, intercept

Is the slope of the linear model considered to be zero? Why or why not? no, the p-value of this linear regression is below the 0.05 significance therefore the null hypotheses that for linear regression can be rejected and the slope of the linear model is therefore not 0 

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not? yes, the r-squared value is 0.7 which means roughly 70% of our mpg predictions can be explained using the multiple linear model

## Summary Statistics on Suspension Coils
![screenshots]()
![screenshots]()
The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
According to the summary of all the PSI data in the dataset the variance for the suspension coils is 62 which does not exceed the design specifications but when the variance is calculated per manufacturing lot it has been determined the suspension coils produced by manufaturing lot 3 exceed the 100 pound per square inch design specification with a variance of 170 while the variance for manufactuiring lot 1 and 2 are within the design specification with variance values of 1 and 7 respectively

## T-Tests on Suspension Coils
![screenshots]()
![screenshots]()
![screenshots]()
![screenshots]()
Using one-sample t-Test the mean of the PSI on the full sample dataset provided along with a subset of the dataset for each manufacturing lot was compared to the poplation mean of 1500.
The one-sample t-Test for all manufacturing lots within the provided dataset returned a p-value of 0.06 which is above the 0.05 significance level indicating the dataset provided is statistically similar to the population.

The one-sample t-Test for each manufacturing lot returned p-values for Lot1, Lot2 and Lo3 of 1, 0.6 and 0.04 respectively indicating manufacturing lot1 and lot2 are statistically similar to the population but the p-value for lot 3 is below the 0.05 significance level indicating the mean of the PSI reading for lot3 is statistically different from the population

## Study Design: MechaCar vs Competition
In order to quantify how the MechaCar performs against other brands in the market the following statistical study can be used.
The study will use the following metrics to compare to competitors
 - acceleration time (0 to 60mph)
 - MSRP
 
The study will look to proof/disprove the following hypotheses
 - Null hypothesis: the mean amount of time it takes the MechaCar to accelerate to 60 mph is the same or more than competitor vehicles within the same price range
 - Alternative hypothesis: the mean amount of time it takes the MechaCar to accelerate to 60 mph is less than competitor vehciles in the same price range
 
The following satistical test will be used to test the hypothesis
 - A two-way ANOVA statistical test will be used to test the hypothesis as the ANOVO test will determine if there is a statistical difference of multiple independant variables such as the vehicle name and the MSRP between the distribution mean of the different samples of acceleration time from each vehicle in the study.
the following data will need to be collected from for each vehicle manufacture by competitive brands
 - The average time it takes the MechaCar and comptitor cars to accelerate to 60 mph
 - The MSRP of vehicles on the market within $5000 of the MSRP of the MechaCar
 - The brand and model name of each vehicle
 
