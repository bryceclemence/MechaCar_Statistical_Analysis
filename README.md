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
- Tis linear model predicts the mpg of MechaCar prototypes effectively since the R-rquared value is 0.7149 (71.5%). While this is relatively low, it is a passing score.


## Summary Statistics on Suspension Coils

![SummarizeDF](https://user-images.githubusercontent.com/95730890/162672300-d448c129-303c-4f7f-963f-a4e675889df1.PNG)


![LotSummary](https://user-images.githubusercontent.com/95730890/162672328-66eb939e-ab2c-4af9-8bbd-5bdfde727bfb.PNG)


![tTests](https://user-images.githubusercontent.com/95730890/162672362-2a2fe8e2-dec4-4323-a7b8-ab3a81393f24.PNG)
