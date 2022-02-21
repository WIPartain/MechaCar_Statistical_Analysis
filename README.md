# MechaCar_Statistical_Analysis

## Overview

For this project we were tasked with creating a data analysis to provide some insight into the production issues of the MechaCar.  We analyzed the miles per gallon or MPG of the vehicle as well as the production of the suspension coils.  We created a linear regression using R Studio as well as other types of statistical analysis to determine if the car was ready to sell.

## Linear Regression to predict MPG

![](https://github.com/WIPartain/MechaCar_Statistical_Analysis/blob/main/images/regression.png)


From the data we received, we can determine that the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the vehicle. The lower p-values confirm there is a non-random variance leading to lower mpg.

The low overall p-Value of 5.35e-11, is much smaller than the assumed significance level of 0.05%. This determines a rejection of the null hypothesis and implies a non-zero slope.

The r^2 value of roughly .71 indicates that nearly 71% of the mpg predictions will be based on this model, and it proves that this regression is indeed effective.



## Create Visualizations for the Trip Analysis

![](https://github.com/WIPartain/MechaCar_Statistical_Analysis/blob/main/images/lot_summary.png)
![](https://github.com/WIPartain/MechaCar_Statistical_Analysis/blob/main/images/total_summary.png)

The variance of the coils is 62.29 PSI which is much less than the 100 PSI variance requirement.

Lots 1 and 2 were both well within the 100 PSI parameters at 0.98 and 7.47 variance respectively.  However, lot 3 was nearly double the varaince requirement at 170.29 which greatly skewed the variance of the overall population of the coils.

## T-Tests on Suspension Coils

![](https://github.com/WIPartain/MechaCar_Statistical_Analysis/blob/main/images/sample_t_test.png)
![](https://github.com/WIPartain/MechaCar_Statistical_Analysis/blob/main/images/lot_t_test.png)

From here we can see the true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

The mean PSI of the full sample is 1498.78 with a p-value of 0.06.  With a p-value > 0.05, we cannot reject the null hypothesis because the significance level is too high.  

If we analyze each lot individually, we see that lot 1 and 2 have mean PSI's of 1500 and p-values of 1 and 0.61 respectively.  As was true with full sample, the significance level is too high and we cannot reject the null hypothesis for either of these lots.

However, lot 3 has a mean PSI of 1496.14 and a p-value of 0.04 which is below the common significance level of 0.05.  This indicates that we can reject the null hypothesis of the sample mean and the lot mean are not statistically different.


 ## MechaCar Vs Competition
 
I would like to determine how effectively the MechaCar is priced by analyzing the following metrics:

Current MSRP
Safety Rating
MPG
Annual Maintenance Costs
Average Duration of Ownership

After analyzing these variables for several competitors against our own data, we will test them against our null and alternative hypotheses:

Null Hypothesis: MechaCar is priced effectively against its competition.
Alternative Hypothesis: MechaCar is not priced effectively against its competition.

For the statistical tests, I would want to perform a multiple level regression in order to determine which of the aforementioned variables affects the overall value of the cars. By determining which variables are statistically significant, we can see how effectively the MechaCar ranks against its competition in these categories.  We can then assess if the car is priced accurately based on these rankings.

For this test to be conducted effectively, I would need to collect the Current MSRP, Safety Rating, MPG, Annual Maintenance Costs, Average Duration of Ownership for each competitor car with same features of the MechaCar.
