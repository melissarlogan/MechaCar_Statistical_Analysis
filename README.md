# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

In the summary output, each Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model, the smaller the amount the less likely to provide variance. According to our results, vehicle length and ground clearance (as well as intercept) are statistically unlikely to provide random amounts of variance to the linear model. variances that would provide random amount of variance to the model are vehicle weight, spoiler angle and AWD.

![image](https://user-images.githubusercontent.com/85718354/138564104-480c10df-9371-438a-9067-7c6ccc35c1dd.png)


- Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model is not considered to be zero. By looking at the p-value, which is less than 0.05 this determines that the slope is not 0 .


- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The r squared value from this regression is 0.714 this r squared shows a strong correlation between the data sets meaning that in 71% of tests the linear regression will predict the mpg values correct. 

![image](https://user-images.githubusercontent.com/85718354/138564362-98a3b6da-8fe4-422d-8fb0-357a402cd30e.png)


## Summary Statistics on Suspension Coils

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Per the total summary below, the variance within the suspension coils is shown to be 62, meaning that per the total review it does not exceed the 100 pounds per square inch


![image](https://user-images.githubusercontent.com/85718354/138564852-2fc1e493-4085-43e2-8f9e-06cac95d3f7f.png)

Per the Lot summary this shows that while in total it doesn’t exceed the 100-pound threshold, Lot 3 exceed that with a variance of 170, lot 1 and 2 both have variances <10. This means that in the total summary, the 62 variance is the average across the lots, and majority of this variance can be attributed to Lot 3. Lot 3 should be rejected.

![image](https://user-images.githubusercontent.com/85718354/138564891-0d3e5284-820c-4da9-a624-a15123a53a80.png)


## T-Tests on Suspension Coils

- T-Test on Total

When looking at the T-test across the total population, the mean is 1498.


![image](https://user-images.githubusercontent.com/85718354/138565068-37a3b397-8c31-4d78-9edb-4567a72b165e.png)

When you run the same test on the varying lots the below is found

Lot 1

![image](https://user-images.githubusercontent.com/85718354/138565099-70037d79-d1be-402e-a157-0aaef4b267fa.png)


Lot 2

![image](https://user-images.githubusercontent.com/85718354/138565121-1f9418e3-876a-4697-abae-bcedd19b00ad.png)


Lot 3

![image](https://user-images.githubusercontent.com/85718354/138565140-377cc261-767f-4847-808c-51d824f6dafb.png)


Like the PSI discussion above, lot 3 shows the most variability with the sample mean of x being 1496, with Lot 1 and 2 being 1,500. This is again showing the variability in lot 3 causing the shift in the total summary.

## Study Design: MechaCar vs Competition

In today's world many consumers are becoming more environmentally conscious and price sensitive. miles per gallon is key for individuals who want to get the most out of their money spent on fuel, and who also are concerned with the planets health and are looking to burn less fossil fuel when travelling. 


- What metric or metrics are you going to test?

    I would be testing the mpg of MechaCar compared to their competitors

- What is the null hypothesis or alternative hypothesis?

    H0: MechaCar prototypes' average mpg is similar to competitor's vehicles in the same vehicle class 
    Ha: MechaCar prototypes' average mpg is statistically above or below that of competitor vehicles.

- What statistical test would you use to test the hypothesis? And why?

    I would test this using a two-sample t test as I would be looking to see if the average mpg per the two manufactures was statistically different.


- What data is needed to run the statistical test?

    I would need the mpg from their top competitor as well as the mpg from MechaCar for their varying vehicle types.


