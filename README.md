# MechaCar_Statistical_Analysis

OVERVIEW

A few weeks after starting his new role, Jeremy is approached by upper management about a special project. AutosRUs’ newest prototype, the MechaCar, is suffering from production troubles that are blocking the manufacturing team’s progress. AutosRUs’ upper management has called on Jeremy and the data analytics team to review the production data for insights that may help the manufacturing team.

In this challenge, you’ll help Jeremy and the data analytics team do the following:

  *  Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes.
  *  Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
  *  Run t-tests to determine if the manufacturing lots are statistically different from the mean population.
  *  Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll      write a summary interpretation of the findings.


Deliverables:

  Part 1: Linear Regression to Predict MPG
  
  Part 2: Summary Statistics on Suspension Coils
  
  Part 3: T-Test on Suspension Coils
  
  Part 4: Design a Study Comparing the MechaCar to the Competition



PART 1: Linear Regression to Predict MPG

##Statistical Summary

<img width="498" alt="Linear_Regression_1" src="https://user-images.githubusercontent.com/119356418/229687166-35126c03-15e0-4d9c-85df-7768be496c21.png">

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
 * The vehicle length and vehicle ground clearance are likely to provide non-random amounts of variance. 
 * They both demonstrate a significant impact on miles per gallon on the MechaCar prototype

Is the slope of the linear model considered to be zero? Why or why not?
 * The p-Value of 5.35e-11 is smaller than the significance level of 0.05%; rejecting our null hypothesis, in turn, indicating a slope for this model as not zero.

Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
 * With an r-squared value of 0.7149, we can effectively say the multiple regression model does predict mpg of MechaCar prototypes because at least 71% of all mpg   
   predictions will be determined by this model.
 


Part 2: Summary Statistics on Suspension Coils

##Total Summary Dataframe

The suspension coil’s PSI continuous variable across all manufacturing lots.  The following PSI metrics for each lot: mean, median, variance, and standard deviation.

<img width="1085" alt="Total_Summary" src="https://user-images.githubusercontent.com/119356418/229694658-e451ab3d-cd6b-4789-b5ef-2c0e5af5229b.png">

<img width="1083" alt="Lot_Summary" src="https://user-images.githubusercontent.com/119356418/229694716-57e171ea-edd5-45ec-904a-af74de8f3604.png">

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 

Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

All variances to include variance of the coils at 62.29 PSI and Lot 1 and Lot 2, 0.98 and 7.47 respectively, all show within the 100 PSI requirement.  
All while, Lot 3 shows a much larger variance of 170.29.  It is Lot 3 that is overly causing the variance at the full lot level.

<img width="964" alt="Variance Levels" src="https://user-images.githubusercontent.com/119356418/229698011-e4716120-2df0-4746-ab31-0799a3786747.png">

Part 3: T-Test on Suspension Coils

As shown, is the summary of the t-test results across all manufacturing lots.

<img width="787" alt="mecha_coilTtest" src="https://user-images.githubusercontent.com/119356418/229698765-6c4b75a9-2daf-4337-9e76-59fb16e347f7.png">

With a mean of 1498.78 and a p-Value of 0.06, showing to be higher than the significant level of 0.05, there is not enough evidence to support rejecting the null hypothesis. In summary, the mean of all three of these manufacturing lots is similar to the expected population mean of 1500.

As shown, is the summary of the t-test results across all three lots.

<img width="556" alt="Lot_TTests" src="https://user-images.githubusercontent.com/119356418/229699505-28f1b43b-2e16-4cf9-a581-aae8ff8b3927.png">

Lot 1 sample shows the true sample mean of 1500 along with a p-Value of 1, it is safe to say that we cannot reject the null hypothesis. There is no statistical difference between the observed sample mean and the expected population mean of 1500.

Lot 2 has an almost exact outcome of Lot 1 with a sample mean of 1500.02 and a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the expected population mean of 1500 are similar.

Lot 3 shows a sample mean of 1496.14 and a p-Value of 0.04, lower than the significant level of 0.05%, indicating a rejection of the null hypothesis. This sample mean and the expected population mean are not statistically different.

Part 4:  Study Design: MechaCar vs Competition

What metric or metrics are you going to test?

 * Current Price (Selling): Dependent Variable
 
 * Resale Value: Independent Variable
 
What is the null hypothesis or alternative hypothesis?

 * Null Hypothesis (Ho): MechaCar is priced correctly 

 * Alternative Hypothesis (Ha): MechaCar is NOT priced 

What statistical test would you use to test the hypothesis? And why?
 * A multiple linear regression because it will demonstrate the highest correlation/predictability with the list selling price (dependent variable);   which combination has the greatest impact on price (it may be all of them!)

What data is needed to run the statistical test?
 *




