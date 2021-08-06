# MechaCar_Statistical_Analysis

Regina Negrycz 
genglist@yahoo.com 
Module 15 Challenge 
Submitted 5 Aug 2021 
Resources/lm_call.PNG
Resources/summary_data.PNG
Resources/grouped_data.PNG
Resources/t_tests.PNG
MechaCarChallenge.R
README

## Linear Regression to Predict MPG

# Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The variables that provided a non-random amount of variance were vehicle length, ground clearance, as well as the intercept.

# Is the slope of the linear model considered to be zero? Why or why not?

The slope of the linear model is not considered to be zero. Our p-value is basically zero, therefore we can state there is sufficient evidence to reject the null hypothesis that the slope of our line was zero.

# Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

No, this linear model does not predict mpg of MechaCar prototypes effectively. When an intercept is statistically significant, it means there are other variables and factors that contribute to the variation in calculating mpg that have not been included in our model.

See https://github.com/genlgist/MechaCar_Statistical_Analysis/blob/main/Resources/lm_call.PNG

## Summary Statistics on Suspension Coils

# Question: The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

The current manufacturing data meets the design specification for all manufacturing lots in total, as seen in total summary table image.  The variance in PSI is approximately 63 pounds per square inch. 

See https://github.com/genlgist/MechaCar_Statistical_Analysis/blob/main/Resources/summary_data.PNG

Manufacturing lot 3 does not meet the design specifications. Unlike the other two manufacturing lots which have a very low variance in PSI, lot 3 has a variance over 170 pounds per square inch.

See https://github.com/genlgist/MechaCar_Statistical_Analysis/blob/main/Resources/grouped_data.PNG

## T-Tests on Suspension Coils

Since our significance level was 0.05 percent, our p-value is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar. Manufacturing lot 3 was below our significance level and the means may be statistically different. Additional analysis should be done with additional samples to confirm.

See https://github.com/genlgist/MechaCar_Statistical_Analysis/blob/main/Resources/t_tests.PNG

## Study Design: MechaCar vs Competition

The MechaCar is being marketed as one of the highest cost vehicles on the market.  The manufacturer assures that over the lifetime of the vehicle consumers will spend 50% less on maintenance compared to their competitors. MechaCar is looking to validate this through a statistical study by comparing cost, highway fuel efficiency and horse power in how they impact annual maintenance costs.  
The null hypothesis is a statement of no difference between a sample mean or proportion and a population mean or proportion. The alternative hypothesis is a contradictory to the null hypothesis. The mean of metric-A from MechaCar can be equal/different to the mean of metric-A from their competition. A t-test can calculate the p-value which can let us know if we can reject the null hypothesis if the p-value is smaller than 0.05 and support the alternative hypothesis or accept the null hypothesis and reject the alternative hypothesis.

We are comparing the means from two populations and can therefore use two sample t-tests.  If we want to know whether one population mean is greater/less than the other, we can perform a one-tailed t-test.  In order to run a statistical test, we would need the mean of both samples, the number of observations and the standard deviation of both samples.
