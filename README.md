# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

In the summary output, each Pr(>|t|) value represents the probability that each coefficient contributes a random amount of variance to the linear model, the smaller the amount the less likely to provide variance. According to our results, vehicle length and ground clearance (as well as intercept) are statistically unlikely to provide random amounts of variance to the linear model. variances that would provide random amount of variance to the model are vehicle weight, spoiler angle and AWD.

![image](https://user-images.githubusercontent.com/85718354/138564104-480c10df-9371-438a-9067-7c6ccc35c1dd.png)


Is the slope of the linear model considered to be zero? Why or why not?
The slope of the linear model is not considered to be zero. By looking at the p-value, which is less than 0.05 this determines that the slope is not 0. 


Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

The r squared value from this regression is 0.714 this r squared shows a strong correlation between the data sets meaning that in 71% of tests the linear regression will predict the mpg values correct. 

![image](https://user-images.githubusercontent.com/85718354/138564362-98a3b6da-8fe4-422d-8fb0-357a402cd30e.png)
