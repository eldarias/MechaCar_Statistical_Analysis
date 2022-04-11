# MechaCar_Statistical_Analysis
Module 15 - Using Statistics and R

---
## Overview
The purpose of this challenge is to run data analysis to review the production data for insights that may help the manufacturing team on AutosRUs' newest prototype, the MechaCar.

The challenge consists of the following four deliverables:
- Deliverable 1: Linear Regression to Predict MPG
    - Perform multiple linear regression analysis to identify which variables in the dataset predict the mpg of MechaCar prototypes
- Deliverable 2: Summary Statistics on Suspension Coils
    - Collect summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots
- Deliverable 3: T-Test on Suspension Coils
    - Run t-tests to determine if the manufacturing lots are statistically different from the mean population
- Deliverable 4: Design a Study Comparing the MechaCar to the Competition
    - Design a statistical study to compare vehicle performance of the MechaCar vehicles against vehicles from other manufacturers. For each statistical analysis, you’ll write a summary interpretation of the findings.  

---


## Linear Regression to Predict MPG
- Results:
    - <image src="./Results/Deliverable1_Results.PNG">
- Question#1/Answer: Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
    - The 'vehicle_weight', 'spoiler_angle' and 'AWD' variables/coefficients provided a non-random amount of variance to the mpg value in the dataset as shown above.
- Question#2/Answer: Is the slope of the linear model considered to be zero? Why or why not?
    - No, the slope of the linear model is not considered to be zero by looking at the p-value from the results above.
- Question#3/Answer: Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
    - The R-squared from the image above shows 0.7149 (71%), which means that the linear regression model was able to explain 71% of the available data.

---
## Summary Statistics on Suspension Coils
- Results:
    - Total Summary:
        - <image src="./Results/Deliverable2_TotalSummary.PNG">
    - Lot Summary:
        - <image src="./Results/Deliverable2_LotSummary.PNG">
- Question/Answer: The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
    - On average for all lots, the total variance is 62, which is within the 100 pounds therefore it meets the design specifications as a whole.  From the individual lot analysis, Lot1 and Lot 2 are within range, but Lot 3 is not, which has a variance of 170.


---
# T-Tests on Suspension Coils
- Results:
    - All Manufacturing Lots t-test results:
        - <image src="./Results/Deliverable3_ttest_All.PNG">
    - Lot 1 t-test results:
        - <image src="./Results/Deliverable3_ttest_Lot1.PNG">
    - Lot 2 t-test results:
        - <image src="./Results/Deliverable3_ttest_Lot2.PNG">
    - Lot 3 t-test results:
        - <image src="./Results/Deliverable3_ttest_Lot3.PNG">
- Overview from the above results: The p-value from the t-test results above for All Manufacturing Lots, Lot 1 and Lot 2 are similar, but Lot 3 has a p-value of 0.04168, which means that Lot 3 is statistically different.

---
## Study Design: MechaCar vs Competition
Due to high fuel prices and concerns with the environment, a statistical study that I believe would be important is to compare city and highway fuel efficiency to see how MechaCar performs against the competition.
The following questions would need to be addressed on the statistical study:
- What metric or metrics are you going to test?
    - City and highway fuel efficiency
- What is the null hypothesis or alternative hypothesis?
    - The hypothesis is that MechaCar has the same efficiency as the competition
- What statistical test would you use to test the hypothesis? And why?
    - One-sample t-test to determine where the same mean of fuel efficiency is statistically different.
- What data is needed to run the statistical test?
    - City and High MPG

---

## Summary:
Overall, the challenge showed us how we can use R to perform statistical studies of the available data.