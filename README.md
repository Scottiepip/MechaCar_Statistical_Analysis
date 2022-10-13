# MechaCar_Statistical_Analysis

## Overview:
Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, we are helping Jeremy and the data analytics team do the following:

  - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
  - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
  - Run t-tests to determine if the manufacturing lots are statistically different from the mean population
  - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll
   write a summary interpretation of the findings.

## Linear Regression to Predict MPG:
![image](https://user-images.githubusercontent.com/108709071/195501043-5bbf11ad-380b-4e41-9162-3128fb333e65.png)

  - According to the result, vehicle_length and ground_clearance are providing non-random amount of variance to the mpg values in the dataset.
  - The slope of the linear model is not consider to be zero. The P-value for the other three variables, vehicle_weight, spoiler_angle and AWD are all greater thean  0.05, it means that all these three variables have significant impact on mpg values.
  - The R-squared value of the linear model is 0.71, which means 71% of the variablilty of our dependent variable (mpg values) is explained using this linear model. So the linear model predict mpg of MechaCar prototypes effectively.

## Summary Statistics on Suspension Coils

Total Summary

![image](https://user-images.githubusercontent.com/108709071/195502913-1eb3cbcf-ec78-4f2d-b4d3-72a031f9d524.png)

Lot Summary

![image](https://user-images.githubusercontent.com/108709071/195503012-a446e6a0-a5f2-4026-8a00-f4ea7e4968c5.png)

  - According to the result, manufacturing data meet this design specification for all manufacturing lots in total as the variance for all lots in total is 62 psi which is lower than the 100 psi allowance. But if we look at the 3 lots individually, we can see that lot 1 and lot 2 meets the specification with variance of only 1 psi and 7 psi, and lot 3 has a variance of 170 psi which is out of specification.

## T-Tests on Suspension Coils

All Lots

![image](https://user-images.githubusercontent.com/108709071/195504454-781d45b3-e03b-496c-9a9f-ae98259ece3b.png)

  - The P-value for all manufacturing lots in total is 0.45 which is greater than the assumed significance level of 0.05%. So we can state that for all manufacturing lots in total there is no statistically different from the population mean of 1,500 psi.

Lot 1

![image](https://user-images.githubusercontent.com/108709071/195504511-e622122e-c7af-4bf3-8bc6-7092f3dc8dc8.png)

  - P-value for lot 1 is 1, greather than the assumed significance level of 0.05%. Lot 1 is no statistically different from the population mean of 1,500 psi.

Lot 2

![image](https://user-images.githubusercontent.com/108709071/195504557-14d85b9e-3ebe-47ba-b44a-4600445ebc73.png)

- P-value for lot 2 is 0.61, greather than the assumed significance level of 0.05%. Lot 2 is no statistically different from the population mean of 1,500 psi.

Lot 3

![image](https://user-images.githubusercontent.com/108709071/195504620-721de018-2b9b-4ead-8679-887cffb850a3.png)

- P-value for lot 3 is 0.042, it is less than the assumed significance level of 0.05%. It meas that we have sufficient evidence to state that lot 3 is statistically different from the population mean of 1,500 psi.

## Study Design: MechaCar vs Competition
Fuel efficiency is one of important factor to determine a vehicle's performance. It will be good to compare the fuel efficiency of MechaCar vehicles to other manufacturers' vehicles based on different class of vehicles.

  - The metrics I will going to teat will be city mpg and highway mpg.
  - The null hypothesis is there is no difference in fuel efficiency between MechaCar vehicles and other manufacturers' vehicles.
  - 
