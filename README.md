# W4-School_District_Analysis-Anaconda

## Overview of the school district analysis
The purpose of this analysis was to explore key metrics in school performance data in math and reading. Throughout this analysis, we look at the overall district performance, the performance of 15 high schools and other frameworks. In our initial phases, we assume that the scores for 9th graders at Thomas High School show evidence of academic dishonesty and should be dropped from the data set. In this analysis, we look at how school performance in terms of passing reading and/or math (scores >=70) is impacted by removing the scores of Thomas High School students in 9th grade. In addition to looking at overall district and school performance, we also examine grade averages at each school, performace by school type and school size. 

## Results 
### Impact on District Summary
The impact to the overall district summary from removing the scores of 9th graders at Thomas High School (referred to as 9 THS scores moving forward) is negligible as show by the figures below. The reason for this is that the number of 9th graders at Thomas High Schools is just over 450 of the approximately 39K students sampled. As these students account for 0.01% of all students in the district, the impact of removing these datapoints is minimal. 

**fig 1: Initial District Summary**
![initial_district_analysis](https://user-images.githubusercontent.com/81983110/118418003-9ebc2200-b684-11eb-98be-895f66b09904.png)

**fig 2: Updated District Summary without 9 THS scores**
![clean_district_analysis](https://user-images.githubusercontent.com/81983110/118418001-9e238b80-b684-11eb-9efe-1241f2dce93e.png)

### How is the school summary affected?
In the school specific summary, the results for the other 14 schools in the district remain the same as conducted in the initial analysis as expected. 


How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type
Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
