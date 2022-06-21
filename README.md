# MechaCar_Statistical_Analysis

## Overview
For this project, we are using R to help AutosRUs with their manufacturing process. The MechaCar, AutosRus' newest prototype is having production issues. We will review the production data to provide insights that will help the manufacturing team. In this analysis, we will:

1. Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.

2. Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.

3. Run t-tests to determine if the manufacturing lots are statistically different from the mean population.

4. Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers.


## Linear Regression to Predict MPG
<img width="508" alt="Deliverable 1" src="https://user-images.githubusercontent.com/100978922/174683137-23b37ac6-589b-4b28-9719-261f94677768.png">

From the data above we can see that:

1. The vehicle length and ground clearance are likely to demonstrate non-random amounts of variance in this model. This means that the length and ground clearance of a vehicle have an impact of the mpg of the MechaCar. The variables vehicle weight, spoiler angle and all wheel drive, all indicate random amounts of variance.  

2. The p-value of our linear regression is 5.35 x 10-6, which is a significantly smaller value than the assumed significance level of 0.05. This means the slope of our linear regression model is not zero and the null hypothesis is rejected. 


3. The r-squared value is 0.7149, which indicates a strong positive relationship between predicting mpg of MechaCar prototypes effectively. 


## Summary Statistics on Suspension Coils
Total Summary:  <img width="457" alt="Screen Shot 2022-06-20 at 7 23 51 PM" src="https://user-images.githubusercontent.com/100978922/174688411-e8020b7f-62cf-4956-94fd-737d90750fed.png">

Lot Summary:  <img width="494" alt="Deliverable 2" src="https://user-images.githubusercontent.com/100978922/174684276-7f1eb27e-348b-4aff-b5db-f8c15c9394f2.png">

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. When we examine the lot summary as a whole, the current manufacturing data does meet this design specification. However, when the data is broken down by lot; we can see that lot 1 and lot 2 do meet this design specification, and lot 3 does not. Lot 1 and lot 2 have a variance of 0.98 and 7.47, respectively. Lot 3 shows a variance of 170.29.

## T-Tests on Suspension Coils
<img width="431" alt="Deliverable 3" src="https://user-images.githubusercontent.com/100978922/174685134-04a6a7e6-58f3-41a2-97d9-4faea15ac8cd.png">

All manufacturing lots: the p-value is 0.06 which is above the assumed significance level of 0.05. Based on this value, there is not enough evidence to reject the null hypothesis that every lot is statistically similar to the presumed population mean of 1500. We will perform a breakdown of every lot.

<img width="423" alt="Deliverable 3 pt2" src="https://user-images.githubusercontent.com/100978922/174685146-0b0468dc-886f-48c3-bd2e-e26e7992d303.png">

Lot 1: has a true sample mean of 1500 and a p-value of 1. The p-value is above the assumed significance level. Therefore, lot 1 is not substantially different from the population mean.
Lot 2: has a very close sample mean, at 1500.2 and p-value of 0.61. The p-value is above the assumed significance level. Therefore, lot 2 is not substantially different from the population mean
Lot 3: has a sample mean of 1496.14 and a p-value of 0.04. The p-value is below the assumed significance level. Therefore, lot 3 is substantially different from the population mean.


## Study Design: MechaCar vs Competition

A study designed to compare performance of the MechaCar against performance of vehicles from other manufacturers:
We already have metrics on vehicle length, vehicle weight, spoiler anlge, vehicle ground clearance, and AWD. Additional metrics to consider for comparison to other vehicles include: cost, fuel efficiency (city and highway), horsepower, maintenance cost, and safety rating.
 
The metrics to test are: 
The null hypothesis is: the MechaCar is priced appropriately based on its performance in relationship to similar cars from the competition.
The alternative hypothesis is: the MechaCar is NOT priced appropriately based on its performance in relationship to similar cars from the competition.
The statistical tests used would be: multiple linear regression 
The data needed to perform these tests include: models from other manufacturers that are comparable to the MechaCar, the average price of each of these models, the average maintenance cost (per year) for each of these models, and each models fuel efficiency (both city and highwauy). The data collected should be over a five year period to gain an accurate representation of how AutosRUs has performed on cost in comparison to it's competing car manifacturers.
