# MechaCar Statistical Analysis

## Linear Regression to Predict MPG
There were two variables that provided a non-random amount of variance to the mpg values in the dataset: The vehicle length (Pr(>|t|) = 2.60e-12) and the ground_clearance (Pr(>|t|) = 5.21e-08). Both of these variables have extremely small p-value -- which indicates that we have sufficient evidence to state that those parameters have significant impact on the mpg values in the dataset. Also, the linear regression shows that some of the independent variables had a significant effect on the dependent variable and therefore, the slope of the linear model is not considered to be zero. The r-squared value of this multiple linear regression model is the main indicator of whether the linear model predicts the mpg of the MechaCar: 0.71; and this model would be considered effective.
![This is an image]( https://github.com/gonzojc/MechaCar_Statistical_Analysis/blob/main/Resources/images/linearregression.PNG)

## Summary Statistics on Suspension Coils
Suspension coil presented in the dataset is normally distributed and densely gathered around the mean and median (1498.78 and 1500 respectively). The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch and the variance of the PSI sample distribution is 62.29 meets the design specifications for the MechaCar. However, if we look at the the second table above, it shows that not all lots satisfy the design specifications; "Lot1" and "Lot2" meet the design specification at a variance of 0.98 PSI and 7.47 PSI respectfully, but "Lot3" exceeds the design specifications with its variance of 170.29 PSI.
![This is an image]( https://github.com/gonzojc/MechaCar_Statistical_Analysis/blob/main/Resources/images/lot_summary.PNG)
![This is an image]( https://github.com/gonzojc/MechaCar_Statistical_Analysis/blob/main/Resources/images/total_summary.PNG)

## T-Tests on Suspension Coils
is 0.06028. Assuming our significance level was the common 0.05 percent, this p-value of 0.06 is above our significance level. Therefore, we do not have sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

## Study Design: MechaCar vs Competition
To design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers, I would use the maintenance cost metric and my null hypothesis would be: all of the cars with high maintenance costs will have high mpg. The alternative hypothesis is the mean of our mpg dataset (with low maintenance cost) is greater than the mean of our competitors' mpg dataset (with low maintenance cost). I would use a paired t-test to compare the datasets. I would need to collect and "group by" such levels of maintenance costs and the types of cars and its mpg.
