# MechaCar Statistical Analysis

## Linear Regression to Predict MPG
Each coefficient contributes a random amount of variance to the linear model. Based on the results, miles per gallon (MPG) and ground clearance are statistically unlikely to provide any variance to the model. From the linear regression model, the r-squared value is 0.68, which means that roughly 68% of all predictions will be correct.

Additionally, the p-value of our linear regression analysis is p-value: 6.712e-11, which is much smaller than our assumed significance level of 0.05%. Ultimately, there is sufficient evidence to reject our null hypothesis, which means that the slope of our linear model is not zero.

The visualization combined with the calculated p-value and r-squared value, revealed that there is a significant relationship between ground clearance and mpg.
R-squared: 0.7119, Adjusted R-squared: 0.6791 indicates a strong correlation and the P-value significantly lower than 0.05, suggest strong correlation and prediction.
![This is an image]( https://github.com/gonzojc/MechaCar_Statistical_Analysis/blob/main/Resources/images/linearregression.PNG)

## Summary Statistics on Suspension Coils
Suspension coil in the dataset is normally distributed around the mean and median (1498.78 and 1500 respectively). The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch and the variance of the PSI sample distribution is 62.29 meets the design specifications for the MechaCar. However, if we look at the the second table above, it shows that not all lots satisfy the design specifications; "Lot1" and "Lot2" meet the design specification at a variance of 0.98 PSI and 7.47 PSI respectfully, but "Lot3" exceeds the design specifications with its variance of 170.29 PSI.
![This is an image]( https://github.com/gonzojc/MechaCar_Statistical_Analysis/blob/main/Resources/images/lot_summary.PNG)
![This is an image]( https://github.com/gonzojc/MechaCar_Statistical_Analysis/blob/main/Resources/images/total_summary.PNG)

## T-Tests on Suspension Coils
The result was 0.06028. Assuming our significance level was the common 0.05 percent, this p-value of 0.06 is above our significance level. There is not enough sufficient evidence to reject the null hypothesis, and we would state that the two means are statistically similar.

## Study Design: MechaCar vs Competition
To design a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers, using the maintenance cost metric and the null hypothesis would be: all of the cars with high maintenance costs will have high mpg. The alternative hypothesis is the mean of our mpg dataset (with low maintenance cost) is greater than the mean of our competitors' mpg dataset (with low maintenance cost). Ideally, using a paired t-test to compare the datasets would work the best. 
