# Running-Project-GroupE

## Project Title: Factors Affecting Half Marathon Runners’ Performance

### Team Members: Gabriel New, Lisa McGowan, Daniel Conrad, Sirine Khelifi

### Project Description/Outline: 

Analyzing how location, gender, age group and humidity affect the performance of full marathon runners.

### Research Questions to Answer:
1. How does training location correlate to the total time to finish the full marathon.

Alternate Hypothesis: If elevation is related to the total time to finish the full marathon then runners from a higher elevation city than the Marathon location would result in a shorter finishing time.

Null-Hypothesis:  If elevation is not related to the total time to finish the full marathon then runners from a higher elevation city than the Marathon location would not result in a shorter finishing time.

2. Does Gender affect the runners’ performance?

Alternate Hypothesis: If gender is related to the runner's performance then one gender would have a shorter finishing time than the other gender.

Null-Hypothesis: If gender is not related to the runner's performance then one gender would not have a shorter finishing time than the other gender.

3. Does age group affect the runners’ performance?

Alternate Hypothesis: If age group is related to the runner's performance then younger runners would have a shorter finishing time.

Null-Hypothesis: If age group is not related to the runner's performance then younger runners would not have a shorter finishing time.

4. Does Humidity affect the runner's performance?

Alternate Hypothesis: If humidity is related to runner's performance then runners from high humidity cities would have shorter finishing time.

Null-Hypotheses: If humidity is not related to runner's performance then runners from high humidity cities would not have shorter finishing time.


### Datasets and resources to be used:

- https://github.com/llimllib/bostonmarathon/tree/master/results

- http://registration.baa.org/2019/cf/Media/iframe_ResultsSearch.cfm?mode=advanced

- https://openweathermap.org/api

- https://developers.google.com/maps/documentation/elevation/overview

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