# Running-Project-GroupE

## Project Title: Factors Affecting Marathon Runners’ Performance

### Team Members: Gabriel New, Lisa McGowan, Daniel Conrad, Sirine Khelifi

### Project Description/Outline: 

Analyzing how location, gender, age group and humidity affect the performance of full marathon runners.

### Research Questions to Answer:
1. How does training elevation correlate to the total time to finish the full marathon.

Alternate Hypothesis: If elevation is related to the total time to finish the full marathon then runners from a higher elevation city than the Marathon location would result in a shorter finishing time.

Null-Hypothesis:  If elevation is not related to the total time to finish the full marathon then runners from a higher elevation city than the Marathon location would not result in a shorter finishing time.

2. Does Gender affect the runners’ performance?

Alternate Hypothesis: If gender is related to the runner's performance then one gender would have a shorter finishing time than the other gender.

Null-Hypothesis: If gender is not related to the runner's performance then one gender would not have a shorter finishing time than the other gender.

3. Does age group affect the runners’ performance?

Alternate Hypothesis: If age group is related to the runner's performance then younger runners would have a shorter finishing time.

Null-Hypothesis: If age group is not related to the runner's performance then younger runners would not have a shorter finishing time.

4. Does humidity affect the runner's performance?

Alternate Hypothesis: If humidity is related to runner's performance then runners from high humidity cities would have shorter finishing time.

Null-Hypotheses: If humidity is not related to runner's performance then runners from high humidity cities would not have shorter finishing time.


### Datasets and resources used:

- https://github.com/llimllib/bostonmarathon/tree/master/results

- http://registration.baa.org/2019/cf/Media/iframe_ResultsSearch.cfm?mode=advanced

- https://openweathermap.org/api

- https://developers.google.com/maps/documentation/elevation/overview

- https://developers.google.com/maps/documentation/geocoding/overview

### Rough Breakdown of Tasks:

-Data Research

-Cleaning of Data

-Break down of coding section:

* Create Dataframe relevant to the hypothesis.
* Sort by relevant variable.
* Use Matplotlib to create charts that best represent the data.
* Use statistics such as the t-test and p-test.
* Draw conclusions

-Presentation 

### Break down by question

#### Question 1
- Create dataframe that will list Cities to pull Latitudes and longitudes using API key.

    - Use Lat and long to obtain Elevation using API key.

    - Add a column of elevation data to the Dataframe.

- Create a Stat summary table.

- Use Matplotlib to generate charts.

- Exports charts as elevation .png file.

#### Question 2
- Create a dataframe that sorts the data by gender.

- Create a stat summary table for each gender.

- Use Matplotlib to generate charts.

- Exports charts as gender .png file.

#### Question 3
- Create a dataframe that sorts the data by age group.
   
   - Create bins for age groups. 

- Create a stat summary table for each age group.

- Use Matplotlib to generate charts.

- Exports charts as age .png file.

#### Question 4
- Sort the dataframe by cities.

- Create a dataframe that includes humidity.

    - Obtain humidity data for each city.

    - Add a column of humidity data to the dataframe.

- Create a stat summary table.

- Use Matplotlib to generate charts.

- Exports charts as humidity .png file.

## Summary of Findings:

### Elevation Summary of Findings
* A linear regression was created to show the elevation of the runners' resident cities and their finishing times. The correlation coefficient is low for the linear regression. The data could still be related, not necessarily in a line. The scatter plot does show a greater number of runners from higher elevations grouped towards the first half of finishing times.
* One of the histograms created shows the means of two groups: those from elevations above Boston (where the marathon took place) and those from elevations below Boston. Even though the means appear to be close on the chart, the P value is very low. This suggests there is significance in the difference of means and that the null hypothesis should be rejected.
* Another histogram was created to compare the means of two other groups: those from elevations over 1500 meters (considered high elevation) and those from elevations below 1500 meters. The P value was also very low, lending more evidence to reject the null hypothersis and consider that elevation and running performance are related.

### Gender Summary of Findings
* There are more men runners than women runners in the 2019 Boston Marathon. 
* Looking into the overall data from the two graphs and analyzing the t and the p values, as well as the total finishing time for each of the Gender groups, we can decrypt that the Null Hypothesis would be IGNORED/REJECTED. The Null Hypothesis stating:
“If  gender is not related to the runner’s performance then one gender would not have a shorter finishing time than the other gender.”
* Gender is then related to the runner’s performance in this analysis, and shows that Men overall had a much shorter finishing time compared to Women, even with having a much larger sample size within the Marathon.

### Age Summary of Findings
* The scatter plot show that the majority of runners in the 2019 Boston Marathon are in the 40-49 age group. The average age of the runner is 43 years old which falls on the regression line and corresponds to 19,ooo seconds (5.27 hours). 
* The scatter plot of age versus Total finishing time shows a clearer distribution of Data. The regression line has a very small positive slope indicating a slight positive correlation between age and total finishing time. 
* The majority of runners are in the 40-49 years old age group and their average finishing time is 3.82 Hours. The shortest average finishing time belongs to the age group 30-39 with  3.69hrs.                   
* The box plot  shows that the mean of finishing time of each group increases as age increases except for group 30-39 where three of the top 5 winners of race belong to.
* The Anova test results of p= o and F value= 405 reject the null hypothesis indicating that the age has a correlation to the total finishing time.

### Humidity Summary of Findings 
* The scatter plot of Humidity% versus Finishing time (s) showed that the majority number of runners in our data, live/train in a weather with humidity over 50%. The mean humidity of our data is 79%. 
* The histogram shows that the two data sets, humidity above the mean of 79 and the humidity below the mean, are overlapping. The p value of 0.050 suggest that the difference between the two data sets is significant. This means the difference between finishing time for runners coming from cities with high humidity is significantly different from the finishing time of runners coming from low humidity cities.
* The regression line on the scatter plot of Humidity % versus Total finishg time in seconds show a horizontal line suggesting no direct correlation between the two variables. In fact, the Pearson's r-value is 0.02, so close to zero suggesting there is little to no correlation between the runner's original city's humidity and finishing time.
