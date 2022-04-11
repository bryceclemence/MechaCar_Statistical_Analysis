# MechaCar Statistical Analysis

In this module we we tasked with using R to review the production data on AutosRUs' newest prototype, the MechaCar. The car is having some production issues
and it is our job to review the data to alleviate the trouble so the company can move forward with production.

## Linear Regression to Predict MPG
We first performed linear regression analysis on 51 of the MechaCars that have already been produces, our results are shown below.
![LinearRegression](https://user-images.githubusercontent.com/95730890/162667602-79a114a2-fad5-4e24-8499-4e9753e9022d.PNG)

- The variables that provided a non-random amount of variance to the mpg values are ground_clearance with a p-value of 5.21e^-08, and vehicle_length with a p-value of 
  2.50e^-12
- The slope cannot be considered 0 since the p-value of this regression has a results of 5.35e^-11, which is much lower than the significance level of 0.05%, also 
  concluding that we can reject our null hypothesis.
- This linear model predicts the mpg of MechaCar prototypes effectively since the R-rquared value is 0.7149 (71.5%). While this is relatively low, it is a passing score.


## Summary Statistics on Suspension Coils

The second part of this analysis was comparing the consistency of the suspension coils on three different manufacturing lots. We used summary statistics to determine the mean, median, variance, and standard deviation of the PSI on the suspension coils of those three lots.

### Total Summary
![SummarizeDF](https://user-images.githubusercontent.com/95730890/162672300-d448c129-303c-4f7f-963f-a4e675889df1.PNG)

### Lot Summary
![LotSummary](https://user-images.githubusercontent.com/95730890/162672328-66eb939e-ab2c-4af9-8bbd-5bdfde727bfb.PNG)

Based off our results the suspension coils do not meet design specifications. The specifications for the MEchaCar suspension coils deicate that the variance of the suspension couls must not exceed 100 pounds per square inch. Lots one and two meet this requirement, but lot three does not. If would be worth while to look into why lot three has a drastically different variance than the other lots.


## T-Tests on Suspension Coils

In the final part of our analysis we used the t-test function to dtermine if the PSI across all manufacturing lots is statistially different fromthe population mean of 1,500 pounds per square inch.

### All Lots Test
The t-test for all of the lots gave us a p-value of 0.06028, which is higher than the value of statistical significance, we are unable to reject the null hypothese.

### Lot One Test
The t-test for lot 1 gave us a p-value of exactly 1, which is also higher than the value of statistical significance, once again we are unable to reject the null hypothesis.

### Lot Two Test
The t-test for lot two was 0.06072, which is again, higher than the value of statistical significance, we are unable to reject the null hypothesis.

### Lot Three Test
The t-test for lot three was 0.04168 which is less than the value of statistical significance, making is statistically significant. We can reject the null hypothesis.

# Study Design: MechaCar vs. Competition
A case study that we can perform to determine how the MechaCar is valued against its competition is looking at its value over time. For this analysis we can look at repair costs, especially when it get's up to a higher mileage, frequency of breakdowns, average amount of miles it can max out at before rendering it "totalled" for simple repairs.
The null hypothesis would be that the MechaCar is a better quality car, with its MechaCapabilities, and MechaPerformanceEnhancedTechnologies.
The tests we would performs in the stdy would be a linear regression analysis on the mentioned variables above.
To run these tests we would need data on how many times the MechaCar needed routine maintenance and serious, non-routine maintenance, on average how often the MechaCar broke down or was in a state where it was not drivable, and on average how many miles can be put into the MechaCar before it constantly needs repairs, and the repairs start to cost more than the cars actual worth.

