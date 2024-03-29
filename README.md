# MechaCar Analysis
## Linear Regression to Predict MPG

<img width="470" alt="Screen Shot 2022-02-13 at 8 05 26 AM" src="https://user-images.githubusercontent.com/92963227/153789002-fbdb8a58-6a20-46fb-a4c1-e4364422c59b.png">

 * Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The vehicle length and the vehicle ground clearance provide non-random amounts of variance to the model.

 * Is the slope of the linear model considered to be zero? Why or why not?

The slope of the linear model is is not zero. This is because the p-value is 5.35e-11 which is much smaller than the 0.05% significance level, indicating a rejection of the null hypothesis meaning that the slope is not zero.

 * Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

This linear model does predict the mpg effectively because the R^2 value is 0.7149, meaning the amount of predictions that will be determined by the model is 71%.

## Summary Statistics on Suspension Coils

<img width="321" alt="Screen Shot 2022-02-13 at 7 00 06 PM" src="https://user-images.githubusercontent.com/92963227/153793042-f741b3cc-c279-49f2-848d-643dca5e1119.png">

<img width="493" alt="Screen Shot 2022-02-13 at 7 00 35 PM" src="https://user-images.githubusercontent.com/92963227/153793053-58e18321-ba3b-4287-acd3-fa921e689c88.png">

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. 

 * Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Using the above tables, it is clear that for the manufacturing data for all lots combined, the variance of the coils is 62.29 PSI. The variance requirement is 100 PSI, which means that the data for all the lots meets the design specification. For the individual lots, lot 1 and lot 2 are within the designated variance, but lot 3 has a variance of 170 which is outside of the bounds of the design specification.

## T-Tests on Suspension Coils
For the t-test, 

All Lots:

<img width="434" alt="Screen Shot 2022-02-13 at 8 13 26 AM" src="https://user-images.githubusercontent.com/92963227/153790292-9aa8a119-46ad-4d02-9178-9d9deee648bd.png">

With a p-value of 0.06, this t-test indicates that there is not enough evidence to reject the null hypothesis with a signifigance level of 0.05. This means that the three lots are similar to the population mean.

Lot 1:

<img width="419" alt="Screen Shot 2022-02-13 at 8 14 38 AM" src="https://user-images.githubusercontent.com/92963227/153790321-925c0824-bb01-4b63-a1dc-ba6d29e8638b.png">

With a p-value of 1, this t-test indicates that there is not enough evidence to reject the null hypothesis with a signifigance level of 0.05. This means that there is no difference between the sample and population mean.

Lot 2:

<img width="419" alt="Screen Shot 2022-02-13 at 8 14 46 AM" src="https://user-images.githubusercontent.com/92963227/153790248-28b363c5-7a04-42f3-981b-18788b575f33.png">

With a p-value of .61, this t-test indicates that there is not enough evidence to reject the null hypothesis with a signifigance level of 0.05. This means that there is not a large difference between the sample and population mean.


Lot 3:

<img width="439" alt="Screen Shot 2022-02-13 at 8 14 55 AM" src="https://user-images.githubusercontent.com/92963227/153790185-c7d59da1-d2bb-4f17-9143-95b81605b7f1.png">

With a p-value of .04, this t-test indicates that there is  enough evidence to reject the null hypothesis and accept the alternative with a signifigance level of 0.05. This means that there is a statistically signifigant difference between the sample and population mean.

## Study Design: MechaCar vs Competition
Write a short description of a statistical study that can quantify how the MechaCar performs against the competition. In your study design, think critically about what metrics would be of interest to a consumer: for a few examples, cost, city or highway fuel efficiency, horse power, maintenance cost, or safety rating.

What metric or metrics are you going to test?

There are many factors that will be useful for a consumer to know when comparing MechaCar to it's competitors, such as price, highway and city fuel efficiency, horse power, maintenance cost, and safety rating. But, with climate change becoming an increasingly important issues, I want to compare the carbon emissions in kg of carbon dioxide produced per mile fore Mecha Car and it's top 5 competitors. 

 * Null Hypothesis (Ho): MechaCar prototypes' average carbon emissions per mile is similar to competitor's vehicles.

 * Alternative Hypothesis (Ha): MechaCar prototypes' average carbon emissions per mile is statistically above or below that of competitor vehicles.

What statistical test would you use to test the hypothesis? And why?

The statistical test I would use to test this hypothesis would be a two sample t-test because it is a dichotomous data type since we are comparing two samples, the MechaCar and it's competitors. 

What data is needed to run the statistical test?
To run this test, data would need to be gathered for the carbon emissions per mile for the MechaCar prototypes as well as for all of the top 5 competing vehicles.
