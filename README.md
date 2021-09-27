#MechaCar_Challenge_Analysis
R Programming week 15
# MechaCar_Challenge_Analysis
Working with R programming through RStudio
## Overview of MechaCar_Challenge_Analysis:
After Jeremy is offered the lead with a data analytics team for AutoRU’s.  He has been working with this team for 10 years however, to preform analysis for the new prospective future line testing, he need to brush up on his R programming skills. With my help, Jeremy, has learned retrospective analysis of historical data, analytical verification and validation of automotive specifications and study design of future product testing.  To reach upper management goals, he needs to ensure his statistical background and quantitative metric and clear results to bring to upper management. This includes providing summary statistics for different variables, visualizations for different data sets and our personal interpretation of the statistical test results. Finally, with our experience, we need to propose our own study design, hypothesis, and analysis workflow to improve the AutoRU’s manufacturing process. 
#### The below pseudocode provided us an outline for the analysis ####
•	Deliverable 1:  Linear Regression to Predict MPG 
•	Deliverable 2: Summary Statistics on Suspension Coils  
•	Deliverable 3: T-Test on Suspension Coils
•	Deliverable 4: Design a Study Comparing the MechaCar to the Competition

### MechaCar_Challenge_Analysis: ###
1.	#### Deliverable 1:  Linear Regression to Predict MPG ####

•	The MechaCar_mpg csv is imported and read into a dataframe:

![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/MechaCar_df.PNG) 

•	Linear Regression Model for all 6 variables:
### mecha_lm <- lm(mpg ~ vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD,data=mecha_car_df) ###

![alttext]( https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/lm_mechacar.PNG)

## Linear Regression to Predict MPG
•	summary(mecha_lm) 
![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/summary_mechacar.PNG)

![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/summary_mechacar2.PNG)

•	Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The vehicle length and ground clearance provided a nonrandom amount of variance to the mpg values in the dataset. They may need scaling or transforming to help improve the predictive power of the model.

•	Is the slope of the linear model considered to be zero? Why or why not?
No because the p value is above .05 which considers it to be statistically significant.

•	Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
No because there are outstanding factors that affect the linear model and skew the p and t values. 

2.	#### Create Visualizations for the Trip Analysis ####

![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/suspension_coil_df.PNG)

### Total_summary ###

![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/total_summary.PNG)

### Lot_summary ###

![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/lot_summary.PNG)


3.	T-Tests on Suspension Coils

 
![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/one-sample_t.test.PNG)

 
![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/sample_t.test-lot1.PNG)

 
![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/sample_t.test-lot2.PNG)

![alttext](https://github.com/mbehr11/MechaCar_Statistical_Analysis/blob/main/Resources/sample_t.test-lot3.PNG)

4.	## Study Design: MechaCar vs Competition

•	What metric or metrics are you going to test?
I would test vehicle length vs ground clearance for one test. I would also look at how awd systems affect mpg. 
•	What is the null hypothesis or alternative hypothesis?
my null hypothesis is that mpg is not affected by vehicle weight and ground clearance. My alternate is that the larger the vehicle and more ground clearance the less mpg. 
•	What statistical test would you use to test the hypothesis? And why?
•	I would use a chi-squared test so that we can compare the model years and model types to test my hypothesis.
•	What data is needed to run the statistical test?
I would use data from dealerships and Kelly blue book such as the Mecha_car_csv file.

## Contributing 
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

